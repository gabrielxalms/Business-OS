# TideWater AI Prompt Library (Higgsfield)

Companion to `albemarle-window-power-washing.md`. AI is used for **scene and bright-side shots** in hooks (Hopkins: show the result, not the grime) **and for AI-Gabe on camera, lip-synced to Gabe's real recorded voice.** Real cleaning stays real B-roll wherever possible. All cleaning, crew, owners, results and reviews stay real (see section 1 of the ad doc).

Workflow reference: `higgsfield-prompting-reference.md` (uploaded by Gabe). Build assets first, register them as Elements with exact @names, then write the video prompts.

---

## 1. The TideWater Realism Look (apply to every image and video prompt)

Gabe approved this look on the `@loc_home` reference. Every new prompt has to follow it.

**Format**
- **Always 9:16 vertical.** Main subject in the vertical center. Top ~20% stays simple (hook text goes there). Bottom ~20% has nothing important (Meta's buttons cover it).

**Camera: "iPhone on the sidewalk," not "real estate photographer"**
- Slight wide-angle lens distortion. Vertical lines lean very slightly (not perfectly corrected).
- Mild sensor noise in the shadows, slightly clipped bright highlights, normal phone HDR (not heavy).
- Slightly desaturated, true-to-life colors. No HDR look, no oversaturation, no lens flare, no CGI or illustration look.
- Not everything razor-sharp: distant things are softer and hazier.

**Light**
- **Always sunny** (Gabe's rule, no overcast). Clear autumn afternoon, sun named with a direction and ~5000K. Longer mid-afternoon shadows, dappled tree shade.
- Exception: a clip whose idea *is* weather (e.g. C-H04 rain streaks) sets its own light in the video prompt.

**Place: Charlottesville suburb, not farm country**
- Subdivision like Forest Lakes, Hollymead or Old Trail: sidewalks, curbs, mailboxes, neighbor houses.
- Houses use **one consistent material all the way around.** Default: vinyl lap siding on every wall + a ~2 ft brick foundation skirt + brick front steps. Never a brick front with vinyl sides.
- Blue Ridge = a **faint, hazy, low line** barely above the treeline. Never big or looming.

**Lived-in, not staged**
- Everyday stuff: a car in the driveway (no logo, plate unreadable), trash bin, coiled hose, doormat, house numbers, coach light, gutters with a few leaves, blinds at different heights.
- Imperfection: uneven shrubs (one overgrown, one browning), faded patchy mulch, uneven lawn with thin patches, leaves clumped unevenly (curb, beds, under trees), mixed early-November trees (green, orange, brown, one partly bare), faint dirt splash on the brick, stained and cracked sidewalk.

**Bright side (Hopkins):** AI clips show the *result and the feeling*: sun pouring through spotless glass, a sparkling, guest-ready house. No grime close-ups, no homeowner failing at a task.

**Always exclude (unless the clip calls for it):** people, animals, text, signs, logos, holiday decorations, ladders, pumpkins, dirty or streaked windows, perfect symmetry, pristine surfaces.

---

## 2. Asset registry (Higgsfield → Elements)

| @name | What it is | Used in | Status |
|---|---|---|---|
| `@loc_home` | Exterior: 2-story light gray vinyl home, brick skirt, covered porch, black door with sidelights, garage on the left, sunny autumn subdivision. 9:16. | B-H08, C-H02, C-H05 (garage), C-H08, C-H09 (if not in B-roll) | ✅ Done |
| `@loc_home_int` | Interior: living room window of the same house, seen from inside | A-H05, C-H04 | ✅ Done |
| `@loc_home_sale` | `@loc_home` edited: plain "FOR SALE" yard sign on the lawn, no brokerage branding | B-H08, "Getting ready to sell?" hook | ✅ Done |
| `@loc_home_wreath` | `@loc_home` edited: wreath on the front door, sidelights sparkling, mums and pumpkins on the steps | C-H02 | ✅ Done |
| `@loc_garage` | Inside the same home's garage: homeowner's extension ladder **leaning** against the wall (never mounted on hooks), cluttered family garage, sun through the open door | C-H05 | ✅ Done |
| `@gabe` | Gabe's character sheet from his real photos (front full body, back full body, face close-up; one face only), in his work outfit | All AI talking clips, bodies A–D, ~20 hooks | ✅ Done |
| `@tech1` | Crew tech character sheet: same work outfit as Gabe, visually distinct from Gabe (cap, sunglasses, different build) so the two faces don't blend | A1 background, other crew shots | ✅ Done (full body + close-up) |
| `@prop_wfp` | Gabe's real water-fed pole: black telescoping pole with a brush head. **Show it without a hose.** Scrubbing is slow and only on the **top sash** of a double-hung window | A1 background, any pole shot | ✅ Photo uploaded in Higgsfield |
| `@prop_squeegee` | Gabe's real tool (photo): a short black-and-blue plastic handle with a strip-washer (mop) head attached. **Gabe grips ONLY the handle in his fist; his hand never touches the mop head.** | Every AI-Gabe clip where he holds it | ✅ Photo uploaded in Higgsfield |
| `@partner1`, `@partner2` | Partners' character sheets, same format | Body D, D hooks | Later |
| `@loc_view` | Clean window framing a Blue Ridge view (only if no real footage) | A-H02 | Optional |

Rules from the Higgsfield reference: register each element under **exactly** the name used in the prompts. Any change to an asset (e.g. the house with a wreath) gets its own image, not a text instruction, if the model keeps "repairing" it.

---

## 3. Prompt log

### `@loc_home`: approved
Built in three passes: base generation (Seedream / GPT Image 2), then a realism edit, then a 9:16 reframe edit. The final edit prompt is in this conversation's history. Section 1 above captures everything it does.

### `@loc_home_int`: approved
Seedream 5.0 Pro, 9:16, with `@loc_home` attached as a reference. A white six-over-six window in the center, the sunny suburban street outside, a lived-in living room (uneven blinds, pothos and a photo on the sill, couch edge, worn rug).

### A-H05 (video, Seedance 2.5): "That first sunny morning after your windows get cleaned…"
Rewritten for Hopkins (bright side, never insult the customer). Settings: Seedance 2.5, 9:16, 5 s, 1080p, audio on (sound effects only). Reference: `@loc_home_int`. Full prompt in the chat; log it here once it's approved.

### Lessons from Gabe's image reviews (apply to every new asset)
- **Real people are messy.** First passes always come out too neat. Ask for half-open bins, crushed boxes, things leaning unevenly, stuff left out.
- **Show things the way people actually use them:** ladders lean against walls or hang high up, never mounted at chest height.
- Get the materials right for the area (vinyl all around + brick skirt), keep it in the suburbs, and keep it sunny.

### B-H08 (video, Seedance 2.5): "Realtors — here's how to make your listing photos shine."
Reference: `@loc_home_sale`. 9:16, 5 s. Full prompt in the chat.

### Body A edit plan (AI-Gabe + real B-roll)
Gabe's real recorded audio runs the whole way through. AI-Gabe is on screen for only 3 short segments; real B-roll covers everything in between.

| Segment | On screen | Audio (Gabe's real recording) |
|---|---|---|
| A1 (~4 s) | **AI-Gabe** on the front lawn of `@loc_home`, squeegee in hand. **No ladder.** Behind him (soft focus), a crew tech cleans a second-story window with the water-fed pole | "This is what happens when we come out to your house." *(Gabe's final recorded line)* |
| B-roll | Real: truck, shoes off, screens, squeegee passes, tracks, water-fed pole, siding (no concrete; no surface cleaning) | Talking points 1–7 |
| A2 (~4 s) | **AI-Gabe** turns from the window to camera | "And then, okay, this is my favorite part…" (or any line he wants to land on camera) |
| B-roll | Real: the walk-through | Walk-through line |
| A3 (~5 s) | **AI-Gabe** to camera, relaxed | 30-day guarantee + "So… yeah. That's pretty much it." |

Order: record the audio → trim each segment into its own file (`gabe_a1`, `gabe_a2`, `gabe_a3`) → attach that file as the audio reference when generating, so Seedance lip-syncs to Gabe's real voice from the start → edit with real B-roll in between.

### A1 upload order (final)
image1 house · image2–4 Gabe · image5–6 tech · image7 water-fed pole · image8 squeegee · audio1 "This is what happens when we come out to your house." 4 s.
Fixes from Gabe's review: no hose; black pole; the brush scrubs ONLY the top sash of the second-story window; slow, unhurried strokes.

### Clip naming (generated videos)
`[Body]-S[segment]_[short-name]_v[take]`, e.g. `A-S1_intro_v1.mp4`. Keep the 720p take and add `_1080` to the upscaled version: `A-S1_intro_v1_1080.mp4`. Hook clips: `A-H05_sunny-window_v1.mp4`.

- **A-S1** ✅ approved: AI-Gabe on the lawn, tech with the black pole on the top sash, third-person framing (fixed the selfie look by saying "filmed by a coworker, NOT a selfie, both hands visible, camera 2.2 m away").
- **A-S2** next: AI-Gabe inside at the open window (`@loc_home_int`), in socks (shoes off, from reviews), pointing at the track. Audio: "And then, okay, this is my favorite part… the tracks."

### Lesson: talking-to-camera + iPhone look + 9:16 makes the model default to a selfie
Always state: third-person, filmed by a coworker standing 2+ m away, NOT a selfie, both hands visible and occupied, no arm reaching toward the lens.

### A-S2b (AI process demo): the track before → after
Gabe's decision: the tracks before/after is AI (there's no real B-roll of it). It plays right after A-S2 ("…the tracks"), under Gabe's voiceover. Upload order: image1 interior, image2–4 Gabe (wardrobe only), image5 handheld brush. Close-up of the same window track from `@loc_home_int`; hands only (sleeve matches Gabe's outfit; the same gray microfiber towel as A-S2); Gabe's real handheld track brush (photo as image5); TideWater does NOT vacuum tracks: brush loosens and sweeps debris, a damp microfiber towel wipes it out. Realistic everyday dust, not gross; the "after" looks like a real cleaned track, not brand new.

- **A-S2** ✅ / **A-S2b** ✅ `A-S2b_tracks-clean_v1`: AI track before/after with Gabe's handheld brush + a damp microfiber towel (no vacuum).
- **A-S3** next: AI-Gabe at the bottom of the front steps of `@loc_home` at the end of the job (warmer, later light), towel on his shoulder, squeegee in hand. Audio `gabe_a3`: "And if anything's not spotless in the next 30 days, we just come back. Free. So… yeah. That's pretty much it." Upload: image1 house, image2–4 Gabe, image5 squeegee, audio1. ~8 s.

- **A-S3** final audio (Gabe's recording): "If anything is not up to your liking, or there happens to be build-up in the 30 days after we service your home, give us a call, and we'll come out for totally free and get your windows clear, sparkling, and exactly how you like again." It's long (~12–15 s): set the clip length to audio + 1 s; if it drifts, split it at "give us a call," into A-S3a / A-S3b.
