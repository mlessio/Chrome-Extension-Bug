# Chrome Extension Bug

Google Chrome extension bug proof of concept for incognito mode.

## The issue

If you have an unsigned and packed extension, you can install it in Google Chrome, then browsing to **chrome://extensions** you can correctly enable the "Allow in incognito" flag from Ubuntu/Linux and from MacOs, **but not** from Microsoft Windows.  
Trying to enable the incognito mode from Microsoft Windows, causes the extension disabling.  
After extension disabling, it is not possible to re-enable it anymore.

## Steps to reproduce

1. Have a Microsoft Windows machine
2. Open Google Chrome
3. Download the sample extension from [here](https://github.com/mlessio/Chrome-Extension-Bug/raw/master/dist/chrome-incognito-poc.crx)
4. Browse to **chrome://extensions**
5. Drag&drop the downloaded crx file to the page
6. Confirm extension installation
7. Check the 'Allow in incognito' flag
8. The extension should be now disabled


