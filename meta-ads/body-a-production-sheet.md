# Body A Production Sheet: "The Process" (TideWater Window Cleaning)

Everything needed to finish Body A and its first 10 ads, in one place. Every prompt here is the latest approved version.

**How each ad is built:** Hook (2–4 s) → Body A (~45–60 s) → CTA. **10 hooks × Body A × CTA C1 = 10 ads.**

**Rules that apply to everything:**
- 9:16 vertical. Generate at **720p**, then upscale the keeper to **1080p** (Higgsfield Upscale). Export the final ad at 1080×1920.
- Gabe's voice is **always his real recording.** AI-Gabe is lip-synced to it.
- Hopkins rules: never insult the customer, show the bright side, never knock competitors.
- TideWater sells **windows (inside, outside, screens, tracks, sills) and siding soft wash. No surface cleaning.** Never show the surface-cleaner B-roll.
- **Clip naming:** `[Body]-S[segment]_[name]_v[take]` for body clips and `[Hook]_[name]_v[take]` for hooks; add `_1080` after upscaling.

---

## 1. Audio to record (phone voice memos, recorded outside)

### Body A (one continuous, loose take, then trim the three AI segments out)
Talking points, in your own words:
1. You get a text when we're on our way.
2. Shoes come off at the door.
3. Screens come off and get washed by hand.
4. Scrub, squeegee, then hand-detail the edges.
5. The tracks and sills (your favorite part).
6. Purified water up high, so it dries spot-free.
7. Siding: soft wash, no blasting.
8. The walk-through, and the 30-day guarantee.

| File | Exact line (as recorded) | Length |
|---|---|---|
| `gabe_a1` | "This is what happens when we come out to your house." | ~3 s |
| `gabe_a2` | "And then, okay, this is my favorite part… the tracks." | ~3–4 s |
| (voiceover, no AI) | "We brush 'em all out, wipe 'em down, do the sills… this is the part people always notice after." | — |
| `gabe_a3` | "If anything is not up to your liking, or there happens to be build-up in the 30 days after we service your home, give us a call, and we'll come out for totally free and get your windows clear, sparkling, and exactly how you like again." | 14 s |

⚠️ **Before March:** re-record `gabe_a3` without "build-up" (or add "pollen excluded"). Spring pollen would trigger the guarantee.

### Hooks (read word for word, one file each: `hook_A-H01` … `hook_A-H10`)
| # | Line |
|---|---|
| A-H01 | "One pass. Watch the glass disappear." |
| A-H02 | "Crozet — this is the Blue Ridge view you bought your house for." |
| A-H03 | "Well water leaves white spots on glass. Here's how we get them off for good." |
| A-H04 | "The detail that makes a clean window look brand new: the tracks." |
| A-H05 | "That first sunny morning after your windows get cleaned…" |
| A-H06 | "Want your siding looking like the day you moved in?" |
| A-H07 | "The best your windows have looked since the day they were installed." |
| A-H08 | "Inside, outside, and the screens. Every single window." |
| A-H09 | ⚠️ "We just finished a house in Earlysville and the owner asked if we'd taken the glass out." *(only if true)* |
| A-H10 | "Every cleaning includes these 4 things." |

### CTA C1
"Tap **Get Quote** below. Answer 3 quick questions, and we'll text you a price." *(Add "within the hour" only if you can really do that.)*

---

## 2. Reference images (all done ✅)

| Name | What |
|---|---|
| `loc_home` | House exterior, 9:16, sunny autumn subdivision |
| `loc_home_int` | Living room window of the same house |
| `loc_home_sale` / `loc_home_wreath` / `loc_garage` | For other bodies' hooks (B-H08, C-H02, C-H05) |
| Gabe ×3 | Gabe's reference images (one face close-up + full body) |
| Tech ×2 | Tech's full body + close-up (cap, sunglasses) |
| Water-fed pole | Black pole, brush head. **Never show a hose** |
| Gabe's tool | Short black-and-blue handle with a strip-washer head. **Gabe holds the handle only** |
| Track brush | Gabe's handheld track brush. **TideWater doesn't vacuum tracks** |

---

## 3. Body A edit order

Gabe's full Body A recording runs underneath the whole time.

| # | Clip | Audio over it |
|---|---|---|
| 1 | **A-S1_intro** (AI-Gabe on the lawn, tech on the pole behind) | `gabe_a1` |
| 2 | Real B-roll: shoes off, screens, squeegee passes | Points 1–4 |
| 3 | **A-S2_tracks** (AI-Gabe pointing at the track) | `gabe_a2` |
| 4 | **A-S2b_tracks-clean** (AI brush before/after) | "We brush 'em all out…" |
| 5 | Real B-roll: water-fed pole, siding soft wash | Points 6–7 |
| 6 | **A-S3_guarantee** (AI-Gabe on the front steps), with 2–3 s of sparkling-window B-roll during "clear, sparkling" | `gabe_a3` |
| 7 | CTA C1 | CTA line |

