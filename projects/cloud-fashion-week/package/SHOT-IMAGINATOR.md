# Shot Imaginator — 10-Field Prompt Scaffold

> Write any AI image-generation prompt by filling 10 fields.
> No more "I don't know what to put in my prompt."

---

## The framework

Every great gen-AI prompt covers 10 dimensions. Skip a field and the AI fills in a default that probably isn't what you wanted. Fill all 10 and you control the output.

| # | Field | What it does |
|---|---|---|
| 1 | SHOT INTENT | Tells the AI WHY this shot exists narratively |
| 2 | SUBJECT | Who/what is in frame, including specific identity |
| 3 | SCENE CONTEXT | Where the shot happens, atmospheric setup |
| 4 | CAMERA | Lens, position, angle, sensor aesthetic |
| 5 | FRAMING | Composition, rule of thirds, model size in frame |
| 6 | DEPTH | Foreground / midground / background plan |
| 7 | LIGHTING | Sources, direction, color temp, key/fill/rim |
| 8 | SUBJECT PHYSICS | What subject does + what it doesn't do |
| 9 | COLOR GRADE | Register, mood, tonal range |
| 10 | ANTI-KEYWORDS + SELF-CHECKS | What to avoid + critical pass/fail checks |

---

## The blank scaffold (copy this)

Paste this into your notes and fill in each field for any shot you need to prompt.

```
[Shot ID + brief description] — [shot purpose, e.g. "OPENING HOOK FRAME for [project name]"]

SHOT INTENT:
[Why does this shot exist? What does it deliver to the viewer?]

SUBJECT:
[Who/what is in frame. Identity markers if person. Material/state if object.]

SCENE CONTEXT:
[Where the shot takes place. Atmospheric setup. Time-of-day if outdoor. Equipment density if indoor.]

CAMERA:
[Camera model + lens + f-stop + position + angle. Phase One IQ4 / Hasselblad / Leica for premium register.]

FRAMING:
[Aspect ratio. Composition rules. Model size as % of frame. Where head sits vertically. What surrounds.]

DEPTH:
[Foreground, midground, background plan. What's in focus vs bokeh.]

LIGHTING:
[Light sources by name. Direction. Color temperature. Key / fill / rim breakdown. Atmospheric haze.]

SUBJECT PHYSICS:
[For static subjects: pose, weight distribution. For motion: what motion is allowed.
For materials: what behavior the material has + what it DOESN'T have.]

COLOR GRADE:
[Register name (Tim Walker / Vogue / cinematic / commercial). Mood. Tonal range.]

ANTI-KEYWORDS:
- NO [common failure mode 1]
- NO [common failure mode 2]
- NO real brand wordmarks
- NO uncanny valley, NO CGI, NO illustration

SELF-CHECKS:
1. [Specific check that must pass]
2. [Specific check that must pass]
3. [Specific check that must pass]

If any check fails → gen failed → regenerate.
```

---

## Worked example — Cloud Fashion Week B3 (push-in hero)

Here's the same scaffold filled in for our actual B3 prompt. Compare to the [final B3 still](../stills/b3.jpeg).

