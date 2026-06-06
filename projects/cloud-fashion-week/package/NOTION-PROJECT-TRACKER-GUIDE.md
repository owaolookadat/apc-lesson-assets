# Notion Project Tracker — Build Guide

> Step-by-step instructions to build a Notion dashboard that tracks any AI video reel from concept to ship.
>
> **Why a Notion tracker (vs the markdown Project Sheet):**
> The markdown Project Sheet is a STATIC planning doc.
> The Notion tracker is a LIVING DASHBOARD that shows progress, embeds media, and ties together every artifact across the build.
>
> Use both — markdown sheet for planning, Notion for executing + sharing the build journey publicly.

---

## What you'll build

A Notion page with:
- 📊 Project hero (concept name, status, dates, final reel embed)
- 📋 Concept brief + distribution plan
- 📐 **Sheets Tracker database** (kanban view of F-Sheet, E-Sheet, M-Sheet)
- 🎥 **Beat Tracker database** (table view of B1-B6 with embedded stills + clips)
- 📝 Decision log (timeline of choices)
- 🔁 Iteration history (what was tried, what failed, what worked)
- 💡 Lessons learned (doctrines discovered during build)
- ✅ QC checklist (pre-publish gate)
- 🚀 Distribution log (where posted, engagement metrics)

When done, this is a SINGLE PAGE that shows the entire build journey. You can share it as a public duplicate link — your case-study marketing asset.

---

## Estimated time

- First build: ~45 minutes (read this, build the structure)
- Per project after that: ~10 minutes (duplicate the template, fill in your data)

---

## Build sequence

Follow these steps in order. Each step has the exact Notion blocks to add.

### Step 1 — Create the page

1. In Notion, click "Add a page" in your sidebar
2. Title: `[PROJECT NAME] — Production Tracker` (e.g., "Cloud Fashion Week — Production Tracker")
3. **Cover image:** Click "Add cover" → Upload → use your reel's cover thumbnail
4. **Icon:** Click "Add icon" → Choose emoji 🎬 (or 📽️ / 🎞️ / your project-specific emoji)
5. Add a brief description directly under the title:
   > A 15-second slow-motion IG Reel exploring [your impossibility]. Built in [N] days using AI Production Club Track C workflow.

### Step 2 — Add the project hero block

Below your description, add a callout block (`/callout`):

```
🎬 Status: [In Progress / Shipped / On Hold]
📅 Date locked: [YYYY-MM-DD]
🎯 Format: IG Reel · [N] sec · vertical 9:16
🏷️ Wedge category: [Physics / material / scale / time impossibility]
💰 Production cost: [total spent]
⏰ Production time: [hours/days]
```

Right below, embed your final reel:
- `/video` → Upload your `reel-final.mp4`
OR
- `/embed` → Paste your YouTube/Vimeo URL

### Step 3 — Add Block 1: Concept + Brief

Add a heading 1 (`/h1`): **📋 Block 1 — Concept + Brief**

Add a quote block (`/quote`):
- Paste your one-paragraph concept description

### Step 4 — Add Block 2: Distribution Plan

Add a heading 1: **📢 Block 2 — Distribution Plan**

Add a table (`/table`) with 2 columns:

| Field | Value |
|---|---|
| Hook (first 2 sec) | [Your visual hook description] |
| Caption | [Your IG/TikTok caption] |
| Hashtags | [Comma-separated tags] |
| CTA | [Comment trigger or other call-to-action] |
| DM funnel keyword | [Trigger word] |
| Posting time | [Day + time] |
| Platforms | [IG Reel / TikTok / X / etc.] |

### Step 5 — Build the Sheets Tracker database (most important step)

Add a heading 1: **📐 Block 3 — Sheets Tracker**

Add an inline database (`/database` → "Database — Inline"):
- Name it: **Sheets**

**Configure properties:**
1. **Name** (default — already there) → rename to "Sheet Name"
2. Add property: **Type** (Select)
   - Options: Character (F-Sheet), Environment (E-Sheet), Material (M-Sheet), Identity (custom)
3. Add property: **Status** (Status)
   - Options: TODO, Generating, Approved, Failed/Regen
4. Add property: **Preview** (Files & media)
   - This is where you embed the sheet image
