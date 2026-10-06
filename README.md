# Audio Sampler — Selfie Social Society

Hear every procedural sound effect in Selfie Social Society by selecting its
intended replacement file name — whether or not a replacement file exists yet.

## What it does
- All 30 procedural SFX slots: 10 player emotes, 9 game SFX, 2 ambience,
  1 movement, 8 cat sounds
- Each card shows the intended replacement path (`assets/audio/sfx/<fileId>.mp3`;
  .ogg/.wav/.m4a also accepted)
- "Play procedural" triggers the game's real Web Audio synthesis engine
  (extracted verbatim from `assets/snug-audio.js`)
- Upload your own recording per slot to A/B it against the procedural original
- Global volume control

## Run it
Open `index.html` in a browser — it's fully self-contained.

## Notes
- Game repo: `Kmberry1989/selsocsoc` (the game itself; this tool is separate)
- No replacement audio files exist in the game yet — every slot is procedural-only
- Replacement files belong in the game's `assets/audio/sfx/` folder