Captions burned in, hook text in the top third for the first 3 s, nothing important in the bottom 20%.

---

## 4. Body A video prompts (Seedance 2.5)

### A-S1_intro: 4 s
Uploads: `@image1` house · `@image2–4` Gabe · `@image5–6` tech · `@image7` water-fed pole · `@image8` Gabe's tool · `@audio1` gabe_a1

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: slight wide-angle distortion, mild sensor noise in the shadows, slightly clipped bright sky, normal phone HDR, slightly desaturated true-to-life colors. Third-person shot filmed by a coworker standing in front of Gabe. NOT a selfie. NOT present: no selfie framing, no arm reaching toward the lens, no phone in Gabe's hand, no text, no captions, no logos or printing on clothing, no music, no ladder, no hose of any kind, no third person visible, no generated voice, no CGI look, no gimbal smoothness, no studio lighting.

SCENE CONTEXT: On a sunny autumn afternoon in a Charlottesville subdivision, a window cleaner (Gabe) stands on a client's front lawn mid-job, holding his strip washer, while a coworker films him. Gabe turns to the camera and starts explaining what happens when his crew comes out, speaking exactly the words in @audio1. Behind him, softly out of focus, one of his techs slowly scrubs the top pane of a second-story window with a black water-fed pole, water sheeting down the glass in the sun. Relaxed, friendly, unscripted.

ACTIVE REFERENCES:
@image1 — the house: siding, brick skirt, windows, porch, front door, landscaping and street 100% match this image. Environment, materials and mood only; reference framing not inherited.
@image2, @image3, @image4 — all three show the SAME man, Gabe, the man in the foreground. His face, hair, skin tone, facial hair, build and work outfit 100% match. Reference backgrounds and reference camera angles NOT inherited.
@image5, @image6 — the SAME younger man, the tech in the background. His build, cap, sunglasses and work outfit 100% match. He is a different person from Gabe and never takes on Gabe's face. Reference backgrounds NOT inherited.
@image7 — the water-fed pole: a black telescoping pole and its brush head 100% match this image. Shown WITHOUT any hose.
@image8 — Gabe's tool: the short black-and-blue plastic handle and the strip-washer (mop) head attached to it 100% match this image. He holds it ONLY by the black-and-blue handle.
@audio1 — Gabe's real voice and the ONLY dialogue in the clip. Gabe's lips, jaw, pauses and breaths sync exactly to this audio.

LOCATION MAP: Foreground, left half of the frame: Gabe stands on the front lawn 2.2 m from the camera, framed from mid-thigh up, with both hands visible in frame. Background, right half of the frame, 8–10 m behind him (soft focus): the front of the house from @image1. The tech stands on the lawn near the foundation beds to frame-right of the porch, his back and side to the camera, facing the house. His black pole (@image7) is extended up about 6 m. The brush rests on the TOP sash (the upper pane) of a second-story double-hung window in the upper-right part of the frame. The bottom sash of that window is not touched. The camera operator is never visible. The sun is behind the camera and to the left, lighting Gabe's face and the front of the house.

FIRST FRAME / BLOCKING: Gabe is already in frame, body angled about 30° toward the house as if he just stopped working. His RIGHT hand grips only the black-and-blue handle of the tool (@image8) at his side; his fingers never touch the mop head. His LEFT hand rests relaxed on his hip. Both arms stay close to his body; neither arm reaches toward the camera at any point. The tech is already mid-stroke with the brush on the top pane of the second-story window. No empty establishing frame, no delayed reveal.

FORMAT MODE: Single continuous take, 4 s, zero cuts.

OPTICS: 47° lens, locked, no drift mid-segment. Focus on Gabe's face; the house, the tech and the pole are softly out of focus but clearly readable.

CAMERA: Third-person handheld phone held by a coworker standing 2.2 m in front of Gabe, at Gabe's chest height, pointed at him. Natural breathing sway (about 1–2 cm), small human reframes. The camera is never in Gabe's hand and never at arm's length from him. Never gimbal-smooth, never digital jitter.

