# Mimir for macOS – 1.6.0

Happy New Year! Mimir is starting off 2023 with a big update that adds a new Downloads view and a reworked custom audio player that fixes many playback issues for a solid playback experience. Thank you for your support while I continue to update the app to make it a great podcast player. Expect to see many new updates coming this year!

## New Features
Audio Player 2.0
- Internally reworked to be much more stable and accurate
- Added an AirPlay menu to the main player controls
- Improved controls for Bluetooth headsets (e.g. Airpods) with skipping forward/backward in an episode
- Many bugs fixes and stability improvements

Automatic Downloads
- Enabled in Podcast Settings, Mimir will now download new episodes added to the feed for your selected podcasts
- This setting syncs with other devices
- New Downloads section added to the sidebar
- View a summary of the number of files and total space used
- View downloads organized by podcast
- Search to quickly find downloaded episodes
- Sort by most file size, number of files, or podcast title
- Quickly remove individual files, all files for a podcast, or all downloads in the library
- Full Drag & Drop support
- Added ability to drag downloaded episodes outside of Mimir and into other applications

Local notifications improvements
- Podcasts that are marked to show local notification will now display alerts for newly added episodes.
- Added quick-actions to the notifications to play the episode now, next, later, or view the source podcast.

Podcast Setting Redesign
- Updated the podcast settings with an improved layout and room for more options

## Bug Fixes 
- Fixed an issue that kept downloaded files on disk longer than they should because they were not being properly marked as played.
- Fixed a crash that could occur when reading data that caused a race condition
- Fixed a memory leak that could occur when parsing audio data packets
- Fixed issues where the episode could complete too early when skipping forward
- Fixed a crash that could occur when updating the recommendations view
- Fixed an issue where a separate download could start when the audio player also downloads the same file. This fixes issues with studdering audio when loading a new episode on a poor network connection.
- Fixed an issue where audio from the beginning of the file could be played when the player is rebuilt from an audio session interruption
