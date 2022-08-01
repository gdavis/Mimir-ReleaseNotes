# Mimir 1.0.0 Beta

Welcome to the Mimir beta test! 💥🚀🎉

The iOS app has been in development for almost a full year but is finally ready to get into your hands and play some podcasts. Mimir fully supports both iPhone and iPad, including split view on the iPad. 

The macOS app is also receiving a big update along with the release of this iOS version, and can also be tested with TestFlight on the Mac when using macOS Monterey. If you can, please test both versions and enable iCloud to help test the syncing features of the app.

Since this is a beta test, please be aware there are bugs to squash and in some very rare cases some major issues may occur such as data loss in your library. The iOS version adds iCloud sync to keep all your devices working together, and a new library file format was needed to support it. This new library system needs your help to work out all the kinks!

Mimir is a solo-developer project, so please bear with me as I work to resolve all the major issues with the new custom audio engine and iCloud sync, the two most technical features in the app. Suggestions and feature improves are very welcome as Mimir takes shape for iOS. 

Thank you for helping test my app!


## App Features

The iOS release of Mimir brings a completely rewritten custom audio engine with some big improvements to silence skip, audio quality at higher playback speeds, a voice boost feature, sleep timer, and efficent usage of network data when streaming episodes. Being the core feature of the app, this needs rigorous testing and is a very complex feature, so please let me know if you run into any serious problems with the audio engine as soon as you can.

Please note that the new audio effects only work with audio files, so silence skip, voice boost, and the improved audio quality will not apply to video podcast episodes. 


### Main Feature Highlights
- Custom Audio Engine
  - Much improved silence skip detection
  - Voice boost to add volume to voice audio frequencies
  - Sleep timer
  - Playback speeds from 0.8x-2.5x
  - Efficient data loading when streaming audio files
- iCloud Sync
- Preferences Sync
- Up Next Playlist
- Continuous Playback
  - Let Mimir do the work to find the episodes to listen to next, using custom sorting and filtering options along with custom set priority ratings to keep the podcast you like most at the top of the list.
- Context Menus
  - Quickly access controls for groups, podcasts, and episodes from context menus
- Podcast Groups
  - Organize your podcast library into groups that can be nested into as many other groups as you like. No more endless lists.
- Podcast Recommendations
  - Curated Lists
  - Recommendations based on your highest priority and top played podcasts, region, and most subscribed categories
- Podcast Search
- Podcast Category Directories
- Swipe actions for podcasts and episodes for quick, commonly used actions
- Custom RSS Feed Support
  - Password-protected Feeds
- App Customization
  - Color Schemes
  - Custom Tint Color
- Favorite or Archive Episodes
- Download or Stream Episodes 
- Light and Dark Mode Support
- Dynamic Type Support


## Known Issues
These bugs are already in queue for fixing and will be addressed before release. If you encounter any of these, please know a fix is coming soon! If you can consistently reproduce these issues, please use the Bug Report feature in the Support menu to let me know how you made it happen.

- Skipping forward in a episode that has not yet been downloaded can rarely fail and skip to the next track.
- Some episodes can fail to complete playback when reaching the end of the file and not automatically advance to the next track. Workaround the issue by manually tapping the next track button.
- Some episodes with very long titles, or when using large dynamic type, can cause the UI to be cramped and cut off certain UI elements.
- When using Bluetooth player, such as car audio, sometimes an episode can show an incorrect duration. Seeking in this state can fail and cause the player to play the next episode.
- When syncing with other devices, sometimes data from the local device will overwrite the iCloud data.

## Tips and Tricks
- Tap and hold on the navigation bar on any screen to quickly change from light or dark mode.
- Tap and hold on groups, podcasts, and episodes to get a context menu for common actions.
- Swipe left or right on podcast or episode cells for quick actions.
- Tap and hold to rearrange the up next episode playlist.
- Use the podcast priority setting to have episodes from your favorite podcasts appear more often in the Continuous Playback list.


## Coming Later in Beta
The following features are coming later in the beta test and will arrive before the iOS app launches to the app store.

- Import from Apple Podcasts
- More Color Schemes
- Custom Silence Skip Sounds
- In-App Purchases
- Release Notes


## Testing
During testing, use the Support menu to email me feature requests and suggestions, and the Bug Report form to submit any issues you encounter. You can also email me directly at support@mimirpodcasts.app  

Mimir currently supports importing podcast library in OPML format, which most popular podcasting apps support. Import by saving an OPML file to the Files app and choosing the "Open in Mimir" option. 

The beta is planned to hopefully only take a month or so before Mimir is ready to launch, but could take longer if any major issues are found. Please take the time to help get the app ready by submitting feedback and bug reports. Mimir is a one-developer project, so all the help I can get in testing goes a long way!


## Future Roadmap
The features listed here are things I'd love to get into future versions of Mimir, but are not yet available. Please let me know if you don't see a feature you'd like to see added to the list!

- CarPlay Support
- watchOS Support
- MP3 Chapter Support
- Support for embedded episode images
- Support to skip the first/last N seconds of audio per podcast
- Support for custom audio effect settings per podcast
- Sharing
- Siri Shortcuts
- Widgets
- Custom App Icons
- Background Tasks for RSS Feed Updates
- Notifications
- Localization