ACTION:
Start: Gabe turns his head and shoulders from the house toward the camera with a small easy smile, timed so he's facing the camera as the first word of @audio1 begins.
During the audio: he talks to the camera, lips synced to @audio1. On "what happens," he tips the tool hand loosely back toward the house and the tech, then lets it drop to his side. His left hand stays on his hip.
After the audio ends: he holds a relaxed half-smile for the last moment, mouth closed.
Background, the whole clip: the tech scrubs SLOWLY and calmly, only about two to three strokes in the entire clip. Each stroke is a short, unhurried side-to-side movement of about 30 cm that stays entirely inside the top pane. The brush never moves down onto the bottom pane. His face never turns toward the camera.

PERFORMANCE: Gabe is unrehearsed and relaxed: natural blinks, a slight squint from the sun, a small inhale before he speaks, eyebrows lifting slightly on "what happens." Mouth shapes match the audio exactly; jaw relaxed. Not salesy. He looks like he's talking to a coworker filming him. The tech is focused, steady and unhurried, unaware of the camera.

PHYSICS: The tool has real weight in Gabe's hand, held only by its handle; the strip-washer sleeve is damp. Gabe's shirt lags his shoulders slightly. The long black pole flexes very slightly as the tech moves it; his arms and shoulders carry its weight with slow, controlled motion. Water from the brush runs down the top pane and over the bottom pane, sparkling in the sun, and drips off the sill. A light breeze moves a few leaves and the trees.

LIGHTING: Single source: the afternoon sun, ~5000K, behind the camera to the left, lighting Gabe's face directly with soft natural shadow under the brow and chin. The same sun lights the house front, the tech, and the water on the glass, creating bright glints. Shadows keep detail.

AUDIO: Use @audio1 as the dialogue, unchanged. The words are: "This is what happens when we come out to your house." Do not generate any other voice or words. Underneath it, very quiet outdoor ambience only: a light breeze, distant birds, faint trickling water. No music.

STYLE: Photoreal, natural iPhone color, light grain.

POSITIVE LOCKS: Third-person shot, NOT a selfie: both of Gabe's hands are visible the whole clip, the tool held only by its black-and-blue handle in his right hand, his left hand on his hip, and neither arm reaches toward the camera. Exactly two people visible. Gabe (foreground) matches @image2, @image3 and @image4 in every frame. The tech (background) matches @image5 and @image6, stays facing the house, and never looks at the camera. The two never share a face. Lip-sync matches @audio1 exactly; only Gabe speaks. No ladder, no hose. The pole is black and matches @image7. The brush stays ONLY on the top pane, with slow strokes, two to three in total. Single continuous take, no cuts. The house matches @image1.
```

### A-S2_tracks: audio + 1 s (usually 5 s)
Uploads: `@image1` interior · `@image2–4` Gabe · `@audio1` gabe_a2

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: slight wide-angle distortion, mild sensor noise in the shadows, slightly clipped highlights in the window, normal phone HDR, slightly desaturated true-to-life colors. Third-person shot filmed by a coworker standing in the room. NOT a selfie. NOT present: no selfie framing, no arm reaching toward the lens, no phone in Gabe's hand, no shoes on Gabe's feet, no text, no captions, no logos or printing on clothing, no music, no other people, no generated voice, no CGI look, no gimbal smoothness.

SCENE CONTEXT: Inside a client's lived-in living room on a sunny afternoon, a window cleaner (Gabe), in his socks, kneels at a front window with the bottom sash raised open. He turns to the coworker filming him and, with a little grin, points down at the window track, speaking exactly the words in @audio1. Casual, a little playful, like he's showing a neighbor his favorite trick.

ACTIVE REFERENCES:
@image1 — the room: the white six-over-six double-hung window, white trim and sill, blinds, curtains, sill objects, couch edge, rug, walls, and the sunny street outside 100% match this image. Environment, materials and mood only; reference framing not inherited.
@image2, @image3, @image4 — all three show the SAME man, Gabe. His face, hair, skin tone, facial hair, build and work outfit 100% match. Reference backgrounds and reference camera angles NOT inherited.
@audio1 — Gabe's real voice and the ONLY dialogue in the clip. His lips, jaw, pauses and breaths sync exactly to this audio, including the pause after "okay."

LOCATION MAP: The window from @image1 sits at frame-right, its bottom sash raised about 40 cm, exposing the bottom track and sill. The potted pothos and the framed photo have been moved to the floor beside the wall. Gabe kneels on the rug in front of the window, his body angled toward it, about 2 m from the camera, framed from the knees up, both hands visible. Sunlight comes through the open window from frame-right, lighting the side of his face nearest the window. The camera works from inside the room, near the couch, and the camera operator is never visible.

FIRST FRAME / BLOCKING: Gabe is already kneeling at the window, looking at the track, his left hand resting on the sill, his right hand on his knee. A folded gray microfiber towel hangs over his right shoulder. He wears dark socks, no shoes. No empty establishing frame, no delayed reveal.

FORMAT MODE: Single continuous take, zero cuts, same length as the clip.

OPTICS: 47° lens, locked, no drift mid-segment. Focus on Gabe's face; the window and the track are slightly soft but readable.

CAMERA: Third-person handheld phone held by a coworker standing about 2 m away at Gabe's head height (slightly above him, since he's kneeling). Natural breathing sway (about 1–2 cm), small human reframes. Never gimbal-smooth, never digital jitter.

ACTION:
Start: Gabe looks up from the track and turns his head and shoulders toward the camera with a small grin, facing the camera as the first word of @audio1 begins.
During the audio: lips synced to @audio1. On "okay," he raises his eyebrows playfully. In the pause after "favorite part," he points his right index finger down at the open window track. On "the tracks," he glances down at the track, then back at the camera.
After the audio ends: he holds a small knowing smile, still pointing at the track.

PERFORMANCE: Unrehearsed, playful and proud of the detail: natural blinks, a small inhale before he speaks, a slight smile building through the line. Mouth shapes match the audio exactly; jaw relaxed. Not salesy.

PHYSICS: His knees press into the rug slightly. The microfiber towel hangs with real weight on his shoulder and shifts when he turns. The open sash stays still. A gentle breeze moves the curtain edge slightly. The track holds a light layer of everyday dust and a couple of tiny leaf bits, nothing gross.

LIGHTING: Single main source: afternoon sunlight, ~5000K, through the open window at frame-right, lighting the window side of Gabe's face with a soft falloff to the other side. The room is dimmer, with natural falloff. Shadows keep detail.

AUDIO: Use @audio1 as the dialogue, unchanged. The words are: "And then, okay, this is my favorite part… the tracks." Do not generate any other voice or words. Underneath it, very quiet room tone and faint birds through the open window. No music.

STYLE: Photoreal, natural iPhone color, light grain.

POSITIVE LOCKS: Third-person shot, NOT a selfie: both of Gabe's hands are visible, and neither arm reaches toward the camera. Exactly one person. Gabe matches @image2, @image3 and @image4 in every frame. He is in socks with no shoes. Lip-sync matches @audio1 exactly; only Gabe speaks. The bottom sash stays open and the track stays visible. Single continuous take, no cuts. The room matches @image1.
```

