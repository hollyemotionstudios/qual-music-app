# Music app prop

Mock music-streaming web app for film (qual 6138, Antonelli). Unbranded. Pick the song (Funiculì, Funiculà) from the library, see the now-playing screen with album art and title, then open synced lyrics. There's no audio: a timer drives the playback. The song is public domain (Denza / Turco, 1880); the album art is original to the prop. Lyric timings are estimates until the production's recording is known.

Primary size: Galaxy Z Fold 8 cover screen in portrait, 416×658 CSS px (assumed 3× scaling, unverified on device). Larger screens still work. Single static file: `index.html`. Pushes to `main` redeploy on Vercel.

## On set
- **Space** play/pause · **← / →** seek 5s · **L** lyrics · **Esc** back · **R** reset to library · **F** fullscreen
- Tap a lyric line to jump to it. The cursor hides after 2.5s without movement.
- Deep link straight to a shot: `?song=funiculi-funicula&view=lyrics&t=47&play=0`

Edit the song and lyric timing in the `SONGS` array at the top of the script.
