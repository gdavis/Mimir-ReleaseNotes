# Mimir for macOS – 1.5.0

Version 1.5.0 comes with the biggest set of new features for Mimir to date! Launching alongside the new iOS app, the macOS app has been updated with new features that have been in the works for many months. This includes a brand new audio processing engine that greatly improves silence skip, better audio quality at faster or slower playback speeds, voice boost enhancements, and a new sleep timer. iCloud sync has also made a return to the app to keep your desktop in sync with all your iOS devices logged into the same account.

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
  - To better support iCloud and help backing up and sharing of podcast libraries, a new `mimir` filetype has been added to store your podcast library.
  - This filetype can be opened in the app and used to merge or replace the current podcast library.
  - In the unlikely case of a database corruption, this file can also be used to restore your podcast library.


## Changes & Fixes
- Added new error alerts that display when the application encounters problems
- Added new keyboard shortcuts to show different application windows
- Added Silence Skip sound slider to control sound volume in the Effects Preferences tab
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

- Updated episodes to be marked as played when initially adding a new podcast to the library. Episodes added to the feed after the inital library import will be marked as new.
- Updated UI for player controls
- Updated icons and layout for the Preferences window
- Updated the video controls to now immediately fade out when the mouse leaves the window
- Updated the window close button behavior to either close the app or just close the main window. Can be changed in preferences after intially prompted to choose the desired behavior.
- Updated the CoreData model to be simplified and work with the new library file structure
- Updated video playback to no longer use silence skip detection or audio effects. These are now performed only for audio files using the new custom audio processing engine.
- Updated the import action to support new library filetype
- Updated the app store primary category to "News" and secondary category to "Entertainment"

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