### A-S2b_tracks-clean: 5 s (no audio reference)
Uploads: `@image1` interior · `@image2–4` Gabe (wardrobe only) · `@image5` track brush

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: mild sensor noise in the shadows, slightly clipped highlights where the sun hits, normal phone HDR, slightly desaturated true-to-life colors. NOT present: no faces, no people besides one pair of hands and forearms, no vacuum, no text, no captions, no logos or brand names, no music, no dialogue, no CGI look, no gimbal smoothness, no exaggerated "brand new" shine.

SCENE CONTEXT: A close-up of a window cleaner's hands cleaning the bottom track of an open living-room window. A small handheld brush scrubs along the track channel, loosening everyday dust and debris and sweeping it along. Then a damp microfiber towel wipes the track clean. Ends holding on the clean track in the sun. Satisfying, calm, real.

ACTIVE REFERENCES:
@image1 — the window: the white six-over-six double-hung window, white trim, white sill, and the room 100% match this image. Environment, materials and mood only; reference framing not inherited.
@image2, @image3, @image4 — wardrobe only: the sleeves and the work-outfit fabric on the forearms match this man's outfit. His face does NOT appear.
@image5 — the handheld brush: its shape, handle, size, color and bristles 100% match this image.

LOCATION MAP: A tight close-up of the bottom of the window from @image1. The bottom sash is raised about 40 cm, and its bottom edge shows at the top of the frame. The white vinyl window track runs horizontally across the middle of the frame, with the white sill in front of it in the lower part of the frame. Through the open window (soft focus, upper part of the frame): green lawn and autumn leaves outside. Sunlight comes through the opening from outside, slightly frame-right. The camera is inside the room, about 50 cm from the track, looking down at it at about 45°.

FIRST FRAME / BLOCKING: The track is already in frame, holding a realistic layer of everyday debris: gray dust and grit packed into the corners and channels, a few small dried leaf fragments, a couple of tiny dead gnats, and a little pollen. Not gross, just normal. A right hand holding the brush (@image5) is already at the left end of the track, bristles down in the channel. The left hand rests on the sill holding a folded gray microfiber towel.

FORMAT MODE: Single continuous take, 5 s, zero cuts.

OPTICS: 29° lens, locked, no drift mid-segment. Focus on the track; the outside view is soft.

