# Sound & Music Needs — Selfie Social Society

Every filename below is a canonical SFX slot from the game's own audio guide
(`Kmberry1989/selsocsoc` → `assets/audio/README.md`). A file dropped in the
game's `assets/audio/sfx/` folder takes priority over the procedural Web Audio
version with the same ID. WAV is safest. Lowercase, hyphens, no spaces.

The game's 6 music tracks (title-screen, home, plaza, shops, minigames,
board-game) are DONE — no music needs remain. See "Music (optional ideas)" at
the bottom.

Build briefs name the sampler tools to reach for: waveforms
(sine/square/sawtooth/triangle), the 4 formant voices (Ah/Ee/Oo/Eh), the 8
foley starters, and the effects rack (distortion, 8-bit crunch, LFO, echo,
sustain, resonance, reverb).

## UI & feedback

- `ui-tap.wav` — the default tap. Start from the UI Blip foley starter: short
  sine blip ~1200Hz, 60ms, fast decay.
- `ui-confirm.wav` — warm two-tone rise, sine 660→880Hz, 150ms.
- `ui-back.wav` — soft descending blip, sine 500→350Hz, 120ms.
- `coin-collect.wav` — bright metallic ping. Classic coin: two quick sine pings
  (B5→E6), triangle body, touch of sparkle.
- `coin-payout-shower.wav` — cascading coin arpeggio, ~8 pings rising, ~1s.
- `minigame-win.wav` — happy major-arpeggio fanfare, square lead, 3 notes.
- `minigame-lose.wav` — descending minor phrase, soft triangle, 3 notes down.
- `countdown-beep.wav` — neutral beep, square 880Hz, 150ms.
- `countdown-go.wav` — bigger go-tone: rising sweep into a chord hit. Start
  from the Riser foley starter.
- `achievement-unlock.wav` — shimmering unlock: sparkle + rising arpeggio,
  generous reverb.
- `dialogue-blip.wav` — NPC text blip. Short square blip ~800Hz, 40ms; slight
  pitch variation per blip feels alive.
- `error.wav` — dull buzz. Low square 160Hz with a touch of distortion, 200ms.

## Character emotes

The NPCs have distinct voices — build these from the formant voices (Ah/Ee/Oo/Eh)
so they read as vocal, not beepy.

- `emote-laugh.wav` — "ha-ha-ha" triplet, Ah formant, pitch bobbing.
- `emote-grunt.wav` — short low effort grunt, Eh formant ~120Hz, touch of
  distortion.
- `emote-confusion.wav` — wavering "huh?", Oo formant with pitch LFO wobble.
- `emote-question.wav` — rising "hm?", Ee formant gliding 300→500Hz.
- `emote-excitement.wav` — quick rising yip, Ah formant, fast attack.
- `emote-cheerful.wav` — bouncy two-note "hey!", Ah→Ee.
- `emote-talking.wav` — loopable murmur bed, soft formant babble, 1s seamless loop.
- `emote-mumbling.wav` — low indistinct mumble, Oo formant, lowpassed.
- `emote-gasp.wav` — sharp inhale, noise burst with highpass, 200ms.
- `emote-sigh.wav` — falling exhale, filtered noise sweeping down, 600ms.

## Cat vocals

Adopted cats + Agnes Alley's shelter cats. Triangle/sine core with pitch
envelopes and Ee/Ah formants. Hiss/growl/yowl are reserved for genuine threat
or distress events — ordinary companion moments use the quieter ones.

- `cat-meow.wav` — classic meow: sine glide 600→900→500Hz, Ee→Ah formant, 400ms.
- `cat-question.wav` — rising "mrrp?", short, rising tail.
- `cat-purr.wav` — low rattling purr: 25Hz AM on a low triangle, 1.5s loop.
- `cat-hiss.wav` — white noise burst, highpass, 500ms. (Threat only.)
- `cat-trill.wav` — warbling trill: fast pitch LFO on the meow tone.
- `cat-chatter.wav` — rapid teeth-chatter: fast AM bursts, 300ms.
- `cat-growl.wav` — low growl: distorted low sawtooth 80Hz with AM. (Threat only.)
- `cat-yowl.wav` — long mournful yowl, slow pitch arc. (Distress only.)

## Minigame, movement & ambience

- `minigame-whistle.wav` — referee whistle: square 2200Hz with fast tremolo, 600ms.
- `minigame-stopwatch.wav` — mechanical clicks: 3 short filtered clicks.
- `minigame-alarm.wav` — alarm bells: alternating two-tone square, 1s.
- `minigame-siren.wav` — rising/falling siren sweep. Reserved for a future event —
  not attached to ordinary play, build it last.
- `ambience-rain.wav` — sparse, breathing rain: filtered noise bed with slow
  swells and lulls (never a flat bed), sparse drip plinks, occasional patter
  bursts. 3s seamless loop. Keep it quiet — rain sits under the scene.
- `movement-snow-crunch.wav` — footstep crunch: short noise bursts with a
  crunch envelope.
- `ambience-fire.wav` — cozy crackle loop: random pops over a low rumble, 2s loop.
- `minigame-impact.wav` — thud: low sine drop 150→50Hz + noise click. Start from
  the Impact foley starter.
- `minigame-ball-whoosh.wav` — bandpass noise sweep upward. Start from the
  Whoosh foley starter.
- `minigame-ball-catch.wav` — soft catch thump: muted pop.
- `minigame-paint-splatter.wav` — wet splat: noise burst + low blub.
- `minigame-buzzer.wav` — game-show buzzer: harsh square 140Hz + distortion, 500ms.

Thunder (new slots for the rain weather system — the game already fires lightning
during Thunderstorm weather, so these have a live hook waiting):
- `thunder-distant.wav` — low rolling rumble, 3-4s, soft attack. Distant storm.
- `thunder-close.wav` — sharp crack transient then rolling decay, ~2s. Near strike.
- `thunder-roll.wav` — long rolling thunder, 5-6s, slow swells. Lingering storm.

## Legacy aliases (no new builds needed)

These old IDs still work as aliases — they map onto the sounds above, so don't
build separate files for them: `ui-click`, `ui-select`, `coin-pickup`, `win`,
`ready`, `game-start`, `shop-buy`, `dice-roll`, `bot-turn`, `camera`, `select`.
`footsteps.wav` is also supported and optional — start from the Footstep foley
starter if you want walking to make noise.

## Music

The 6 core scene tracks are DONE and live: `title-screen`, `home`, `plaza`,
`shops`, `minigames`, `board-game`.

### Area tracks (new — game will switch to these by area)

The game is being wired to switch music when the player enters these areas
(anything else keeps the current 6). Build each as a clean loop, like the core
tracks. Filenames (in `assets/audio/music/`):

- `pond.wav` — the fishing pond (Bobby Gill). Lazy water, soft plucks, unhurried.
- `garden.wav` — Fern's garden. Sunny, earthy, gentle momentum.
- `footbridge.wav` — the Moonlight Footbridge. Night air, a little magical,
  sparser arrangement.
- `cat-shelter.wav` — Agnes Alley's shelter. Warm, gentle, playful.
- `bank.wav` — Mr. Buck Coinsworth's bank. Polished, a bit pompous, steady.
- `festival.wav` — the rotating festival grounds (Pip Parade). Upbeat,
  celebratory, higher energy than plaza.

### Optional ideas only
