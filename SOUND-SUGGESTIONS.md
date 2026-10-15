# Sound Suggestions — Chick & Little's build notes

My own suggested builds for every sound and track in SOUND-NEEDS.md. These are
starting points, not orders — bend them however you like. Everything here is
buildable in the sampler: the 15 recipes, 4 formant voices (Ah/Ee/Oo/Eh), 8
foley starters, and the effects rack (distortion, 8-bit crunch, LFO, echo,
sustain, resonance, reverb).

## UI & feedback

- `ui-tap.wav` — Start from the UI Blip starter, but layer a barely-there 2.4kHz
  tick (triangle, 20ms) on top for tactility. Keep it under 80ms total. The tap
  is the most-heard sound in the game — it should be felt more than noticed. A
  whisper of reverb (10% wet) so it doesn't sound dry against the music.
- `ui-confirm.wav` — Two-note chime, sine 660→990Hz (a perfect fifth — friendlier
  than the octave). Soften the attack, 180ms. My take: bloom the second note
  with the Airy pad recipe at low volume. Confirmations should feel like a small
  exhale.
- `ui-back.wav` — Reverse the confirm: 520→340Hz, but woodier. Triangle wave, no
  reverb, 100ms. Backing out should sound smaller than going forward.
- `coin-collect.wav` — The classic two-ping (B5→E6), voiced with the Bright Pluck
  recipe plus the Sparkle starter layered at -12dB for shimmer. Bit of sustain so
  it rings ~300ms. This is the game's "money" sound — make it glitter.
- `coin-payout-shower.wav` — 8 ascending pings, but accelerate them (rhythmic
  accelerando) and drift the pan slightly left to right. End on a high E7 ping
  with a reverb tail. Jackpot energy.
- `minigame-win.wav` — C–E–G on the Retro Lead (square), then a fourth "answer"
  note an octave up with echo on it. The echo makes 3 notes feel like 6.
- `minigame-lose.wav` — Descending A–F–D on Nylon Pluck, slow attack, bone dry
  (no reverb — dryness reads as flat disappointment). Detune the last note -8
  cents for a slightly deflated feel.
- `countdown-beep.wav` — Square 880Hz is fine, but run it through the 8-bit
  crunch at ~30% for a gamey edge. Bitcrush reads "game starting" instantly.
- `countdown-go.wav` — Riser starter (600ms — long enough to anticipate, short
  enough to stay snappy) into a C-major chord stab: Saw Bass + Soft Lead stacked,
  with a noise pop at the hit.
- `achievement-unlock.wav` — Magic Sparkle starter plus a slow Cmaj9 arpeggio on
  the Choir Pad voice, long reverb tail (~2s). Achievements are rare — let it
  linger.
