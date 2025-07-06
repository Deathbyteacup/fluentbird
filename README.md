# FluentBird

<p align="center">
  <img src="https://www.dannyking.co.uk/github/fluentbird-logo.png" alt="FluentBird Logo" style="width:50%;">
</p>

FluentBird is a userChrome.css theme for Mozilla Thunderbird, that implemenets Windows 11 Fluent Design and Mica transparency materials.

Created by Danny King - www.dannyking.co.uk
Released under the MIT License

<p align="center">
  <img src="https://www.dannyking.co.uk/github/fluentbird-preview.png" alt="FluentBird Screenshot" style="width:90%;">
</p>

---------------------------------------------------------------

Features
--------
- Implements Fluent Design styling in Thunderbird
- Supports both dark and light modes (system theme)
- Enhances and highlights Mica transparency on Windows 11 systems

Release Notes
--------
- This is the initial release of FluentBird
- Not yet fully tested; bug reports welcome via the GitHub repository
- Untested on Mac and Linux. It should work on these platforms, 
  but will not support Mica/transparency

Credits
--------
FluentBird uses Fluent Design icons provided by Microsoft, licensed under the MIT License. 
Copyright (c) Microsoft Corporation.


---------------------------------------------------------------

Setup Instructions
------------------

1. Enable userChrome.css
- Open Thunderbird  
- Go to **Settings** > **General**  
- Scroll down to **Language & Appearance**  
- Check the box **“Enable userChrome.css”** (it may appear as “Enable legacy user profile customizations” depending on your version)  
- Restart Thunderbird

2. Enable the Mica flags in Thunderbird’s (Firefox-based) advanced configuration:  
   - Open Thunderbird  
   - Go to **Settings** > **General**  
   - Scroll down and click **Config Editor…** under **Advanced**  
   - In the search bar, type `widget.windows.mica` and set it to `true`  
   - Search for `widget.windows.mica.popups` and set it to `2`

3. Make sure no other theme is selected in Thunderbird settings.
   *Do not* select Light, Dark, or any theme from the Thunderbird extension store.
   The theme must be set to "System Theme" or simply unselected.

4. Copy the included `chrome` folder to your Thunderbird profile directory:
   - Locate your Thunderbird profile folder:
     - On Windows: `%APPDATA%\Thunderbird\Profiles\xxxxxxxx.default`
     - On Linux/Mac: `~/.thunderbird/xxxxxxxx.default`
   - Place the entire `chrome` folder inside this profile directory.

5. Restart Thunderbird.

---------------------------------------------------------------

Known Issues
------------
- This is a beta release. Expect bugs and incomplete styling.
- Untested on Mac and Linux (should work, but without Mica).
- Report issues via the GitHub repository.

Also, note that some areas of ThunderBird are rendered outside of the influence of userChrome.css in a "Shadow DOM" - as such, it is not possible to fully theme all elements of Thunderbird.

- The mail section is fully themed, as is the general window chrome. The Contacts, Calendar, Tasks and Chat functions have limited themeing in some areas.
- It isn't possible to style the new message / reply message window, or any other pop-up windows.
- As they are entirely contained within a Shadow DOM, it is also not possible to theme the settings areas.

---------------------------------------------------------------

Questions?  
Check the GitHub repo or open an issue there. Enjoy!

===============================================================