```
B3 still — PUSH-IN HERO SHOT for "Cloud Fashion Week" IG Reel.

SHOT INTENT:
This still captures the END POINT of a slow push-in camera move. Head-and-shoulders close-up at slight low-diagonal angle. Intimate and arresting. The heterochromia payoff moment.

SUBJECT:
Female fashion model with albinism. Pale milky-white skin, platinum-white long hair, freckles on nose bridge and cheekbones, heterochromic eyes (LEFT pale violet, RIGHT ice-blue).

SCENE CONTEXT:
Film production studio. Background is soft-focus depth — unattended cinema cameras + lighting grid hint, dramatic spotlight cone creating soft halo behind hair, atmospheric haze gives the bokeh a glowing quality.

CAMERA:
Phase One IQ4, 85mm f/2.8 (or 100mm f/2.8 for more compression). Low-diagonal angle, slightly below eye level, angled up toward face at 10-15 degrees.

FRAMING:
Vertical 9:16. Head-and-shoulders close-up. Model fills upper 70% of frame. 3/4 face angle (rotated 15-30° from frontal). Top wispy edge of cloud visible at bottom 30%.

DEPTH:
Foreground: model's face + collarbone area (sharp).
Midground: cloud's top edge (slight focus falloff).
Background: studio context (soft bokeh — cameras, grid, spotlight halo).

LIGHTING:
Soft directional key from camera-front-left (5400K). Side fill from camera-right preventing flat shadows. Back rim from dramatic spotlight cone (warm gold #C8A24B) giving hair separation from dark background. Skin reads true pale milky with subtle warm pickup on rim-light side.

SUBJECT PHYSICS:
Calm, confident, eyes locked to camera. Slight head tilt (≤5°). Natural micro-expression — not posed/rigid. No motion (this is a still — natural breath only).

COLOR GRADE:
Cinematic editorial portrait — Vogue cover register. Phase One IQ4 medium-format aesthetic. Warm rim on hair, cool fill on face-front. Pale milky skin tones true.

ANTI-KEYWORDS:
- NO full-frontal pose — must be 3/4 angle
- NO clean background — must have soft-focus depth
- NO airbrushed porcelain skin — freckles + texture VISIBLE and SHARP
- NO drawn-on / painted eyebrows
- NO flat eye color — iris striations required
- NO matching eye colors — heterochromia is the entire point
- NO real brand wordmarks
- NO uncanny valley, NO CGI, NO illustration

SELF-CHECKS:
1. Heterochromia clearly visible (left violet, right ice-blue)?
2. Freckles SHARPLY rendered on nose bridge + cheekbones?
3. 3/4 angle on face (NOT full-frontal)?
4. Soft-focus background with spotlight halo?
5. Back-rim warm light on hair from spotlight cone?
6. Pore texture visible on skin?
7. Iris striations + asymmetric catchlights visible?

If any answer is no, generation failed.
```

---

## Quick-fill mode — common shot types

For common shot types, here are the 10 fields pre-filled with sensible defaults. Adapt your specifics.

### Macro / hero close-up

```
SHOT INTENT: Hyperreal luxury-ad macro — the polarizing identity payoff
SUBJECT: [Your subject's defining feature]
SCENE CONTEXT: Clean neutral background OR soft-focus environmental hint
CAMERA: Phase One IQ4, 100mm macro f/4.0, eye level
FRAMING: Vertical 9:16 OR 1:1. Tight crop, [feature] fills 60%+ of frame
DEPTH: Pin-sharp focus on subject, shallow bokeh elsewhere
LIGHTING: Single soft key + subtle fill. 5400K daylight. Natural asymmetric catchlights
SUBJECT PHYSICS: TOTALLY STILL — no motion, no blink
COLOR GRADE: Cartier / Chanel / Tiffany macro register
ANTI-KEYWORDS: NO soft AI haze, NO compression mush, NO flattened tones, NO porcelain skin
SELF-CHECKS: [Feature] crystal clear at this scale? Texture preserved? Pin-sharp focus?
```

### Wide establishing / opening hook

```
SHOT INTENT: Cinematic establishing frame — opening hook for IG Reel
SUBJECT: [Subject + impossibility visible from frame 1]
SCENE CONTEXT: [Venue at full atmospheric register]
CAMERA: Phase One IQ4, 24-35mm wide f/4.0, eye level. Tim Walker / Vogue register
FRAMING: Vertical 9:16. Subject at upper-third (rule of thirds). Subject 35-45% of frame height. Depth behind subject.
DEPTH: Subject is focus plane. Foreground floor leads in. Background recedes into atmospheric depth.
LIGHTING: Multi-source. Overhead key + back rim from atmospheric light source + soft side fill.
SUBJECT PHYSICS: Standing still + slight weight forward (moment in time, not posed)
COLOR GRADE: Cinematic editorial — Tim Walker fashion-film register
ANTI-KEYWORDS: NO center-stamping, NO catalog framing, NO 60%+ subject height, NO clean cut-out look
SELF-CHECKS: Subject NOT center-stamped? Depth behind subject visible? Atmospheric haze present?
```

