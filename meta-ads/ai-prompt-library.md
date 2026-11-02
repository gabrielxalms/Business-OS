# TideWater AI Prompt Library (Higgsfield)

Companion to `albemarle-window-power-washing.md`. AI is only used for **problem shots** in hooks. All cleaning, crew, owners, results and reviews stay real (see section 1 of the ad doc).

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

**Always exclude (unless the clip calls for it):** people, animals, text, signs, logos, holiday decorations, ladders, pumpkins, dirty or streaked windows, perfect symmetry, pristine surfaces.

---

## 2. Asset registry (Higgsfield → Elements)

| @name | What it is | Used in | Status |
|---|---|---|---|
| `@loc_home` | Exterior: 2-story light gray vinyl home, brick skirt, covered porch, black door with sidelights, garage on the left, sunny autumn subdivision. 9:16. | B-H08, C-H02, C-H05, C-H09 (if not in B-roll) | ✅ Done |
| `@loc_home_int` | Interior: living room window of the same house, seen from inside | A-H05, C-H04, C-H08 | ⏳ Next |
| `@prop_sign` | Generic realtor yard sign, no brand | B-H08 | Later |
| `@homeowner` | Generic homeowner character sheet for the ladder shot | C-H05 | Later |

Rules from the Higgsfield reference: register each element under **exactly** the name used in the prompts. Any change to an asset (e.g. the house with a wreath) gets its own image, not a text instruction, if the model keeps "repairing" it.

---

## 3. Prompt log

### `@loc_home`: approved
Built in three passes: base generation (Seedream / GPT Image 2), then a realism edit, then a 9:16 reframe edit. The final edit prompt is in this conversation's history. Section 1 above captures everything it does.

### `@loc_home_int`: next
See the chat. Will be logged here once Gabe approves it.
