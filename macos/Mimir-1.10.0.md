# Improved Sync and Audio Playback
*Release 1.7.0 – May 2026*

## New Features
- **New cloud sync engine** — Mimir now uses a completely rebuilt cloud synchronization system for faster, more reliable syncing of your podcasts, playlists, playback progress, and settings across all your devices.
- **Cross-device podcast matching** — Added a new podcast identifier system to allow custom podcast names and multiple podcasts with the same name to be saved in the library.
- **Custom podcast renaming** — Rename any podcast with a custom title that syncs across all your devices.
- **Redesigned podcast detail view** — The podcast detail screen has been completely rebuilt with a new header, improved layout, and a modern look.
- **Custom Podcast Settings** — Customize the audio playback for each podcast and override the global settings on demand for each podcast.
- **Playback settings popover** — Quickly adjust playback speed, skip intervals, voice boost, silence skip, and per-podcast overrides from a popover right in the player.
- **New player view** — The now playing area features a redesigned player with for quick access to controls in the sidebar and menu bar.
- **Episode and podcast info views** — Press Cmd+I or use the "Get Info" action to see detailed information about any episode or podcast in a dedicated info view. Episode descriptions support text selection and tappable timestamps that seek the player.
- **Podcast settings sheet** — Podcast settings are now presented in a polished new sheet with group selection, episode filtering, playback overrides, and more.
- **Redesigned home screen** — The home screen features a new design with horizontally scrolling cards with an improved layout and look.
- **New onboarding flow** — A fresh multi-page onboarding wizard welcomes new users with a clean design.
- **"What's New" screen** — After app updates, a new screen highlights what's changed.
- **Badge permission alerts** — The app now alerts you when system notification badge permissions are disabled, so you can fix it right away.
- **Improved Voice Boost** — Redesigned for smoother, more consistent loudness across all slider positions.

## Improvements
- **Faster "Mark All" operations** — Marking all episodes as played or unplayed is now significantly faster, especially for podcasts with many episodes.
- **Better episode descriptions** — Episode descriptions now render more accurately with improved HTML and Markdown processing.
- **Improved image performance** — Podcast artwork loads faster and uses less memory.
- **Dock badge reliability** — The unplayed episode badge count is now more accurate and updates properly after batch operations.
- **Playback progress sync** — Playback position updates from other devices are now applied more reliably.
- **New typography** — The app now uses new fonts with a refined type style system for a cleaner, more consistent look.
- **Episode list performance** — The episode list scrolls more smoothly and uses less memory, even for podcasts with thousands of episodes.
- **Episode context menu** — The right-click menu for episodes has been reorganized with clearer action names (e.g., "Play Last" instead of "Add to Queue").
- **Sort and filter indicators** — Active sort and filter options are now visibly indicated in the episode options bar.
- **Filtered episode count** — The episode options area now shows how many episodes match your current filter.
- **Better duration estimates for streaming audio** — VBR MP3, AAC, and M4A files now show accurate durations much earlier during playback.

## Bug Fixes
- Fixed an issue where errored podcast feeds could become hidden and inaccessible.
- Fixed a crash that could occur when navigating between views.
- Fixed an issue where the downloads list wouldn't refresh after cloud-triggered downloads.
- Fixed continuous playback not starting correctly on app launch.
- Fixed the podcast detail header collapse animation sometimes getting stuck.
- Fixed an issue where the library sidebar could allow dragging a group onto itself.
- Fixed an issue where playback could end slightly before audio finished playing, especially on Bluetooth devices.
- Fixed an audio glitch that could occur when seeking in MP3 and AAC files.
- Fixed a brief burst of audio from the start of a track when resuming from a saved position.
- Fixed several memory leaks that could prevent the player from being released properly.
- Fixed a data race that could cause incorrect speed calculations.