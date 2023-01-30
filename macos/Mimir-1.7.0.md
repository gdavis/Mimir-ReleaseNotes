# New Modes Update
*Release 1.7.0 – February 2023*

This update brings new modes to the Continuous Playback feature, playlist sidebar updates, and improves how often the app updates podcast feeds.

I hope you enjoy the new changes!

-Grant 

## New Features:

• Added Continuous Playback Modes
- Append Mode: An initial playlist is generated and suggested episodes are appeneded to the end of the Continuous Playback playlist. Pressing the refresh button will return the playlist to its original order.
- Shuffle Mode: Episodes that would normally display in Continuous Playback are shuffled for a randomized playlist and new episodes are appended to the list. Pressing the refresh button will generate a new randomized list.
- Legacy Mode: The classic sorting style. Episodes are sorted in a standard fashion, and when sorting by highest priority, episodes will always retain their position in the playlist based on their priority.

• Return to Queue
- You can now automatically have an episode return to the top of the Up Next playlist when it is interrupted and has not yet finished playing.
- Added a button to enable this feature in the Preferences > Playback
- Added a button to the current playing episode cell to stop playback and return the episode to the top of Up Next

• Updated Playlist Sidebar UI
- Reworked the Continuous Playback button with a new toolbar.
  - Moved the "Clear Up Next" button to the left of the toolbar
  - Changed the "Enabled Continuous Playback" to a new infinity symbol button
  - Added a refresh button that returns the Continuous Playback playlist back to its original order when using Append mode, or loads a new randomized set of Episodes when using Shuffle mode.
  - Added a new 'gear' button to the playlist sidebar that displays a popover for changing Continuous Playback settings
- Episode cells have new buttons that appear on mouse-over for quick-actions

## Changes:
- Added a new option to show or hide iCloud sync status in the library sidebar
- Added a new 'gear' button to the player controls that opens the Preferences Playback tab
- Improved logic around updating subscribed podcast feeds
- Moved the podcast download directory to the Podcasts settings tab
- Fixed border rounding issue on episode cells in sidebar
- Fixed a crash that could occur when the audio player is interrupted by another audio source
- Fixed some alignment and corner rounding issues in the playlist sidebar
