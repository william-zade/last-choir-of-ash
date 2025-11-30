# Production Notes – The Last Choir of Ash

Working document for how this album should *sound*:
tones, routing, mix philosophy, and repeatable decisions.

---

## 1. Global Session Setup (Reaper)

**DAW:** Reaper on Pop!_OS  
**Interface:** PreSonus AudioBox iTwo  
**Tuning:** Drop A (guitar & bass)  
**Tempo baseline:** ~90 BPM

### 1.1 Project defaults

- **Sample rate:** 48 kHz
- **Bit depth (recording):** 24-bit
- **Master headroom target:**
  - Peaks around -6 dBFS before any limiting.
  - No mixbus limiter while writing; add gentle limiter only near the end.

### 1.2 Basic bus layout

Create and color-code these buses in every project:

- **DRUMS BUS**
- **BASS BUS**
- **GTR RHYTHM BUS**
- **GTR LEAD / MELODIC BUS**
- **VOCALS BUS**
- **FX / AMBIENCE BUS** (pads, bells, sonar, whooshes, etc.)
- **ORCHESTRATION BUS** (strings, woodwinds, etc. when used)
- **MASTER** (2-bus)

Route all individual tracks into these buses, then into the master.  
Global processing (glue, EQ sculpting) happens mostly on the buses, not on the master.

### 1.3 File & track naming

- Project name: `LC0A-<track-number>-<short-title>.RPP`  
  e.g., `LC0A-03-AshesInOrbit.RPP`
- Stems/renders (if exported at all):  
  `renders/LC0A-03-AshesInOrbit-<stem>-v01.wav`

Keep the Git repo text-only; renders & stems live outside or are gitignored.

---

## 2. Guitars

### 2.1 Role & vibe

- Foundation of the doom weight.
- Should sound **big, slow, intentional**, not busy.
- Think: blend of **Orange-ish** saturation + a tighter, more modern head for definition.

### 2.2 Tracking approach

- **Rhythm layers:**
  - Standard: 2 main rhythm tracks (L/R).
  - For extra width: optional 3rd/4th layer tucked lower in level.
- **Playing:**
  - Locked to drums and bass; no flamming chugs.
  - Let chords ring; avoid over-choking everything.

### 2.3 Tone guidelines

- High gain, but not fizzy.
- Low end: tight enough to leave room for bass and kick.
- Highs: controlled, no harsh 3–7 kHz spikes.
- Use cab/IR choices that lean toward:
  - Doom/stoner speakers (V30 + Greenback flavors, or equivalents)
  - Slight mid-forward presence so riffs translate at low volume.

**FX:**

- Reverb and delay mostly on **FX sends**, not baked into the track.
- Lead / melodic lines can have more obvious space (longer verb, slight modulation).

---

## 3. Bass

### 3.1 Role

- Carries the low-end **weight** and groove.
- Should be clearly audible as its own part, not just a blur under guitars.

### 3.2 Tone

- Base tone: rounded low end with mild grit.
- Enough midrange to hear note movement in doom tempos.
- Avoid ultra-scooped sounds; mids are your friend here.

### 3.3 Interaction with kick

- Use sidechain compression or dynamic EQ to duck bass **3–4 dB on kick hits**, fast attack, medium release.
- Goal: keep the kick audible without losing the sense of a single unified low-end.

---

## 4. Drums

### 4.1 Current tools

- **Kits:** DrumGizmo
  - Using **Muljord** as a working kit.
  - Plan to test **Crocell** when it’s behaving.
- Aim for: solid doom/stoner tone, clear kick and snare, natural but punchy.

### 4.2 General approach

- Kick:
  - Low-end body that works with bass.
  - Enough click/attack to be heard in dense riffs.
- Snare:
  - Darker side, not super modern bright.
  - Reverb tails can be long in some sections (especially on *The Throne of Silence*).
- Toms:
  - Used sparingly for emphasis; not constant fills.

### 4.3 Room & overheads

- Overheads capture cymbal character; avoid harshness.
- Room can be pushed in big sections to feel like you’re in a large hall or decaying space.

---

## 5. Ambience, FX & Orchestration

These are critical to the “doomed civilization at the end of time” feel.

### 5.1 Core ambience palette

- **Wind** – subtle noise floors, long fades between movements.
- **Church bells** – mark transitions, warnings, or ritual moments.
- **Sonar pings** – especially on space-facing tracks like *Ashes in Orbit*.
- **Orbital whooshes / debris passes** – panning elements that move slowly across the stereo field.

All of these should live on dedicated tracks routed to **FX / AMBIENCE BUS**.

### 5.2 Orchestration

- Strings & woodwinds to:
  - Double main chord progressions in big sections.
  - Answer or support vocal/guitar melodies.
- Keep them **supporting**, not dominating.
- Use them to:
  - Add tension before drops.
  - Elevate climactic choruses or final refrains.

---

## 6. Mix Philosophy

### 6.1 Overall sound

- Heavy, thick, **but intelligible**.
- Slow tempos mean any mud or harshness is extra noticeable—clean the midrange.
- Lows: controlled; no endless 50 Hz rumble that kills headroom.

### 6.2 Rough loudness & balance

- Aim for mixes that are listenable with or without heavy limiting.
- Pre-master:
  - Peaks around -6 dBFS.
  - RMS/LUFS not crushed; plenty of movement.

### 6.3 Space & depth

- Use:
  - Shorter reverbs for drums/bass/guitars when you need clarity.
  - Long plate/hall verbs for bells, vocals, and some leads.
- Automate reverb send levels:
  - More verb in sparse moments.
  - Less verb when everything is pounding.

---

## 7. Cross-Track Consistency

Some things should be relatively consistent across the whole record:

- Drum kit and basic drum tone.
- Bass core tone (minor tweaks per song).
- Guitar IR/speaker choices, even if amp tones vary slightly.
- Reverb “flavor” for the main spaces.

The listener should feel like they’re in the **same universe** the whole time.

---

## 8. Per-Song Production To-Do (High-Level)

### 8.1 Echoes from the Dying Star

- [ ] Establish baseline drum and bass sound for the album.
- [ ] Design main guitar tone pair (Orange-ish + tighter head).
- [ ] Build first pass of global Reaper template from this session.

### 8.2 The Throne of Silence

- [ ] Push reverb & space to the forefront.
- [ ] Experiment with bell patterns as structural markers.
- [ ] Test more orchestration layers (strings/choir pads).

### 8.3 Ashes in Orbit

- [ ] Implement sonar pings and orbital movement FX.
- [ ] Explore A minor ↔ A Lydian contrast in leads.
- [ ] Focus on “weightless grief” feel: heavy but floating.

### 8.4 We Lit the Fire for No One

- [ ] Pull mix in closer, more intimate; less huge space, more room.
- [ ] Vocal clarity and emotional delivery prioritized over sheer weight.
- [ ] Use dynamics and automation to make the last third of the song hit hardest.

---

## 9. Open Questions / Future Experiments

- [ ] Exact IR/cab combos for rhythm vs lead.
- [ ] Whether to use a consistent drum room on all tracks or vary per song.
- [ ] Use of subtle tape/saturation on the mix bus.
- [ ] Cross-cultural percussion / instrumentation that feels authentic and integrated.