- `dialogue-blip.wav` — Square 700–900Hz randomized per blip, 35ms. My take: put
  the Ee formant under it at low volume — that gives NPCs a "voice" quality
  instead of a pure beep. (Different base pitch per NPC would be lovely —
  Gideon lower, Lyla higher — but that's game-side.)
- `error.wav` — Low square 150Hz + distortion at 60%, 250ms, with a downward
  pitch slide at the end. Errors should sound like a gentle "nope," not an alarm.

## Character emotes

Build these from the formant voices so they read as vocal, not beepy.

- `emote-laugh.wav` — "ha-ha-ha" triplet on the Ah formant, descending pitch,
  last syllable trailing off. Slight distortion (15%) for chestiness. I'd do 4
  syllables, not 3 — the 4th sells it.
- `emote-grunt.wav` — Eh formant, 110Hz, 120ms, distortion 25%. Short and
  guttural, like lifting something heavy.
- `emote-confusion.wav` — Oo formant "huh?" with a slow pitch LFO (±40 cents at
  4Hz). The wobble IS the confusion.
- `emote-question.wav` — Ee formant gliding 280→520Hz over 250ms. End the glide
  slightly sharp — questions lift at the end.
- `emote-excitement.wav` — Ah "yip!" — fast attack, pitch jump 500→900Hz in
  120ms. Double it: two yips, second one higher.
- `emote-cheerful.wav` — Bouncy "hey!", Ah→Ee over 300ms, little vibrato on the
  tail. Sunny.
- `emote-talking.wav` — 1.2s loop of soft formant babble: sequence random
  Ah/Eh/Oo blips at low volume in a talking cadence (short bursts, pauses).
  Crossfade the loop ends or the seam will click.
- `emote-mumbling.wav` — Oo formant, lowpassed at 400Hz, mumbling rhythm. Like
  talking through a door — deliberately unintelligible.
- `emote-gasp.wav` — Highpassed noise burst, 180ms, with a fast pitch-rising
  sine underneath (300→900Hz). That rising sine is the "sharp inhale" shape.
- `emote-sigh.wav` — Filtered noise sweeping 800→200Hz over 700ms, plus a soft
  Oo "ahh" underneath. The exhale should feel like relief.

## Cat vocals

Triangle/sine core with pitch envelopes and Ee/Ah formants. Hiss, growl, and
yowl are reserved for genuine threat or distress — ordinary companion moments
use the quieter ones.

- `cat-meow.wav` — Sine 550→850→450Hz, Ee→Ah morph, 450ms. My take: add a tiny
  vibrato in the middle of the glide — real cats wobble.
- `cat-question.wav` — Rising "mrrp?", 200ms, pitch kicking up at the very end.
  Shorter and brighter than the meow.
- `cat-purr.wav` — 22Hz AM on a 90Hz triangle, 2s seamless loop. Layer a soft
  noise rumble at -18dB for chest. This loops under petting — keep it hypnotic,
  not annoying.
- `cat-hiss.wav` — White noise, highpass 3kHz, 450ms, with a fast amplitude
  "spit" at the start. Threat only.
- `cat-trill.wav` — Meow tone with 9Hz pitch LFO at ±150 cents. The warble is
  the whole sound.
- `cat-chatter.wav` — 40ms AM bursts at 12Hz for 350ms, centered ~1.5kHz. That
  teeth-chatter stutter cats do at birds.
- `cat-growl.wav` — Sawtooth 75Hz + distortion 50% + 30Hz AM. Low, menacing.
  Threat only.
- `cat-yowl.wav` — Sine 400→700→350Hz over 1.2s, Ee formant, slight distortion
  for edge. Distress only — make it ache.

## Minigame, movement & ambience

- `minigame-whistle.wav` — Square 2100Hz with 6Hz tremolo, 700ms, two blasts
  (short-long). Pea-whistle rattle: touch of bitcrush.
- `minigame-stopwatch.wav` — 3 clicks: filtered noise ticks at 200ms intervals,
  each slightly brighter than the last. Mechanical, dry, zero reverb.
- `minigame-alarm.wav` — Two-tone square 660/520Hz alternating 4 times, 1.2s.
  Urgent but not harsh — keep distortion off.
- `minigame-siren.wav` — Sine sweep 600→1200→600Hz over 2s, triangle body.
  Build last — it's for a future event, not ordinary play.
- `ambience-rain.wav` — v2, less constant: noise bed (lowpass 1.8kHz + highpass
  400Hz) with deep slow amplitude wander (integer-cycle LFOs so the 3s loop joins
  cleanly), only 4 sparse drip plinks, 2 brief patter bursts of tiny ticks.
  Breathing, not a flat bed — and still quiet.
- `movement-snow-crunch.wav` — 3 staggered noise crunches per step, bandpass
  ~800Hz, 120ms each. Crunch = short noise burst with fast decay + a tiny low
  thump under it.
- `ambience-fire.wav` — Low rumble bed + 8–12 random crackle pops over 3s
  (varying pitch 1–3kHz), 3s seamless loop. Cozy, not campfire-loud.
- `minigame-impact.wav` — Sine drop 160→45Hz, 250ms, noise click at the
  transient. Start from the Impact starter, add distortion 20% for weight.
- `minigame-ball-whoosh.wav` — Bandpass noise sweep 400→3kHz over 300ms. From
  the Whoosh starter — I'd add a slight pitch fall at the very end, a touch of
  Doppler.
- `minigame-ball-catch.wav` — Muted pop: sine 300Hz with very fast decay (60ms)
  + soft noise. Like catching with a mitt.
- `minigame-paint-splatter.wav` — Noise burst lowpassed at 1kHz + a "blub" (sine
  200→90Hz, 150ms). Wetness: 2–3 tiny droplet plinks trailing after.
- `minigame-buzzer.wav` — Square 130Hz + distortion 70%, 600ms, 55Hz sub
  underneath. Game-show wrong-answer energy.

## Thunder (new — for the Thunderstorm weather hook)

The game fires lightning strikes during Thunderstorm weather (with a cooldown
between strikes), so these have a live hook waiting. Vary which one plays per
strike — distant rumbles for far strikes, the crack for close ones.

- `thunder-distant.wav` — 3.5s. Lowpassed noise (120Hz) swelling in soft over
  ~1s, sub sine at 42Hz riding the same swell, plus a second smaller swell a
  second later for the "rolling" feel. No sharp attack at all — distance rounds
  everything off. Keep it deep and patient.
- `thunder-close.wav` — 2.0s. Opens with a bright crack: highpassed noise burst
  decaying in ~50ms, then the body rolls out — lowpassed noise decaying over
  ~0.7s with a sub thump gliding 70→35Hz underneath. The crack-then-rumble shape
  is the whole trick.
- `thunder-roll.wav` — 5.5s. Long rumble with 3-4 slow amplitude swells
  (raised-cosine bumps, seeded random) over a gently decaying bed, sub sine at
  40Hz following the same swells, tail faded to zero. For when the storm lingers.

## Area music tracks

All six are new — the game is being wired to switch to them by area. Build each
as a clean 12-bar loop like the core tracks (trimmed silence, joins cleanly).

- `pond.wav` — 70 BPM, sparse. Nylon Pluck melody over a Warm Pad bed, with
  occasional "water" droplet plinks (sine 2.5kHz, long reverb) as texture. Leave
  lots of air — the pond is a breather spot, fished with Bobby Gill nearby.
- `garden.wav` — 90 BPM, sunny. Bright Pluck lead + a soft shaker-ish hat pattern
  from the sequencer under Airy Pad chords. I'd run a I–V–vi–IV progression —
  the happiest four chords — with a sparse two-note "bird call" motif on the
  Soft Lead.
- `footbridge.wav` — 60 BPM, night. Choir Pad (Ah) chords + a sparse Buzz Lead
  melody drowned in reverb. Moonlight = space + shimmer: scatter the Sparkle
  recipe as rare accents. Minor key, but lift it hopeful in the last 4 bars.
- `cat-shelter.wav` — 100 BPM, warm. Triangle-wave lullaby feel: Soft Lead
  melody over Warm Pad, gentle throughout. Easter egg idea: bury a soft purr
  (25Hz AM texture) at -20dB. Playful middle section with pizzicato-ish plucks.
- `bank.wav` — 110 BPM, polished. This is Mr. Buck Coinsworth's place — I'd go
  slightly pompous: staccato brass-ish stabs (Saw Bass + Retro Lead stack),
  walking bassline, crisp hats, a little swing. Pompous but toe-tapping.
- `festival.wav` — 128 BPM, celebratory. Highest energy of the area tracks: Saw
  Bass driving, Bright Pluck melody, full 6-row sequencer arrangement,
  handclap-ish noise hits on 2 & 4. Build it in the 32-step sequencer for a
  longer phrase, with a drum fill or key change every 8 bars to keep it festive.
