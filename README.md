# FirefoxIncognitoRebind
For the FireFox browser, changes the keybind of CTRL + SHIFT + N so that instead of opening a previously closed window, it opens a new private window.  This is to match the keybind Chromium uses to open an incognito window.

Ctrl + Shift + P still words as the default keybind to open a new private browser.  This script only affects Ctrl + Shift + N.

Credit:  <br/>
         - https://searchfox.org/mozilla-release/source/browser/base/content/browser-sets.inc as a resource for the command list of all hotkeys in Firefox.
        <br/>
         - https://support.mozilla.org/en-US/kb/customizing-firefox-using-autoconfig as a guide for using Firefox AutoConfig
         <br/>
         - https://www.reddit.com/r/firefox/comments/kilmm2/restore_ctrlshiftb_library_by_setting_configjs/ :  Credit to u/aveyo on Reddit for providing the base code template to modifying hotkeys through a Firefox Javascript template.

# Instructions

1) Locate your Mozilla Firefox root directory.  By default, this will be loated in ```C:\Program Files\Mozilla Firefox\```

2) Download the autoconfig.js file and place it in the ```Mozille Firefox\defaults\pref``` directory.  This file will prompt the browser to load the specified script files to run.  (This process may require administrative privileges).

2.5 A)  If Firefox doesn't load the autoconfig file, then in the Firefox Browser, type aboutconfig in the url.  In the page's search bar, type ```[general.config.filename]``` and set the value to the .cfg file that you wish to run.

2.5 B)  In the same ```about:config``` page, search ```[general.config.obscure_value]``` and set the value to 0

3) Download the firefox.cfg file and place it in the root directory of Mozilla Firefox (```C:\Program Files\Mozilla Firefox\```).

4) Close all Firefox Browsers and restart.  Alternatively, go to Firefox and search about:support in the URL bar.  Click ```[Clear Startup Cache]``` and restart Firefox to force the autoconfig file to load in.
