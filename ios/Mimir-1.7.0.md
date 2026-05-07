# Improved Sync and Audio Playback
*Release 1.7.0 – May 2026*

## New Features
- **New cloud sync engine** — Mimir now uses a completely rebuilt cloud synchronization system for faster, more reliable syncing of your podcasts, playlists, playback progress, and settings across all your devices.
- **Cross-device podcast matching** — Added a new podcast identifier system to allow custom podcast names and multiple podcasts with the same name to be saved in the library.
- **Custom podcast renaming** — Rename any podcast with a custom title that syncs across all your devices.
- **"What's New" screen** — After app updates, a new screen highlights what's changed. You can revisit it anytime from Settings.
- **Badge permission alerts** — The app now alerts you when system notification badge permissions are disabled and prompts you to enable them so you can fix it right away.
- **Improved Voice Boost** — Redesigned for smoother, more consistent loudness across all slider positions.

## Improvements
- **Faster "Mark All" operations** — Marking all episodes as played or unplayed is now significantly faster, especially for podcasts with many episodes.
- **Better episode descriptions** — Episode descriptions now render more accurately with improved HTML and Markdown processing.
- **Improved image performance** — Podcast artwork loads faster and uses less memory.
- **Dock badge reliability** — The unplayed episode badge count is now more accurate and updates properly after batch operations.
- **Playback progress sync** — Playback position updates from other devices are now applied more reliably.
- **New typography** — The app now uses new fonts with a refined type style system for a cleaner, more consistent look.
- **Updated colors and styling** — Refined background colors, fonts, and layout spacing for a more polished look.
- **Background feed refresh** — Improved how feeds refresh in the background so new episodes are ready when you open the app.
- **Feed error indicator** — Podcasts with feed errors now show a visible indicator so you know when something needs attention.
- **Better duration estimates for streaming audio** — VBR MP3, AAC, and M4A files now show accurate durations much earlier during playback.
- **Improved Playback for CarPlay** – Interruptions for reading text messages, turn-by-turn directions, etc will now pause podcast playback.

## Bug Fixes
- Fixed an issue where errored podcast feeds could become hidden and inaccessible.
- Fixed a crash that could occur when navigating between views.
- Fixed playback progress sometimes not updating correctly from cloud sync.
- Fixed an issue where the downloads list wouldn't refresh after cloud-triggered downloads.
- Fixed continuous playback not starting correctly on app launch.
- Fixed swipe actions that conflicted with "back" swipes on iOS 26.
- Fixed HTML decoding for episode descriptions.
- Fixed an issue where playback could end slightly before audio finished playing, especially on Bluetooth devices.
- Fixed an audio glitch that could occur when seeking in MP3 and AAC files.
- Fixed a brief burst of audio from the start of a track when resuming from a saved position.
- Fixed several memory leaks that could prevent the player from being released properly.
- Fixed a data race that could cause incorrect speed calculations.
