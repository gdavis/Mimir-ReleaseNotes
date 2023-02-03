# Mimir for macOS – 1.4.3

Last update took a stab and fixing a nagging permissions issue saving downloads to folders outside of the app's "sandbox", which would make an ugly red exclamation mark show up when trying to download files. This could occur after selecting a custom folder and then when restarting the app, it would "forget" it had permission to access that folder.  Last version's "fix" wasn't a full solution to resolve the problem, so this update takes another stab at resolving it, and this time I believe it is officially squashed! Thank you Mike R. for reporting the issue!

Note that you may need to re-select your download folder to reset the permissions if you were previously encountering this issue.

## Changes
- Fixed an issue with scoped bookmarks to grant permissions to folders to save episode files that are outside of the standard sandboxed locations on subsequent app launches
- Fix left-alignment of library row titles in the left sidebar
- Fixed an issue where episode order was lost when dragging multiple items from the podcast detail into the "Up Next" playlist. (Again, thanks Mike R!)
- Added tooltips for episodes in the podcast detail and library sidebar so full titles can be read in very small window sizes. (Thanks David C. for the suggestion!)
- Updates the wording of the subscription plans to make it more clear that the core features are free, and a subscription is only needed to unlock the premium features.
