# C8 — Ship QC & Final Pass

PROJECT: Polar Bear × Heritage Winter Luxury · IG Reel
PATH: A (Higgsfield Veo 3.1 baked-in)

## EXPORT DELIVERABLES

- `reel-final.mp4` — 40.03 sec, 720×1280 (9:16), H.264, ~3.9 Mbps, AAC audio. Native Veo3-fast output stitched without trimming.
- `reel-final-30s.mp4` — 30.04 sec, 720×1280 (9:16), trimmed to spec (each clip cut to 6s).

## 8-BOX SHIP QC (honest scoring against `reel-final-30s.mp4`)

| # | Check | Result | Notes |
|---|---|---|---|
| 1 | Subject identity locked across all 5 beats | PASS | Same cream-white polar bear, same amber eyes, same fur density across c1-c5. Reference-image chain held. |
| 2 | Product identity consistent across relevant beats | PARTIAL | Camel-cream tartan scarf visible in B2 and B5; tortoiseshell aviators in B4 and B5; leather cuff in B3 and B5; handbag only in B5 (by design). Tartan check colorway shifts subtly between B2 and B5 (cooler in B5) — minor drift, acceptable to ship. |
| 3 | Beat timing aligned to VO (no >0.3s audio-visual drift) | PASS | Veo coordinated VO + visual within each clip. No cuts mid-word in the 30s trim. |
| 4 | Music register matches (locked list, no random tracks) | PASS | Vintage Italian lounge bed Veo-rendered across all 5; register holds throughout. Slight key-change between B1 and B2 (Veo improvising) but stays in register. |
| 5 | Captions burned in (readable, synced, no typos) | FAIL | Not burned in this pass. Veo VO is intelligible without them, but per C7 + C8 they should be there for muted-feed playback. Member fixes in CapCut step (skipped to ship-gate). |
| 6 | APC wordmark visible on landing card, no other brand referenced | PASS (with caveat) | Veo rendered "AI PRODUCTION CLUB" wordmark on B5 landing card as requested. No real brand reference anywhere (no Burberry, no logo, no engraving). Caveat: wordmark typography is Veo's choice (sans-serif), not brand-system Fraunces — would refine in CapCut. |
| 7 | Color grade consistent across all 5 clips | PASS | Cream + camel + soft-warm-black palette holds. B3 macro is slightly cooler (marble surface) but reads as a justified DP choice, not a grade break. |
| 8 | Final pull-out reveal lands the "wait — how was this made?" reaction | PASS | The B5 pull-back to the full ensemble + wordmark is the punchline. The escalation builds and the closer lands. |

**Score: 6 PASS, 1 PARTIAL, 1 FAIL → 6.5 / 8 on first ship-gate pass.**

The FAIL on captions is a known C7/CapCut step that was skipped to keep the test at FFmpeg-only stitch. Adding burned-in captions in CapCut is ~10 minutes per the lesson. With that step added the reel would land 7.5 / 8.

## LOUDNESS / EXPORT NOTES

- Audio comes from Veo bake; not normalized to −16 LUFS. Member's CapCut pass per C8 stage 2 would handle this.
- 720p (not 1080p) — Veo3-fast's native output. Would regen B5 at higher quality for client delivery (~+22 credits each).
