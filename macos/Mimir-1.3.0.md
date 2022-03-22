# Spring Cleaning Update
*Release 1.3.0 – April 2021*

Happy Spring! With the turn of the season I've been working hard on cleaning up parts of the app that were not performing well, causing crashes, and adding some needed polish to many parts of the app. This is the biggest update for Mimir yet and brings some amazing performance improvements!

The main things you'll notice are drastically increased podcast import and update times, faster "mark as played" tasks, more intuitive context menus, and new Continuous Playback options. The library has received a complete overhaul to the code running it, which fixes many UI bugs and crashes.

With spring cleaning taken care of, I'll now be setting my sights on adding new features to the app such as a downloads view, playlists, and improved podcast discovery. Please email me ([support@mimirpodcasts.app](mailto:support@mimirpodcasts.app)) to let me know what you'd like to see next. I hope you enjoy the update!

– Grant

## Quality of Life Improvements
- The Home view has had the promo section reworked. The promos are now less visually obtrusive and rotate between several more relevant promos
- The image loading system has been rewritten to be much more performant. It also now allows features such as local caching, image expirations, and improved support to resize images more accurately for retina screens
- Added a new 'Release Notes…" option to view the latest version changes
- Added a new "Welcome" option to the Help menu to open the onboarding window

### Importing/Updating Podcasts
- The process for importing and updating podcasts has been cleaned with a fine-toothed comb, and RSS feed import times have been improved by an average of 75%!
- Several fixes have been made that prevented some podcast feeds from importing successfully that had missing optional RSS feed values
- Added a confirmation alert when using Library > Mark All to updated the played state of the entire library

### Library Sidebar
- Groups now show lines indentation lines so its much easier to see what group you are in at a glance
- Automatic sorting has been greatly improved so it no longer undoes the manual sorting you have previously made
- The library will now remember what Groups were expanded between app launches
- A new context menu has been added for moving podcasts into groups
- A new context menu has been added to mark podcasts and group contents as Played/Unplayed
- Updated the unplayed count for Groups to include the unplayed count for all nested subgroups and podcasts
- Marking a Group's contents as played/unplayed will now include all nested groups
- Added some extra spacing in the library list so things are not so cramped

### Podcast Detail
- Added a new context menu option to download episodes for all currently selected rows
- Added a new context menu option to delete downloaded files for all currently selected rows
- Changed the functionality of double-clicking rows to start episode playback immediately. Option+Double Click will now expand the episode description instead of the previous double-click functionality
- Renamed "Automatic Updates" to "Subscribe" to match conventional naming for wanting to keep a podcast updated

### Now Playing Sidebar
- Dragging items to the side has been made easier. Previously you had to drag within the Up Next's background frame, now you only need drag onto the sidebar to drop add new episodes to Up Next
- Added the relative publish date of episodes in the expanded state of the view
- The Continuous Playback options have been reworked so it makes more sense how it is pulling in episodes and sorting them
  - "Latest Episodes" has been replaced with "All Podcasts"
  - Added a new "Downloaded" source option
  - Added a new "Highest Priority" sort option
  - Added a new "Apply Podcast Settings Limit" option to turn on/off the podcast episode limit set in the Podcast Detail view
  - Added more count options when choosing to show Episodes in Continuous Playback. Also added an "infinity" option to have no limit

## General Fixes
- Added new placeholder images that display when loading a podcast image for library rows, continuous playback, search results, recommendations, and home episodes
- Made minor text sizing adjustments to section headers in the Home view
- Made minor layout adjustments to the About window
- Made minor layout and text sizing adjustments to the Onboarding window
- Downloaded episodes will now use the title of the episode as the filename instead of the "guid" of the episode from the RSS feed
- When choosing "Show Podcast" from the Now Playing sidebar the library will scroll to place the selected podcast into view
- Fixed a crash that could occur on Catalina when the home sections update
- Fixed a crash that could occur on Catalina when viewing a Curated List
- Fixed the main play button to being playing episodes from continuous playback if there is nothing currently playing, or in the Up Next playlist
- Fixed a crash that could occur when using Control+Click to show context menus
- Fixed crash that could occur when deleting a podcast nested in a group
- Fixed crashes that could occur when the home section updates with new content
- Fixed a memory leak that could occur when the app sets up observers for UI bindings in quite a few places
- Fixed a bug where selecting multiple episodes from the podcast detail, then right clicking another episode that is not selected would present the wrong options
- Fixed an issue where dragging a podcast into a collapsed group would make the expansion arrow be in the wrong position
- Fixed an issue where selecting a podcast within a group, then collapsing that group would take you away from the podcast detail and to the Home view
- Fixed the sortOrder to a use a more logical value when initially when creating new groups or adding a podcast
- Fixed an extra visual gap that would appear in the podcast detail when a podcast does not have any defined categories
- Fixed an issue where adding a group would not immediately start an editing process to change the name of the new group
- Fixed an issue where a native vertical drag-line indicator would display when dragging episodes into the Now Playing list

