# Nocturne — personal iPhone music player

This is a personal, Liner-inspired music player starter designed for iPhone Safari.

## Included
- Import audio files from the iPhone Files picker
- Local library storage using IndexedDB
- Search, favorites, playlists, and recently added tracks
- Now Playing screen, playback controls, shuffle and repeat
- Add plain-text or timestamped LRC lyrics
- Add your own cover images
- PWA manifest, service worker, and Home Screen icon

## Install on iPhone
A PWA must be hosted over HTTPS to be installable as a Home Screen web app. The easiest route is to upload this folder to a static HTTPS host such as Netlify or GitHub Pages, then:
1. Open the hosted website in Safari.
2. Tap Share.
3. Choose Add to Home Screen.
4. Enable Open as Web App if the option appears, then tap Add.

You can do the hosting steps from a phone browser, but some hosting providers are easier to use on a computer. Nocturne itself does not require a computer once hosted.

## Importing music
Tap Import music and select audio files in the iOS Files picker. File names formatted like `Artist - Song Title.mp3` are split into artist and title automatically. Other names are used as the title.

## Important iOS notes
- Audio files are stored in this browser's local website storage. Do not clear Safari website data if you want to keep the library.
- Keep original files backed up in Files or another location.
- iOS may evict website storage under device storage pressure; persistent storage is requested implicitly by browser behavior but cannot be guaranteed.
- Background playback behavior depends on iOS/Safari version and device settings. Test with the screen locked.
- This starter does not stream copyrighted music, fetch commercial catalogs, or bypass DRM.
- Lyrics are user-supplied. LRC lines use `[mm:ss.xx]text`.
- Some audio formats may not be supported by iOS Safari. MP3, AAC/M4A, and WAV are generally safer choices than FLAC or OGG.

## Privacy
Nocturne does not send your audio files to a server. The app stores them locally in your browser. Hosting only serves the app files.
