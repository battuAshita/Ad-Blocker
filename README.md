# SquadASA_CS200Project

# 1. Welcome to YouTube Automatic Ad-Skipper
Youtube-ad-skipper ia a project aimed at skipping all the skippable youtube ads automatically. Works for ads at the beinging and in the middle of videos as well as the pop-up banner ads. Does not work for ads that have no skip option.

# How it Works
This is a browser extension that runs a content script everytime you load a page thats on YouTube. It uses a background script to listen for movement within the YouTube domain (clicking on another video). When it detects you've started a new video, a function is run that repeatedly tries to define the html element that has the "skip add" click listener. Once it's defined it is clicked with the javascript .click() function.

Mid-video ads and banner adds are detected by a mutation observer that is added to the page whenever a new video is started. This listenes for added or removed child elements in "video-ads" DIV.

# How to Install
Click the green "Clone or Download" button
Click "download ZIP"
Unzip the folder and put it anywhere you like
Open a new tab in your Chrome browser and type in "chrome://extensions" in the search bar. Press enter.
In the upper right corner, turn "Developer Mode" on.
Click "load unpacked"
Find the folder you just downloaded/unzipped "youtube_ad_skipper-master" and click "Select Folder"
Turn "Developer Mode" off
*** if you are getting an error that says " Manifest file is missing or unreadable" it's likey because the "youtube_ad_skipper-master" folder has another folder within it (with the same name).If thats the case, make sure you select the folder within the folder.