CAMERA: Handheld phone held by a coworker, steady with slight natural breathing sway (about 0.5 cm). No zoom. Never gimbal-smooth, never digital jitter.

ACTION:
0.0–2.8 s: The brush scrubs along the channel with short, quick back-and-forth strokes, working steadily from left to right. The bristles flex and loosen the packed dust and grit. Loosened debris is pushed ahead of the brush and gathers toward the right end of the track. Behind the brush, the channel is visibly cleaner.
2.8–4.3 s: The brush lifts out of frame-right. The left hand wraps the damp microfiber towel over two fingers and wipes along the track in one pass from left to right, picking up the loosened dust and gathered debris. The towel shows a gray smudge of dirt as it lifts away.
4.3–5.0 s: The hand and towel exit frame. Hold on the clean track: bright white vinyl lit by the sun, with normal faint wear marks from years of use still visible.

PHYSICS: The bristles bend and spring back with each stroke. Fine dust puffs up slightly and settles. Debris moves only when the brush or towel touches it. Once cleaned, a section never gets dirty again (one-way state). The damp towel compresses into the channel and comes away carrying the dirt. The sash and window never move.

LIGHTING: Single source: afternoon sunlight, ~5000K, through the open window from outside, slightly frame-right, raking low across the track so the dust shows in the "before" and the clean vinyl glows softly in the "after." Room fill is dim and warm. Shadows keep detail.

AUDIO: Real-world sound only, kept low: the soft scratch of bristles in the track, a soft cloth swipe, faint birds outside. No music, no dialogue.

STYLE: Photoreal, natural iPhone color, light grain.

