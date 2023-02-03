# Mimir for iOS – 1.2.0

This update introduces Continuous Playback modes (Append, Shuffle, Legacy), Return to Queue feature for interrupted episodes, updated Playlist Sidebar UI with new buttons and settings, improved performance with bug fixes and changes to the audio player, and podcast feed updates.

I hope you like the updates!
-Grant

## New Features:
• Added Continuous Playback Modes
- Append Mode: An initial playlist is generated and suggested episodes are appeneded to the end of the Continuous Playback playlist. Pressing the refresh button will return the playlist to its original order.
- Shuffle Mode: Episodes that would normally display in Continuous Playback are shuffled for a randomized playlist and new episodes are appended to the list. Pressing the refresh button will generate a new randomized list.
- Legacy Mode: The classic sorting style. Episodes are sorted in a standard fashion, and when sorting by highest priority, episodes will always retain their position in the playlist based on their priority.

• Return to Queue
- You can now automatically have an episode return to the top of the Up Next playlist when it is interrupted and has not yet finished playing.
- Added a button to enable this feature in the Settings > Playback preferences
- Added a button to the current playing episode cell to stop playback and return the episode to the top of Up Next

• Background Updates
- The app now fully supports background tasks to perform feed updates while not using the app.

## Changes:
- Added new refresh button to Continuous Playback list
- Added append mode selection to Continuous Playback settings
- Added new "rating request" alerts that will gently ask users to write a review. Users will be prompted for a review after 3 app launches and asked again every 2 weeks if they choose not to.
- Improved logic around updating subscribed podcast feeds
- Fixed a crash that could occur when the audio player is interrupted by another audio source
- Fixed issue with the mini player queue count circle not looking very circle-like
- Fixed an issue where the audio player could end episodes early if it received a `contentLength` that was smaller than the actual audio file
