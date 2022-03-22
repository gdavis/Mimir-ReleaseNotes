# November Minor Fixes

This update attempts to fix some nagging issues related to high CPU usage that can lock up the application, permission issues with custom save locations, and some crash fixes for the most commonly reported crashes. While I have had a hard time reproducing the high CPU issues, I was able to get closer to finding where it occurs, and it seems to be related to audio processing when scanning for audio silence. I'm crossing my fingers this will resolve the issues for most users, but if you continue to have issues, please use the Contact Support menu item from the app and let me know!

## Changes
- Prevent silence skip analysis operations from performing on video episodes
- Improved error reporting if there is an issue reading or writing to the selected podcast directory. A dialogue to re-select the save location may be presented if the permissions need to be refreshed.
- Fixed an issue that allowed more than one audio silence operation to execute at a time
- Fixed a crash that could occur when loading images
- Fixed a crash that could occur when cycling home promos
- Fixed issue checking for the download state of episodes in some UI elements
- Fixed error playing back episodes that have been downloaded to a custom save location
- Fixed issue with the player cycling through multiple episodes after encountering a playback error for each episode.
- Fixed issue where the home view would perform updates when it was not visible.
- Fixed a crash that could occur when loading podcast detail views
- Added code to prevent idle sleep from triggering when listening to episodes
- Removed volume-change that was applied to the volume slider value to make the audio change more linear. Now works as normal volume sliders tend to work.
- Lowered the priority of audio silence analysis operations, which the system will use to free up more resources when an operation is in progress. For the tech savvy, this means I lowered the quality of service value of the `OperationQueue` to `background` from `utility`.