POSITIVE LOCKS: No face visible; exactly one pair of hands. No vacuum anywhere. The brush matches @image5. The track goes from dirty to clean only, never the reverse. The clean result looks like a real, well-cleaned, years-old track, not brand new or glowing. Single continuous take, no cuts. The window matches @image1.
```

### A-S3_guarantee: 15 s
Uploads: `@image1` house · `@image2–4` Gabe · `@image5` Gabe's tool · `@audio1` gabe_a3

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: slight wide-angle distortion, mild sensor noise in the shadows, slightly clipped bright sky, normal phone HDR, slightly desaturated true-to-life colors. Third-person shot filmed by a coworker standing in front of Gabe. NOT a selfie. NOT present: no selfie framing, no arm reaching toward the lens, no phone in Gabe's hand, no text, no captions, no logos or printing on clothing, no music, no other people, no ladder, no hose, no generated voice, no CGI look, no gimbal smoothness, no studio lighting.

SCENE CONTEXT: The job is done. Late on a sunny autumn afternoon, a window cleaner (Gabe) stands at the bottom of a client's brick front steps, a microfiber towel over his shoulder and his strip washer in hand. Behind him, every front window sparkles in the warm low sun. He explains the 30-day guarantee to the coworker filming him, speaking exactly the words in @audio1. Relaxed, sincere, confident, a job well done.

ACTIVE REFERENCES:
@image1 — the house: siding, brick skirt, brick front steps, windows, porch, front door, landscaping and street 100% match this image. Environment, materials and mood only; reference framing not inherited.
@image2, @image3, @image4 — all three show the SAME man, Gabe. His face, hair, skin tone, facial hair, build and work outfit 100% match in every frame of the full 15 seconds. Reference backgrounds and reference camera angles NOT inherited.
@image5 — Gabe's tool: the short black-and-blue plastic handle and the strip-washer (mop) head attached to it 100% match this image. He holds it ONLY by the black-and-blue handle.
@audio1 — Gabe's real voice and the ONLY dialogue in the clip, 14 seconds long. His lips, jaw, pauses and breaths sync exactly to this audio from the first word to the last.

LOCATION MAP: Foreground, center-left of the frame: Gabe stands on the front walkway at the bottom of the brick steps. Background (soft focus, 3–8 m behind him): the covered porch, the black front door with its sidelights, and the front windows from @image1, all clean and sparkling with warm sun glints. The camera operator stands on the walkway facing him and is never visible. The low sun is behind the camera and to the left.

FIRST FRAME / BLOCKING: Gabe is already in frame, 2.2 m from the camera, framed from mid-thigh up, facing the camera. His RIGHT hand grips only the short black-and-blue plastic handle of the tool (@image5) in a relaxed fist at his side, with the strip-washer head attached at the end of the handle. His fingers never touch the mop head. The towel is draped over his LEFT shoulder, and his left hand rests loosely at his side. No empty establishing frame, no delayed reveal.

FORMAT MODE: Single continuous take, 15 s, zero cuts.

OPTICS: 47° lens, locked, no drift mid-segment. Focus stays on Gabe's face the whole time; the house is softly out of focus, but the window glints are clearly visible.

CAMERA: Third-person handheld phone held by a coworker at Gabe's chest height. Over the full 15 seconds the coworker takes one or two slow, small steps forward, closing from 2.2 m to about 1.6 m, so the framing slowly tightens from mid-thigh up to waist up. Natural breathing sway (about 1–2 cm), a gentle footstep pulse on each step, small human reframes. The camera is never in Gabe's hand. Never gimbal-smooth, never digital jitter.

ACTION (beats follow the phrases of @audio1):
Before the first word: a small inhale, eyes on the camera.
"If anything is not up to your liking,": sincere, with a slight open-palm gesture of his left hand at waist height, then it drops.
"or there happens to be build-up in the 30 days after we service your home,": he tips his head toward the house behind him, then back to the camera.
"give us a call,": a small, easy nod.
"and we'll come out for totally free": his eyebrows lift and a smile starts.
"and get your windows clear, sparkling, and exactly how you like again.": he glances back over his shoulder at the sparkling windows, then returns to the camera with a warm, genuine smile.
After the last word: he holds the smile, mouth closed, for the final moment.

PERFORMANCE: Unrehearsed, sincere and relaxed, like he's reassuring a neighbor: natural blinks at a normal rate, a slight squint from the low sun, small breaths between phrases, small natural head movements. Mouth shapes match the audio exactly for all 14 seconds; jaw relaxed. Not salesy, not over-animated. His face and identity stay identical from start to finish.

PHYSICS: The tool has real weight in his right hand, held only by its handle; the strip-washer sleeve is damp and hangs slightly heavy. The towel stays draped on his left shoulder with real weight and shifts slightly when he turns his head. His shirt lags his shoulders slightly. A light breeze moves a few leaves on the walkway and in the trees.

LIGHTING: Single source: the late-afternoon sun, low and warm (~4000K), behind the camera to the left, lighting Gabe's face with a warm glow and long soft shadows, consistent for the full clip. The same low sun makes the clean front windows behind him glint. Shadows keep detail.

AUDIO: Use @audio1 as the dialogue, unchanged. The words are: "If anything is not up to your liking, or there happens to be build-up in the 30 days after we service your home, give us a call, and we'll come out for totally free and get your windows clear, sparkling, and exactly how you like again." Do not generate any other voice or words. Underneath it, very quiet outdoor ambience only: a light breeze, distant birds. No music.

STYLE: Photoreal, natural iPhone color, light grain.

POSITIVE LOCKS: Third-person shot, NOT a selfie: neither arm reaches toward the camera at any point. His right hand holds the tool only by the black-and-blue handle the whole clip, never touching the mop head, and the towel stays on his left shoulder. Exactly one person. Gabe matches @image2, @image3 and @image4 in every frame for the full 15 seconds; his face never changes. Lip-sync matches @audio1 exactly from first word to last; only Gabe speaks. The windows behind him are clean and sparkling. Single continuous take, no cuts. The house matches @image1.
```

If Gabe's face drifts: split `gabe_a3` at "give us a call," into two ~7 s files and generate `A-S3a` and `A-S3b` as two 8 s clips.

---

## 5. Body A hooks

| Hook | Footage | Status |
|---|---|---|
| A-H01 | Gabe's squeegee B-roll | ✅ Ready |
| A-H02 | Stock: mountain view through a clean window (or AI) | Find stock |
| A-H03 | Stock: spot removal on glass (commercial license, no logos or faces) | Find stock |
| A-H04 | Reuse `A-S2b_tracks-clean` | ✅ Ready |
| A-H05 | AI sunny window (prompt below) | Generate |
| A-H06 | Gabe's siding soft-wash B-roll | ✅ Ready |
| A-H07 | Gabe's squeegee B-roll, ending on a sparkling pane | ✅ Ready |
| A-H08 | Gabe's B-roll montage: screens, inside, outside | ✅ Ready |
| A-H09 | AI-Gabe, only if the story is true | Gabe's call |
| A-H10 | AI-Gabe holding up 4 fingers (prompt below) | Generate |

### A-H05_sunny-window: 5 s (no audio reference)
Uploads: `@image1` interior

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: slight wide-angle distortion, mild sensor noise in the shadows, slightly clipped highlights in the window, normal phone HDR, slightly desaturated true-to-life colors. NOT present: no text, no captions, no logos, no music, no faces, no people besides one hand and forearm, no dust, no streaks or smudges on the glass, no CGI look, no gimbal smoothness.

