# New Audio Engine + iOS App Release
*Release 1.5.0 – Summer 2022*

Version 1.5.0 comes with the biggest set of new features for Mimir to date! Launching alongside the new iOS app, the macOS app has been updated with new features that have been in the works for many months. This includes a brand new audio processing engine that greatly improves silence skip, better audio quality at faster or slower playback speeds, voice boost enhancements, and a new sleep timer. iCloud sync has also been added to the app to keep your desktop in sync with all your iOS devices logged into the same account.

Also included is the often requested mini player that can be opened from the macOS menu bar and is configurable to always stay on top of other windows for quick access to the playback controls. I've also been able to fit in improvements such as being able to favorite or archive episodes, UI additions for more easily downloading episodes, and a slew of other improves and bug fixes. 

Thank you for your suggestions and help improving the app!

-Grant


## Major Features
- Custom Audio Engine
  - Much improved silence detection and playback performance when skipping silent audio
  - Drastically reduces CPU usage from scanning files for silence. Now performed in real-time while using much less CPU power. 
  - New Voice Boost toggle adds additional volume to voice audio frequencies
  - New Sleep timer automatically pauses playback after a duration
  - New playback speeds from 0.8x-2.5x with much better sounding audio quality. No more chipmunks! 🚫🐿
  - Efficient data loading when streaming audio files from a remote webserver. Only loads ahead of what is playing.
  
- iCloud & Preferences Sync
  - Sync your library, playlist, preferences, and episode playback progress with all your devices

- New Mini Player
  - Control playback at a glance with a beautiful new mini player
  - Open from the new macOS menu bar icon or with a keystroke (Command + R)
  - Detachable from the menu bar and can placed on any screen
  - Configurable to sit on top of all other windows, can be changed in the Preferences window

- Favorite & Archive Episodes
  - Includes new filtering options in the podcast detail to find your favorites, or hide episodes you don't want to see.
  
- New Custom Library File
  - To better support iCloud and help backing up and sharing of podcast libraries, a new `mimirlibrary` filetype has been added to store your podcast library.
  - This filetype can be opened in the app and used to merge or replace the current podcast library.
  - Automatic backups of your library will save a `mimirlibrary` that can be used to restore the library in case of data loss.
  - In the unlikely case of a database corruption, this file can also be used to restore your podcast library.


## Changes & Fixes
- Added support to import libraries from Apple Podcasts
- Added animation to fade in images when they are loaded
- Added context menu actions to move podcasts or groups to the top level when in a parent group
- Added new error alerts that display when the application encounters problems
- Added new option to disable window blur effects that can improve overall window performance
- Added new keyboard shortcuts to show different application windows
- Added Silence Skip sound slider to control sound volume in the Effects Preferences tab
- Added Silence Skip Sound selection option in the Effects Preferences tab
- Added Voice Boost switch and volume slider in the Effects Preferences tab
- Added new slider options for playback speeds in the Effects Preferences tab. Now you can crank it all the way up to 2.5x!
- Added option to keep the video view on top of other windows in General Preferences tab
- Added custom User Agent for HTTP requests for podcast publishers to better track app usage
- Added functionality to automatically switch playback to a local file when it finishes downloading. Playback will still start immediately using HTTP streaming.
- Added tooltips for home and playlist cells
- Added dock context menu to quickly open different application windows
- Added functionality to always open the main app window when clicking the dock menu icon
- Added context menu options to the podcast detail to favorite and archive episodes
- Added a download button to episodes in the Now Playing sidebar
- Added a close button for the upgrade banner in the library sidebar
- Added a "audio effects disabled" button that displays when the app uses the standard legacy player for video or audio formats not supported by the custom audio player. The buttons for the disabled effects will be hidden when this is displayed. Clicking the button will display an alert explaining why the custom audio engine is not used
- Added a new button to remove the current playing item
- Added a new button to the up next list to clear queued items
- Added a new menu item and key command to clear up next queue
- Added icons to show iCloud sync activity in the library row in the left sidebar

- Improved performance of the podcast detail view when resizing the window
- Improved error alerts when handling network errors
- Updated Onboarding and application menu items to include importing from Apple Podcasts
- Updated episodes to be marked as played when initially adding a new podcast to the library. Episodes added to the feed after the inital library import will be marked as new.
- Updated UI for player controls
- Updated icons and layout for the Preferences window
- Updated the video controls to now immediately fade out when the mouse leaves the window
- Updated the window close button behavior to either close the app or just close the main window. Can be changed in preferences after intially prompted to choose the desired behavior.
- Updated the CoreData model to be simplified and work with the new library file structure
- Updated video playback to no longer use silence skip detection or audio effects. These are now performed only for audio files using the new custom audio processing engine.
- Updated the import action to support new library filetype
- Updated the app store primary category to "News" and secondary category to "Entertainment"

- Fixed the animation of the preferences window when changing tabs
- Fixed an issue caching images between app launches
- Fixed where cached images were not being set correctly, causing an extra network load
- Fixed issue with small podcast images not sizing correctly
- Fixed an issue seeking the player to the correct starting position on startup
- Fixed a crash that occurred when changing Bluetooth devices
- Fixed visual issues when scroll bars are always visible that would make the highlight outlines render incorrectly in the Now Playing sidebar
- Fixed issues with sandbox permissions when saving podcasts to custom directories
- Fixed issues updating Control Center with episode information
- Fixes missing icon issues on older macOS versions
- Fixed an issue where the playing episode cell could be scrolled
- Fixed button highlight states getting "stuck" when switching to another app window
- Fixed issue where download progress would not properly update the progress indicator
- Fixed an issue where deleting the last episode in a podcast directory would not remove the empty directory from disk
- Fixed issues showing the incorrect state for the player play button
- Fixed a crash that could occur in Continuous Playback when an episode's playback status has not yet been created
- Fixed issue with Continuous Playback list not showing enough episodes to fill the set limit when podcast episode limits are applied
- Fixed an issue where the download icon for podcast episodes would enter an error state when cancelling a download
- Fixed an issue where an error alert would display when cancelling a download
- Fixed the recommendations view from refreshing too often and performing a flash when reloading content
- Fixed an issue with the recommendations view resetting the scroll position to the top when entering and leaving the view
- Fixed an issue where the highlight border stops appearing in the recommendations view
- Fixed issue where selecting many episodes and right clicking for a context menu could lockup the UI
- Fixed an issue where the Continuous Playback logic for hours could incorrectly use a podcast's episode limit instead of correctly calculating by duration
- Fixed issue with episodes not being marked played when listening to over 50% of the episode. An episode's played state is now updated when it is no longer in the episode playlist.
