# FluentBird

<p align="center">
  <picture>
    <source srcset="https://www.dannyking.co.uk/github/fluentbird-logo dark.png" media="(prefers-color-scheme: dark)">
    <source srcset="https://www.dannyking.co.uk/github/fluentbird-logo.png" media="(prefers-color-scheme: light)">
    <img src="https://www.dannyking.co.uk/github/fluentbird-logo.png" alt="FluentBird Logo" style="width:50%;">
  </picture>
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

This is the first stable release of Fluentbird, however, there may still be some bugs and issues, specifically when using operating systems other than Windows 11.

There are now issue templates, when reporting issues, please let me know exactly which OS and version you're using, the version of Thunderbird, and any specific settings related to the bug. Thanks!

1.0.2 Release Notes
--------
- Fixes an issue where mail header labels were misaligned when "Hide Label Columns" was unselected in Message Header Settings.

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
   - Click **Config Editor…** under **Advanced**  
   - Search for `toolkit.legacyUserProfileCustomizations.stylesheets`  
   - Set it to `true`  
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

4. Copy the included files to the `chrome` folder in your Thunderbird profile directory:
   - Click on Help > Troubleshooting information
   - Scroll down to "Profile Folder" under "Application Basics" and click "Open Folder"
   - Create a new folder named `chrome` inside your profile folder, if it does not already exist
   - Place the userChrome.css file and all folders into the 'chrome' directory
   
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