5. Add property: **Used in beats** (Multi-select)
   - Options: B1, B2, B3, B4, B5, B6
6. Add property: **Prompt** (Text) — paste-ready prompt for this sheet
7. Add property: **Reference image** (URL) — where the anchor reference came from

**Set the default view to "Gallery"** so each sheet shows as a card with its preview image.

**Add your sheets as cards:**

For Cloud Fashion Week, create 3 cards:
| Sheet Name | Type | Status | Used in beats |
|---|---|---|---|
| F-Sheet (Model) | Character | Approved | B1, B2, B3, B4, B6 |
| E-Sheet (Studio Venue) | Environment | Approved | B1, B2, B3, B6 |
| M-Sheet (Cloud) | Material | Approved | B1, B2, B3, B5, B6 |

For Polar Luxury, create your sheets similarly.

### Step 6 — Build the Beat Tracker database (the heart of the dashboard)

Add a heading 1: **🎥 Block 4 — Beat Tracker**

Add another inline database (`/database` → "Database — Inline"):
- Name it: **Beats**

**Configure properties:**
1. **Name** → rename to "Beat ID" (e.g., B1, B2, B3...)
2. **Beat title** (Text) — e.g., "Opening hook", "Eye macro", "Pull-back reveal"
3. **Time** (Text) — e.g., "0-3s", "3-6s"
4. **Status** (Status) — TODO, Generating, Approved, Reshoot
5. **Still preview** (Files & media) — embed the locked still
6. **Video preview** (Files & media OR URL) — embed the locked video clip
7. **Camera move** (Select) — Arc, Side-track, Push-in, Static, Drift, Pull-back
8. **Subject motion** (Text) — what the subject does
9. **VO line** (Text) — what's spoken during this beat
10. **References attached** (Multi-select) — F-Sheet, E-Sheet, M-Sheet
11. **Hyperrealism req** (Checkbox) — for macro shots

**Set default view to "Table"** for quick scanning. Add a second view as "Gallery" using "Still preview" as the cover.

**Add your beats as rows:**

For Cloud Fashion Week (5-clip version):
| Beat ID | Beat title | Time | Camera move | Subject motion | VO line |
|---|---|---|---|---|---|
| B1 | Opening hook | 0-3s | Slow arc 90° | Still + slow blink | "There's no model." |
| B3 | Push-in hero | 3-6s | Push-in | Slight gaze + blink | "There's no dress." |
| B2 | Side-tracking | 6-9s | Side-track dolly | Still profile | "There's no studio." |
| B4 | Eye macro | 9-12s | Static | Totally still | "There's no shoot." |
| B6-fashion | Pull-back wide | 12-15s | Pull-back | Still | "AI Production Club. Studio quality without the studio." |

### Step 7 — Add Block 5: Decision Log

Add a heading 1: **📝 Block 5 — Decision Log**

Add a simple table (or inline database) tracking key decisions:

| Date | Decision | Reason | Outcome |
|---|---|---|---|
| YYYY-MM-DD | [What you chose] | [Why] | [Did it work?] |

This is gold for the case study — shows your thinking process.

**Example entries from Cloud Fashion Week:**
- 2026-06-03: Pivoted from smoke to cloud — smoke too tendril-y, hard to lock coherence
- 2026-06-04: Dropped B2 walking after 5 failed attempts — Kling applies fabric physics to body-mounted volumes
- 2026-06-05: Final VO line "studio quality without the studio" — original "no studio could shoot" failed defensibility check

### Step 8 — Add Block 6: Iteration History (use toggles)

Add a heading 1: **🔁 Block 6 — Iteration History**

For each beat, add a toggle (`/toggle`):
- Toggle title: **B[N] iterations**
- Inside the toggle: list each iteration as bullets
  - v1: [what was tried, what failed]
  - v2: [what was tried, what failed]
  - v3: [what was tried, what landed]

**Why toggles:** Iteration history can get long. Toggles keep the main page clean but accessible.

### Step 9 — Add Block 7: Lessons Learned

Add a heading 1: **💡 Block 7 — Lessons Learned**

Add a simple table:

| # | Doctrine | When it bit us | The fix |
|---|---|---|---|
| 1 | [Doctrine name] | [What went wrong] | [How we solved it] |

For each lesson, link to the relevant DOCTRINE in your DOCTRINES.md (use `/link` to add an external link).

### Step 10 — Add Block 8: QC Checklist

Add a heading 1: **✅ Block 8 — QC Checklist (pre-publish gate)**

Add a to-do list (`/todo`):
- [ ] Subject identity locked across all beats
- [ ] Impossibility visible in first 0.5 sec
- [ ] Camera-move variety (no consecutive same-move)
- [ ] Slow-mo register consistent
- [ ] Color grade unified across beats
- [ ] No audience / crew in venue beats
- [ ] VO line defensible under scrutiny
- [ ] Brand wordmark legible
- [ ] Runtime matches target
- [ ] Captions burned in
- [ ] No real brand logos
- [ ] Final pull-back / landing pays off the buildup

### Step 11 — Add Block 9: Distribution + Post-Ship

Add a heading 1: **🚀 Block 9 — Distribution + Post-Ship**

Add a table:

| Platform | Posted | Views | Likes | Comments | CTAs converted |
|---|---|---|---|---|---|
| IG Reel | YYYY-MM-DD | | | | |
| TikTok | YYYY-MM-DD | | | | |
| X / Twitter | YYYY-MM-DD | | | | |

Update this weekly post-ship. The data feeds back into Block 5 (Decision Log) for future builds.

### Step 12 — Set up sharing

Once your page is built:

1. Click "Share" (top-right of Notion page)
2. Click "Share to web"
3. Toggle ON: "Allow editing" → OFF (read-only)
4. Toggle ON: "Allow duplicate as template" — **CRITICAL** so people can copy your structure
5. Copy the public link

This is your shareable case study + template.

**Marketing use:** drop the public Notion link in your IG/TikTok bio, X profile, or Skool community as "the full behind-the-scenes."

---

## Worked example references

### Cloud Fashion Week
- [Public repo](https://github.com/owaolookadat/apc-lesson-assets/tree/main/projects/cloud-fashion-week)
- [Markdown Project Sheet](../PROJECT-SHEET.md)
- [Recipe kit](.)

### Polar Luxury
- [Public repo](https://github.com/owaolookadat/apc-lesson-assets/tree/main/projects/polar-luxury)
- [Project Sheet](../../polar-luxury/PROJECT-SHEET.md)

You can build a Notion tracker for either of these following the steps above. Use the existing markdown Project Sheet content to fill in the Notion blocks.

---

## Notion property formula cheat sheet

A few advanced formulas that make the tracker more useful:

### Progress percentage formula

On the Beat Tracker database, add a property:
- **Type:** Formula
- **Formula:**
  ```
  if(prop("Status") == "Approved", "✅", if(prop("Status") == "Generating", "🟡", if(prop("Status") == "Reshoot", "🔴", "⚪")))
  ```
This gives you a visual status indicator in every row.

### Overall project progress

On the main page, add a callout that shows count of beats by status:
- Use a linked view of the Beats database
- Group by "Status"
- Show count per group

You'll see at a glance: "3 Approved / 1 Generating / 2 TODO"

---

## Tips for using the tracker

1. **Update LIVE during the build** — don't fill it in at the end. The decision log especially needs real-time entries.
2. **Embed media inline** — drag the actual still/clip into the database row. Don't just link.
3. **Use the gallery view** for browsing — table view for editing.
4. **Duplicate this tracker per project** — once your structure is locked, "Duplicate" gives you a blank starting point for the next reel.
5. **Share the read-only public link** as your case-study marketing — viewers can duplicate it to build their own.

---

## Why this matters for your $9/month Skool play

A polished Notion tracker is:
- **Proof of work** — anyone can see the full build process
- **Replicable** — they can duplicate the template for their own reels
- **Marketing asset** — shareable as a portfolio piece
- **Conversion driver** — "want the full curriculum behind this? Join Skool $9/mo"

Each project's Notion tracker = one case study. You're building a library of public case studies over time. That library IS the marketing.

---

— Cloud Fashion Week Recipe Kit · Notion Project Tracker Build Guide · AI Production Club Track C
