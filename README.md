# YAPUBFM
Yet Another Ptpimg.me Uploader But For macOS

Make screenshots, directly upload to ptptimg.me, and paste the link straight out from your clipboard.

![yapubfm in action](https://thumbs.gfycat.com/InbornFirsthandDragon-size_restricted.gif)

## Prerequisites
- A ptpimg.me account
- A working bash, curl, awk, sed and osascript (if you have a working Mac, you for sure do; it's sarcasm)

## Installation
1. Download the latest release and unzip it
1. Install it as a service by double-clicking it.
   It will now be accessible from Application --> Services --> YAPUBFM
1. Optionally set a hotkey for the service in System preferences  
  ![Setting a shortcut in System Preferences](https://ptpimg.me/4k80h3.png)
1. Run once and paste in your key. If you mess this up, run `rm ~/.ptpimg.key` in your terminal

## Use
1. Open the service either from the shortcut I highly advise you to make, or from going via the Satus bar --> Application --> Services --> YAPUBFM
1. (Assuming this is not the first-time use, if so check the Installation chapter) Drag out a rectangle or press space to switch to window-selection mode
1. Notification should ping once the link has been copied to your cliboard

## Notes
* The key is left in clear-text, in 0600
* Screenshot is temporarily stored in /private/tmp/toup.png and then deleted at the end of the script. If you want to keep the pic, comment out the "rm ..." line at the end and make your own cp/mv command
* For more information, check the forums on PTP or RED
