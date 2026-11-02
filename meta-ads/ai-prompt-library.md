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
| A1 (~4 s) | **AI-Gabe** on the front lawn of `@loc_home`, squeegee in hand, ladder behind him | Opening: "So, uh, this is basically what happens when we come out to your house." |
| B-roll | Real: truck, shoes off, screens, squeegee passes, tracks, water-fed pole, siding, concrete | Talking points 1–7 |
| A2 (~4 s) | **AI-Gabe** turns from the window to camera | "And then, okay, this is my favorite part…" (or any line he wants to land on camera) |
| B-roll | Real: the walk-through | Walk-through line |
| A3 (~5 s) | **AI-Gabe** to camera, relaxed | 30-day guarantee + "So… yeah. That's pretty much it." |

Order: record the audio → cut it into segments → generate the AI-Gabe clips with the exact words → lip-sync them to the real audio → edit.
