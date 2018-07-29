# yapubfm
Yet Another Ptpimg.me Uploader But For macOS

Make screenshots, directly upload to ptptimg.me, and paste the link straight out your clipboard.

![yapubfm in action](https://thumbs.gfycat.com/InbornFirsthandDragon-size_restricted.gif)

## Prerequisites
- A ptpimg.me account
- Python3
  ```bash
  /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  brew install python3
  ```
- Python packages: ptpimg_uploader, request
  ```bash
  pip install ptpimg_uploader requests
  ```
## Installation
1. Download the latest release and unzip it
1. Install it as a service by double-clicking it.
  It will now be accessible from Application --> Services --> YAPUBFM
1. Optionally set a hotkey for the service in System preferences  
  ![Setting a shortcut in System Preferences](https://ptpimg.me/4k80h3.png)
1. Run once
1. Follow on-screen instructions
  * If you don't have python3 installed, check the prerequisites
  * If you don't have the tool dependencies, they should be installed automatically. If not, check the prerequisites
  * If you don't have a ptptimg.me account, I'm not sure what to say.

## Use
1. Open the service either from the shortcut I highly advise you to make, or from going via the Satus bar -> Application -> Services -> YAPUBFM
1. (Assuming this is not the first-time use, if so check the Installation chapter) Drag out a rectangle or press space to switch to window-selection mode
1. Notification should ping once the link has been copied to your cliboard

## Notes
* The first-time installation is regarded as finished if your token is located in ~/.ptpimg.key. If that's there, it will just skip all the other steps
* The key is left in clear-text, in 0600
* Screenshot is temporarily stored in /private/tmp/toup.png and then deleted at the end of the script. If you want to keep the pic, comment out the "rm ..." line at the end and make your own cp/mv command
* For more information, check the forums on PTP
