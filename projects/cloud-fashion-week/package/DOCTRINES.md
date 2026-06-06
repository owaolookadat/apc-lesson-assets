# 13 Doctrines from the Cloud Fashion Week Build

> Lessons we learned by burning credits so you don't have to.
> Read these before you start. Save yourself the iterations.

---

## 1. Multi-sheet identity-lock doctrine

**Rule:** For every reel with a recurring subject + material + venue, generate THREE sheets BEFORE any beat stills:
- **F-Sheet** (Character / Face) — 5-view turnaround of your subject
- **E-Sheet** (Environment / Venue) — same venue from multiple camera angles
- **M-Sheet** (Material) — your impossible material studied in isolation

**Why it matters:** Beat stills generated WITHOUT identity-lock references will drift across beats. Your model will have different freckles in B1 vs B4. Your venue will have different equipment count in B2 vs B6. Sheets prevent this.

**The cost of skipping:** Each beat still drifts → reel reads as "different person/place each cut" → viewer registers as fake.

---

## 2. Heterochromia / specific-feature explicit override

**Rule:** Even when you attach a reference image, the AI defaults to symmetric / standard features. Explicit override required.

**Example failure:** Reference shows heterochromia → AI generates matching eye colors anyway.
**Fix:** Add an OVERRIDE clause to the prompt: "LEFT eye PALE VIOLET, RIGHT eye ICE BLUE. Both visible. Both different. If matching, gen FAILED."

**Other features that need overrides:**
- Asymmetric facial features
- Specific hair partings
- Distinctive skin marks / scars
- Atypical body proportions

---

## 3. Chiaroscuro as defining-feature spec

**Rule:** For atmospheric materials (cloud, smoke, fog), the LIGHT-TO-SHADOW GRADIENT is the defining realism marker. Without explicit instruction, AI generates uniformly bright/flat material that reads as cotton wool.

**Required spec language:**
- "BRIGHT cream/white HIGHLIGHTS on the upper surface (top-lit)"
- "MID-TONE soft grey-white in the middle volume"
- "COOL BLUE-GREY SHADOWS on the underside"
- "If uniformly white / no shadow gradient, the gen has FAILED"

---

## 4. Wide ≠ tube-top (atmospheric garment proportions)

**Rule:** When the impossibility is a material on a body, explicitly specify proportions OR the AI will compress it to a clothing silhouette.

**Bad prompt:** "She is wearing a cloud."
**Good prompt:** "She is INSIDE a wide cumulus cloud that extends ~2-3× wider than her body. Head + shoulders protrude above the cloud. Thighs + legs protrude below. Arms are HIDDEN INSIDE the cloud. The cloud has irregular billowing shape, NOT a clean tube silhouette."

The mental model "she's STANDING INSIDE the cloud" produces correctly atmospheric proportions. The mental model "she's wearing a cloud" produces a tube-top dress.

---

## 5. Slow-mo as universal AI-tell concealer

**Rule:** For any atmospheric subject (clouds, smoke, fire, water, fog, fabric), apply slow-mo register universally.

**Why:** Real-world physics for atmospheric phenomena IS slow. AI doesn't have to "invent" dramatic motion. The AI-tells (fast morphing, unnatural billowing, cartoony animation) disappear because the AI is only generating subtle motion.

**Implementation:** Specify in every video prompt:
- "Shot in slow motion (120fps capture, 0.4× playback)"
- "All motion is SLOW and atmospheric"
- "NO fast morphing, NO rapid changes"

---

## 6. Reference-per-shot doctrine (not global)

**Rule:** Match references to what's in the frame. Attaching irrelevant references muddies generation.

| Beat type | Attach |
|---|---|
| Eye macro / face close-up | F-Sheet only |
| Material macro / no subject | M-Sheet only |
| Mid-shot of subject | F-Sheet + M-Sheet |
| Wide of subject in venue | F-Sheet + M-Sheet + E-Sheet |

**The cost of skipping:** Attaching all references to all gens = competing inputs = drift increases.

---

## 7. IG Reels openers must hook in 0.5 sec

**Rule:** TV-ad slow-build opens lose IG viewers in 0.3 seconds. Front-load the impossibility / face / contrast in frame 1.