### Material study / pure subject macro (no person)

```
SHOT INTENT: Material hero shot — atmospheric register for the impossible material
SUBJECT: [Material] in pure form. No body, no face, no venue.
SCENE CONTEXT: Clean neutral mid-grey background (#888888)
CAMERA: Phase One IQ4, 85-100mm f/4.0, eye level
FRAMING: Vertical 9:16. Material fills 85-90% of frame. Negative space at corners.
DEPTH: Pin-sharp focus on material surface. Wispy edges fall into slight bokeh.
LIGHTING: Single dramatic key from above. Soft fill from below. 5400K daylight. Directional chiaroscuro.
SUBJECT PHYSICS: [Material behavior — what it does, what it doesn't do]
COLOR GRADE: Cartier / NASA cloud-photography register. Photographic, atmospheric, NOT animated.
ANTI-KEYWORDS: NO uniformly bright material, NO smooth fog wash, NO mushy edges, NO body parts in frame
SELF-CHECKS: Chiaroscuro visible? Wispy edges sharply resolved? Internal volumetric depth visible?
```

### Profile / side-tracking shot

```
SHOT INTENT: Side-tracking [walking / standing] shot — kinetic camera energy
SUBJECT: [Subject in profile, facing walking/gaze direction]
SCENE CONTEXT: [Venue from perpendicular side angle]
CAMERA: Phase One IQ4, 50-85mm f/2.8, eye level
FRAMING: Vertical 9:16. Subject centered horizontally. Runway/floor runs left-right across frame. Subject 40-50% of frame height.
DEPTH: Subject is focus plane. Far side of venue soft-focused (cameras, equipment).
LIGHTING: Multi-source matching established register. Subject lit by venue's own lighting.
SUBJECT PHYSICS: STILL in profile (if doing camera-only motion) OR mid-stride (if doing end-frame trick — be aware of cloth-physics risks per Doctrine #11)
COLOR GRADE: Match established register from other beats
ANTI-KEYWORDS: NO front-facing turn, NO subject motion that triggers fabric physics, NO unstable identity
SELF-CHECKS: Profile maintained? Side angle clearly readable? Atmospheric integration with venue?
```

---

## Using the Shot Imaginator with video gen (Kling)

The 10-field scaffold also works for video motion prompts. Replace some fields:

| Still field | Video equivalent |
|---|---|
| SUBJECT PHYSICS | SUBJECT MOTION — what the subject does over 5 sec |
| FRAMING | + CAMERA MOVE — what the camera does |
| LIGHTING | LIGHTING CONTINUITY — preserve from source still |
| DEPTH | + MOTION PARALLAX — how depth shifts with camera |

Video scaffold structure:

```
[Beat ID] — [video purpose]

SHOT INTENT:
SOURCE STILL: [link to the still being animated]
SUBJECT MOTION:
CAMERA MOVE:
MATERIAL BEHAVIOR (if applicable):
OTHER MOTION (background, atmosphere):
SLOW-MO REGISTER:
ANTI-MOTIONS (what NOT to animate):
PHOTOGRAPHY REGISTER:
```

See [PROMPTS-LIBRARY.md Section 3](PROMPTS-LIBRARY.md) for working video prompts.

---

## When to use the Shot Imaginator

| Use it when | Skip it when |
|---|---|
| Writing a NEW prompt from scratch | Adapting an existing working prompt (just swap specifics) |
| Adapting a prompt for an unusual shot | Doing a regen on a near-keeper (small tweak only) |
| Teaching someone to prompt | The shot is simple and the prompt is one sentence |
| Reviewing why a gen failed | You're iterating fast and need momentum |

---

## Why this works

Most "bad AI gens" fail because the prompt missed 3-5 of these 10 fields. The AI filled in defaults you didn't want. The Shot Imaginator forces you to address every dimension consciously.

**Two minutes of structured prompt thinking = 4 hours saved in iterations.**

---

— Cloud Fashion Week Recipe Kit · Shot Imaginator · AI Production Club Track C
