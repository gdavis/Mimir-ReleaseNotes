# Audio Bug Fixes
*Release 1.11.3 – May 2026*

Recently I've been working on adding support to play additional audio file types other than the standard MP3. This lead to new bugs popping up, and I had to do some pretty big architecture changes to get everything happy. This update should bring the player back to a stable place while also expanding support for more audio types. If you still are having issues please email suppport@mimirpodasts.app

- Improved audio playback stability when playing non-MP3 files
- Fixed a bug where seeking forward/back could adjust the position by 2x the correct amount
- Fixed playback issues when seeking forward/back that could put the player into an error state