SCENE CONTEXT: The first sunny morning after the windows were professionally cleaned. Warm sunlight pours through a spotless living-room window. A hand sets a mug of coffee on the sill, and the camera drifts toward glass so clear the street outside looks like there's no glass at all. Calm, happy, fresh. Ends holding on the crystal-clear view.

ACTIVE REFERENCES: @image1 — the window, trim, windowsill, blinds, curtains, sill objects, room and the street view outside 100% match this image. It controls environment, materials and mood only; reference framing not inherited.

LOCATION MAP: Midground: the white six-over-six double-hung window fills the middle 60% of the frame, the white windowsill along the bottom third with the potted pothos at frame-left and the framed photo at frame-right. Raised blinds and pushed-back linen curtains at the edges. Beyond the glass (sharp and vivid through the clean glass, 10–30 m): the sunny suburban street, sidewalk, the neighbor's beige house, autumn trees, blue sky. The camera starts inside the room, 1.5 m from the window, at chest height.

FIRST FRAME / BLOCKING: A right hand holding a white ceramic mug of coffee is entering from frame-right, about to set it on the sill at center-right. No empty establishing frame, no delayed reveal.

FORMAT MODE: Single continuous take, 5 s, zero cuts.

OPTICS: 47° lens, locked, no drift mid-segment. Focus on the glass and the view beyond; deep enough focus that the street outside stays crisp.

CAMERA: Handheld phone at chest height, slight natural breathing sway (about 1 cm). A slow, gentle walk-in toward the window from 1.5 m to 0.8 m over the shot, with small human reframes. Never gimbal-smooth, never digital jitter.

ACTION:
0.0–1.5 s: The hand sets the mug down on the sill with a soft tap, then withdraws out of frame-right. A thin wisp of steam rises from the coffee.
1.5–4.0 s: The camera drifts slowly toward the window. Sunlight comes through the spotless glass, laying sharp shadows of the window grids across the sill and the mug.
4.0–5.0 s: Hold on the view through the glass. The street outside is so crisp and clear the glass seems invisible. Steam keeps curling gently.

PHYSICS: The mug has weight and settles with a small tap. The steam is thin, rising and drifting slightly in the warm air. The window grid shadows stay steady and sharp. The glass shows only a faint, natural reflection at the very edges.

LIGHTING: Single main source: the morning sun, ~4800K, low and slightly frame-right outside the window, streaming in and creating soft warm bloom at the edges of the glass and bright highlights on the sill and mug. The room is dimmer, with natural falloff. The hand is lit by the sunlight. Shadows keep detail.

AUDIO: Real-world sound only: the soft ceramic tap of the mug on the sill, quiet morning room tone, birds chirping faintly outside. No music, no dialogue.

STYLE: Photoreal, natural iPhone color, light grain, slight halation around the brightest window highlights.

POSITIVE LOCKS: Exactly one hand (right hand, gray sleeve cuff); no face ever visible. The glass is perfectly clean the whole time. Exactly one mug. Single continuous take, no cuts. The room matches @image1. The final 1 s holds on the crystal-clear view.
```

### A-H10_four-things: 4 s
Uploads: `@image1` house · `@image2–4` Gabe · `@image5` Gabe's tool · `@audio1` hook_A-H10

```
GLOBAL STYLE: Photoreal live-action, vertical 9:16, ordinary iPhone video look: slight wide-angle distortion, mild sensor noise in the shadows, slightly clipped bright sky, normal phone HDR, slightly desaturated true-to-life colors. Third-person shot filmed by a coworker standing in front of Gabe. NOT a selfie. NOT present: no selfie framing, no arm reaching toward the lens, no phone in Gabe's hand, no text, no captions, no logos or printing on clothing, no music, no other people, no ladder, no hose, no generated voice, no CGI look, no gimbal smoothness, no studio lighting.

SCENE CONTEXT: On a sunny autumn afternoon in a Charlottesville subdivision, a window cleaner (Gabe) stands on a client's driveway beside the garage, mid-job, strip washer in hand. He looks at the coworker filming him, holds up four fingers and says exactly the words in @audio1. Confident, friendly, quick.

ACTIVE REFERENCES:
@image1 — the house: siding, brick skirt, white garage door, windows, driveway, the parked SUV, landscaping and street 100% match this image. Environment, materials and mood only; reference framing not inherited.
@image2, @image3, @image4 — all three show the SAME man, Gabe. His face, hair, skin tone, facial hair, build and work outfit 100% match. Reference backgrounds and reference camera angles NOT inherited.
@image5 — Gabe's tool: the short black-and-blue plastic handle and the strip-washer (mop) head attached to it 100% match this image. He holds it ONLY by the black-and-blue handle.
@audio1 — Gabe's real voice and the ONLY dialogue in the clip. His lips, jaw and breaths sync exactly to this audio.

