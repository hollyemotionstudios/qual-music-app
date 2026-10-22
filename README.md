# Music app prop

Mock music-streaming web app for film (qual 6138, Antonelli). Unbranded. It opens full screen on the now-playing screen for Funiculì, Funiculà (album art, title, play controls), paused at 0:00; tap play, then open the synced lyrics. The Listen Now library is parked for now: add `?library=1` to the URL to bring it back. There's no audio: a timer drives the playback. The song is public domain (Denza / Turco, 1880); the album art is original to the prop. Lyric timings are estimates until the production's recording is known.

Target sizes: Galaxy Z Fold 8 inner screen held upright, 616×816 CSS px (main), and the folded (cover) screen, 948×1048 (small screen; lyrics use the two-column layout at this width). The inner size assumes 3× scaling and is unverified on device. Larger screens still work. Single static file: `index.html`. Pushes to `main` redeploy on Vercel.

## On set
- **Space** play/pause · **← / →** seek 5s · **L** lyrics · **Esc** back · **R** reset to the start (paused at 0:00) · **F** fullscreen
- Tap a lyric line to jump to it. The cursor hides after 2.5s without movement.
- Deep link straight to a shot: `?song=funiculi-funicula&view=lyrics&t=47&play=0`

Edit the song and lyric timing in the `SONGS` array at the top of the script.
