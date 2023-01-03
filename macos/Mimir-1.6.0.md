# New Year Update
*Release 1.6.0 – January 2023*

## New Features
Player Improvements
- Reworked for a more stable experience
- Improved the overall performance of the player
- Fixed issues with seeking accuracy, especially with long episodes
- Fixed the most common player bugs, including the notorious "stuck at end" of episode bug

Automatic Downloads
- Added an option to podcast settings that, when enabled, will automatically download episode files when added to the feed
- This setting will sync between devices when using iCloud

Added a new Downloads view to the sidebar. From here you can see all files that have been downloaded and manage your downloads.
- View a summary of the number of files and total space used
- View downloads organized by podcast
- Search to quickly find downloaded episodes
- Sort by most file size, number of files, or podcast title
- Quickly remove individual files, all files for a podcast, or all downloads in the library.
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