**Bad opener:** Empty runway (anticipation) → smoke column emerges → walks forward.
**Good opener:** Frame 1 already shows the impossibility in full (model + cloud + studio context).

Internal pacing can still be slow-mo / luxury, but THE OPENING FRAME must carry the hook by itself.

---

## 8. Camera-move variety serves narrative

**Rule:** No two consecutive beats use the same camera move. Repeated moves feel monotone.

**Recommended 6-beat arc:** arc → side-track → push-in → static → drift → pull-back

Each move serves a purpose:
- **Arc** = shows 3D dimensionality
- **Side-track** = kinetic energy
- **Push-in** = intimacy
- **Static** = peak / contemplation
- **Drift** = texture / atmosphere
- **Pull-back** = scale reveal

---

## 9. Blink doctrine — when and when not

**Rule:** AI faces in 5-sec clips at normal framing need a blink to avoid waxwork tell. BUT in slow-mo macro register, totally-still eyes are MORE arresting.

| Face size in frame | Blink? | Reason |
|---|---|---|
| > 30% (head-and-shoulders or larger) | **YES** | Body framing + no blink = uncanny |
| < 30% (full body or smaller) | Optional | Other motion carries naturalism |
| Macro / eyes-only | **NO** | Slow-mo stillness reads as power. Blink risks the colors. |

---

## 10. Twist endings outperform reveal endings

**Rule:** A "brand wordmark fades in" ending is fine. A "pull back through the laptop screen to reveal the creator at a desk" ending is unforgettable.

**Pattern:** Whatever your reel SHOWS, end with a reveal that EXPLAINS the impossibility was achievable.

**Composite technique:** Generate the impossible content + film/AI the real-world container + comp them together in CapCut (screen-tracker). This is far more achievable than asking AI to generate the full nested reveal in one shot.

---

## 11. Cloud-as-atmosphere doctrine (the B2 walking lesson)

**Rule:** AI animates body-mounted volumes as fabric. If you have a walking shot with a cloud/smoke/atmosphere as the "garment," the AI WILL apply clothing physics (bouncing, branching, springy) no matter how you prompt.

**Three workarounds:**

**A) Drop the body motion entirely.** Model stands still + camera moves. Atmospheric drift only.

**B) End-frame trick.** Provide START frame + END frame to Kling, both with cloud in the same position. Cloud will hold but camera motion will also lock (trade-off).

**C) Composite in post.** Generate model walking WITHOUT cloud → generate cloud separately → comp them in CapCut/After Effects. Most reliable but most work.

**My recommendation:** Pick A first. Camera motion + still subject + atmospheric cloud drift = clean physics every time.

---

## 12. End-frame trick — pros and cons

**Use Kling's end-frame slot when:**
- You need to LOCK identity / cloud stability across a clip
- The camera is also static
- You can generate a complementary END still showing the desired final state

**Don't use end-frame when:**
- You want camera movement (it locks)
- The end state is too similar to start (creates oscillating motion)
- You can't generate a clean end frame in 1-2 tries (cost spirals)

---

## 13. VO defensibility check

**Rule:** Your final VO line must SURVIVE scrutiny. Test it against: "Could a real shop with a $500K budget pull this off?"

**Failed example:** "Studio shoots no studio could shoot." Cost: a real studio COULD shoot something like this. The claim breaks under inspection.

**Defensible alternatives:**
- Cost-based: "Studio shoots no studio could afford."
- Time-based: "Studio shoots in an afternoon."
- Method-based: "Studio quality without the studio."
- Direct: "Studio shoots, no studio."

The defensible version is BETTER because it implicitly pitches the value proposition.

---

## Bonus: iteration cost discipline

We burned 5 generations on B4 (eye macro) and 5 on B2 (walking) before pivoting. **Lesson:** if 3 attempts don't land, the approach is wrong, not the prompt.

When to pivot:
- 3 attempts at the same shot still fail → the shot concept needs to change
- A specific feature won't lock in (e.g. opposite-leg position) → accept "close enough" or drop the requirement
- AI fights you on a specific physics → work WITH AI's training data, not against it

---

— Cloud Fashion Week Recipe Kit · Doctrines · AI Production Club Track C
