# Mimir for iOS – 1.3.0
CarPlay support is now available! This update brings the familiar Mimir interface to your car so you can manage podcast playback on the go, as well as a bunch of fixes for the most annoying iCloud and audio player bugs.

The new CarPlay interface includes the following tabs and features:

### Playlist
- View the playing episode, Up Next, and Continuous Playback playlists
- Play episodes from Up Next or Continuous Playback
- Clear currently playing episode
- Clear the Up Next queue

### Podcasts
- View the groups and podcasts in your library. (The number of subgroups may be limited by your CarPlay device.)
- Quickly change library sorting
- View and play podcast episodes

### Episodes
- View and play episodes from:
  - Just Added
  - Highest Priority
  - Favorites
  - Downloaded
  - Continue Listening
  - Recently Played

### Settings
- Enable Continuous Playback
- Enable Return to Queue
- Change Skip Forward/Backward seconds
- Enable Audio Effects (Silence Skip, Skip Sound, Voice Boost)


## Other changes and fixes:
- Improved the loading performance when first opening the episodes tab for large libraries
- Fixed issue with in-app purchase buttons not working
- Fixed issue with error alerts stacking when multiple errors occur. New error alerts will only display when no other error alert is present.
- Fixed a rare crash that could occur when scheduling updates
- Fixed a sync issue when importing playlist items on a device that is missing the episode because the feed is out of date
- Fixed an issue where private feeds could not load when the device was locked
- Fixed a rare crash that could occur when updating podcast feeds
- Fixed an issue where an episode synced to another device would not automatically download
- Fixed an issue where an episode with a previous playback position could start back at the beginning when played again
- Fixed an issue where pausing the player could incorrectly adjust the timeline position
- Fixed an issue where an interrupted download could load audio from the beginning of the file when resuming playback