LOCATION MAP: Foreground, center of the frame: Gabe stands on the concrete driveway 2.2 m from the camera, framed from mid-thigh up. Background (soft focus, 4–7 m behind him): the white paneled garage door and the light gray vinyl siding from @image1, with the rear of the parked SUV partly visible at frame-left and a front window glinting at frame-right. The camera operator stands on the driveway facing him and is never visible. The sun is behind the camera and to the left, lighting Gabe's face.

FIRST FRAME / BLOCKING: Gabe is already in frame, facing the camera. His RIGHT hand grips only the black-and-blue handle of the tool (@image5) in a relaxed fist at his side; his fingers never touch the mop head. His LEFT hand is already rising to chest height. No empty establishing frame, no delayed reveal.

FORMAT MODE: Single continuous take, 4 s, zero cuts.

OPTICS: 47° lens, locked, no drift mid-segment. Focus on Gabe's face and raised hand; the garage and house are softly out of focus.

CAMERA: Third-person handheld phone held by a coworker standing 2.2 m in front of Gabe, at his chest height. Natural breathing sway (about 1–2 cm), small human reframes. The camera is never in Gabe's hand. Never gimbal-smooth, never digital jitter.

ACTION:
Start: Gabe's left hand comes up to chest height, palm facing the camera, with exactly four fingers raised and the thumb folded in, timed to land as the first word of @audio1 begins.
During the audio: lips synced to @audio1. He holds the four fingers steady at chest height, close to his body, with a confident half-smile and slightly raised eyebrows on "4 things."
After the audio ends: he gives a tiny nod, hand still up, as if about to count them off.

PERFORMANCE: Unrehearsed, confident and friendly: natural blinks, a slight squint from the sun, a small inhale before he speaks. Mouth shapes match the audio exactly; jaw relaxed. Not salesy.

PHYSICS: The tool has real weight in his right hand, held only by its handle; the strip-washer sleeve is damp. His shirt lags his arm slightly as it rises. A light breeze moves a few leaves on the driveway.

LIGHTING: Single source: the afternoon sun, ~5000K, behind the camera to the left, lighting Gabe's face and raised hand with soft natural shadows. Background lit by the same sun. Shadows keep detail.

AUDIO: Use @audio1 as the dialogue, unchanged. The words are: "Every cleaning includes these 4 things." Do not generate any other voice or words. Underneath it, very quiet outdoor ambience only: a light breeze, distant birds. No music.

STYLE: Photoreal, natural iPhone color, light grain.

POSITIVE LOCKS: Third-person shot, NOT a selfie. Exactly FOUR fingers raised on his left hand, thumb folded, never three, never five, held close to his chest and never reaching toward the camera. His right hand holds the tool only by the black-and-blue handle. Exactly one person. Gabe matches @image2, @image3 and @image4 in every frame. Lip-sync matches @audio1 exactly; only Gabe speaks. Single continuous take, no cuts. The house matches @image1.
```

---

## 6. Meta setup for these 10 ads

- **Ad names:** `A-H01-C1` … `A-H10-C1`.
- **Primary text:** "Crystal clear, inside and out. Screens hand-washed, tracks brushed out, shoes off at your door, and a walk-through before we leave. Let the light back in. 👇 Tap for a free quote."
- **Headline:** "Windows you'll forget are there"
- **Campaign:** Leads → Instant Form (Higher intent), Albemarle + Charlottesville ZIPs, "people living in," broad/Advantage+, one ad set for Body A with all 10 ads, about $20–30/day.
- **Judge:** hook rate (3-second views ÷ impressions; 30%+ is good, under 20% after ~1,000 impressions means kill it), then cost per lead, then cost per booked job.

## 7. Troubleshooting (what's worked so far)

| Problem | Fix |
|---|---|
| Looks like a selfie | "Third-person, filmed by a coworker 2.2 m away, NOT a selfie, both hands visible, no arm toward the lens" |
| Background action too fast | Fewer, slower strokes; "two to three strokes in the entire clip" |
| Wrong pane scrubbed | "ONLY the top sash; the brush never moves to the bottom pane" |
| Thin details go thick (hose) | Leave the detail out (no hose) or compare it to something ("as thin as a phone cable") |
| Tool held wrong | "Holds it ONLY by the black-and-blue handle; fingers never touch the mop head" |
| Face drifts on long clips | Split the audio into ~7 s pieces and generate shorter clips |
| Lips out of sync | Trim the silence at the start of the audio file |
