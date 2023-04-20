# New Sharing Features
*Release 1.8.0 – April 2023*

This relatively small release includes some new sharing features, UI improvements, and bug fixes. You can now share links to episodes or podcasts through various sharing services. In a future update I plan on adding support for sharing to specific timestamps, or sharing a short audio clip.

- Added a "share podcast" button to podcast detail views
- Added share options to share an episode or a podcast from context menus
- Added a share button to episode detail rows
- Added a "more" button to the main player that has several context menu actions: Play Next Episode, Return Episode to Queue, Sharing, and Playback Preferences. This replaces the previous "gear" button that opened playback preferences.
- Added some user reviews to the purchases window. Thanks for all the stars!
- Updated the podcast detail episode rows so the "expand dots" are always visible and now on the trailing side of the view
- Improved performance scrolling and resizing the window when in the podcast detail view
- Improved database fetch performance when fetching a lot of episodes in the podcast detail
- Fixed an issue with the "Return to queue" button in the playlist sidebar not being properly hidden when needed
- Fixed a memory leak that could lead to a crash from download operations
- Fixed a text color issue for the library sidebar that would make the text hard to read for a selected row when focus is on another view
- Fixed an issue where downloads made from menus might not trigger the UI to show download progress in other locations
