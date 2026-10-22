# Music app prop

Mock music-streaming web app for film (qual 6138, Antonelli). Unbranded. Pick a song from the library, see the now-playing screen with album art and title, then open synced lyrics. There's no audio: a timer drives the playback. All song titles, artists, lyrics and album art are original to the prop.

Single static file: `index.html`. Pushes to `main` redeploy on Vercel.

## On set
- **Space** play/pause · **← / →** seek 5s · **L** lyrics · **Esc** back · **R** reset to library · **F** fullscreen
- Tap a lyric line to jump to it. The cursor hides after 2.5s without movement.
- Deep link straight to a shot: `?song=midnight-arcade&view=lyrics&t=40&play=0`
  - Song ids: `paper-lanterns`, `northbound`, `slow-motion-summer`, `midnight-arcade`, `saltwater-letters`, `glasshouse`

Edit songs and lyric timing in the `SONGS` array at the top of the script.
