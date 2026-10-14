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

## Labs: generate your own
- **Sound Lab** — a small synth (wave, pitch sweep, noise, filter, wobble) with
  one-shot presets (coin, jump, pop, whoosh, click, power-up) and a randomizer
- **Music Lab** — composes 12-bar loop-ready tracks in the game's relaxed cozy
  style; pick a mood (Sunny Meadow, Quiet Evening, Playful), key, tempo, and
  melody density, then draft new melodies
- Both labs play instantly and download real WAV files
- **Sound Recipes** — 15 selectable synth recipes built from sine, square,
  sawtooth, and triangle tones, plus four formant voices (Ah, Ee, Oo, Eh);
  play, download, or save any of them as a new slot
- **Foley FX** — 8 procedural foley starters (footstep, whoosh, pop, splash,
  magic sparkle, UI blip, impact, riser) with instant play + WAV download
- **Loop Sequencer** — 16- or 32-step sequencer with 6 instrument rows
  (kick, snare, hats, bass, chord stab, lead/arp); tap a step to cycle
  off → 4 sound variants, each in its own color. Built-in effects rack
  (distortion, 8-bit crunch, LFO, echo, sustain, resonance, reverb) works
  live during preview and bakes into WAVs. Preview has loop autoplay + stop;
  save the pattern as a new music slot
- **Save as new slot** — give a creation its own filename and purpose (e.g.
  what game moment it belongs to); it lands in **My Creations** with its
  intended game path (`assets/audio/sfx/<name>.mp3` or
  `assets/audio/music/<name>.wav`), and persists across visits
- **Export game music pack** — one click zips every saved music track whose
  filename or purpose names a game scene (title-screen, home, plaza, shops,
  minigames, board-game) into `game-music-pack.zip`; newest track wins per
  scene, anything ambiguous is left out

## Run it
Open `index.html` in a browser — it's self-contained apart from the `music/`
folder, which must sit next to `index.html`.

## Notes
- Game repo: `Kmberry1989/selsocsoc` (the game itself; this tool is separate)
- No replacement SFX files exist in the game yet — every SFX slot is procedural-only
- Replacement SFX belong in the game's `assets/audio/sfx/` folder; replacement
  music belongs in `assets/audio/music/`
