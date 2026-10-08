# Audio Sampler — Selfie Social Society

Hear every procedural sound effect and music track in Selfie Social Society by
selecting its intended replacement file name — whether or not a replacement
file exists yet.

## What it does
- All 30 procedural SFX slots: 10 player emotes, 9 game SFX, 2 ambience,
  1 movement, 8 cat sounds
- 6 music tracks (board-game, home, minigames, plaza, shops, title-screen) —
  the actual WAV files shipped in the game, in `music/`
- Each SFX card shows the intended replacement path (`assets/audio/sfx/<fileId>.mp3`;
  .ogg/.wav/.m4a also accepted); each music card shows `assets/audio/music/<fileId>.wav`
- "Play procedural" triggers the game's real Web Audio synthesis engine
  (extracted verbatim from `assets/snug-audio.js`); "Play track" plays the
  bundled music WAV
- Upload your own recording per slot to A/B it against the original
- Global volume control

## Run it
Open `index.html` in a browser — it's self-contained apart from the `music/`
folder, which must sit next to `index.html`.

## Notes
- Game repo: `Kmberry1989/selsocsoc` (the game itself; this tool is separate)
- No replacement SFX files exist in the game yet — every SFX slot is procedural-only
- Replacement SFX belong in the game's `assets/audio/sfx/` folder; replacement
  music belongs in `assets/audio/music/`
