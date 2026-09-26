# PULL BACK — a scroll film for Crystals World

**Logline.** We open inside one amethyst. As the visitor scrolls, the camera pulls back steadily: the stone is resting in someone's palm, the palm is at the counter, the counter is at the end of an aisle full of crystals, and the aisle is inside a little shop under a purple sign on Guadalupe Street. The last frame is the storefront, which hands straight off to "Get directions".

**The one rule of this film:** *the camera only ever pulls back.* Never forward, never sideways. Each clip picks up exactly where the last one ended.

**Runtime:** 6 keyframes → 5 clips × 5 s = 25 s. 16:9, 1080p or higher, **audio off**.

| Chapter (scroll) | Keyframes | What the visitor feels |
|---|---|---|
| I. The stone | KF1 → KF2 | Mystery: something beautiful, and you don't know what it is yet |
| II. The hand | KF2 → KF3 | Warmth: someone chose it |
| III. The shelves | KF3 → KF4 | Abundance: there are hundreds more |
| IV. The door | KF4 → KF5 | Arrival: this is a real place |
| V. Guadalupe St | KF5 → KF6 | Invitation: come find yours |

---

## Continuity bible (keep identical in every prompt)

- **The stone (our protagonist).** A single natural amethyst point about 7 cm tall. Deep violet base fading to pale lavender at the tip, one small chipped edge on its left facet, a faint white phantom line inside.
- **The hands.** One pair of natural, unadorned hands: no rings, no nail polish, the same skin tone in every frame. Sleeves of a charcoal knit sweater. We never see a face.
- **The room.** A narrow shop in the evening. White shelving down both walls, glass display cases, a glass counter at the back, warm-white shop light (about 3500K). Outside is night.
- **The accent.** A soft violet glow from the purple sign, strongest near the front door and faint deeper inside.

## Master style block (paste at the end of every image prompt)

> Photoreal commercial cinematography, shot on ARRI Alexa 35 with Cooke S7/i primes, shallow depth of field, gentle highlight roll-off (no blown-out whites), deep clean blacks, subtle fine film grain, natural colour, 16:9, no text, no logos, no watermark.

## Negative prompt (every image and every clip)

> text, letters, words, watermark, logo, extra fingers, deformed hands, jewelry on hands, faces, people in background, lens flare, white-out, bloom, overexposed, cartoon, 3D render, CGI look, plastic, oversaturated, fisheye, dutch angle, camera shake, cut, scene change

---

## How to generate (order matters)

1. **Make KF6 first, from the real storefront photo** (`site/img/storefront-night.jpg`). This anchors the whole film to the real shop.
   - AI will mangle the "CRYSTALS WORLD" lettering, so keep the image strength high enough that the sign stays as-is.
   - If the letters still come out garbled, tell me and I'll paste the real sign back in locally, for free.
2. **Then make KF1 → KF5 in order.** Give each one the previous keyframe as an image reference, so light, colour and the stone carry over.
   - From KF3 on, also add the real shop photos as references (`shop-counter.jpg`, `shop-shelves.jpg`, `shop-interior.jpg`), so the interior is *their* interior.
3. **Clips use first + last frame mode, 5 s each, audio off.** Clip 1 = KF1 → KF2, and so on.
4. **Chain rule:** the *start* frame of clip 2 is the **actual last frame of clip 1**, not KF2. The same goes for every clip after.
   - That is what makes the joins invisible.
   - Send me each clip as you go and I'll extract the exact last frame locally.
5. **Phones (optional):** once the 16:9 film is approved, repeat the same 6 keyframes at 9:16 for a phone version.

---

## Keyframe prompts (image generation)

### KF1 — Inside the stone
> Extreme macro, looking straight into the heart of a natural amethyst crystal so that the stone fills the entire frame edge to edge. Layered violet facets receding in depth, soft internal veils and a faint white phantom line crossing the lower third, tiny inclusions catching light like distant stars. One warm key light from the upper left glances across a facet edge; everything else falls into deep violet shadow. Abstract, hushed, jewel-like; the viewer should not yet know what they're looking at. Lens: 100 mm macro, focus on the phantom line, the rest melting into soft violet. The upper-left third is darker and calm, with negative space for a title. *[master style block]*

### KF2 — The stone in a palm
> Same amethyst point, same light, the camera now far enough back to see the whole crystal: a single natural amethyst point about 7 cm tall, deep violet base fading to pale lavender at the tip, a small chipped edge on its left facet, resting upright in an open cupped palm. The fingertips curve up softly out of focus at the frame edges. The warm key light from the upper left makes the tip glow lavender. Background is dark and indistinct with a hint of warm shop light far behind. Intimate, careful, reverent. Lens: 85 mm, focus on the stone. Keep the violet, the light direction and the black levels identical to the previous image. *[master style block]*

### KF3 — Two hands at the counter
> Same amethyst point, same hands, further back: two natural, unadorned cupped hands (charcoal knit sleeves at the wrists) holding the amethyst point just above a glass shop counter. The hands and stone sit at the centre of the frame, in focus. Behind them, softly defocused, glass display cases and white shelves hold crystal clusters (violet amethyst, clear quartz, honey-gold citrine) under warm-white shop light. No face; the frame crops above the forearms. Evening, calm, welcoming. Lens: 50 mm. Match the real shop's counter and cases from the reference photos. *[master style block]*

### KF4 — Down the aisle
> Same shop, further back: a symmetrical view down the length of a narrow crystal shop toward the glass counter at the back, where the same two hands hold the small amethyst point, now small at the exact centre of the frame. White shelving runs down both walls, and glass cases are packed with amethyst clusters and geodes, clear quartz points, citrine clusters, lapis and banded onyx pieces. Warm-white shop lighting (about 3500K), evenly bright, clean and organized. One-point perspective, eye level. Lens: 35 mm, deep focus. Match the real interior from the reference photos. *[master style block]*

### KF5 — The front door
> Same view down the aisle, further back again: the camera stands just inside the shop's front glass door, looking in. The dark metal frame of the open door and front window sits at the left and right edges of the frame, and a faint reflection of the night street shows in the glass. Beyond it the lit aisle recedes to the counter, where the tiny figure of the hands and the stone is barely visible at the centre. A soft violet glow from the sign above the entrance washes the top of the door frame. Interior lighting identical to the previous image. Lens: 28 mm. *[master style block]*

### KF6 — Guadalupe Street (build from the real storefront photo)
> Use the real Crystals World storefront photo as the base. Night, eye level, from the sidewalk directly in front of the shop: the full storefront with the glowing purple "CRYSTALS WORLD" sign above (keep the real sign exactly as it is), the lit interior visible through the glass door and windows, and the aisle of white shelves glowing warm inside. Wet-looking dark pavement reflects a little purple. Quiet street, no people. Framing: storefront centred, sign in the upper third, clean space at the sides for text. Lens: 24 mm. *[master style block]*

---

## Clip prompts (video: first + last frame, 5 s, audio off)

*(These pass the skill's direction check: every clip pulls back and none reverses.)*

**Clip 1 · KF1 → KF2** — One continuous slow backward dolly. The camera pulls back from deep inside the amethyst point: violet facets and inner veils recede, and the whole crystal point resolves, resting in an open cupped palm. The same warm key light from upper left throughout. One unbroken move, no cuts.

**Clip 2 · (end of clip 1) → KF3** — Continuing the same slow backward dolly, the camera keeps pulling back: the palm becomes two cupped hands holding the amethyst point above a glass counter, wrists and charcoal sleeves appearing at the frame edges, glass cases softly out of focus behind. Lighting unchanged. One unbroken move, no cuts.

**Clip 3 · (end of clip 2) → KF4** — Continuing the same slow backward dolly, the camera pulls back away from the counter along the aisle: the hands grow small at frame centre while white shelves and glass cases of amethyst, clear quartz and citrine clusters slide past on both sides. Constant warm-white shop lighting. One unbroken move, no cuts.

**Clip 4 · (end of clip 3) → KF5** — Continuing the same slow backward dolly, the camera keeps pulling back through the length of the shop to the front door: the aisle recedes, the dark frame of the glass door appears at the edges of the shot, and a faint purple glow from the sign above spills on the door frame. Interior lighting unchanged. One unbroken move, no cuts.

**Clip 5 · (end of clip 4) → KF6** — Continuing the same slow backward dolly, the camera pulls back out through the open glass door onto the night sidewalk and keeps retreating to reveal the whole storefront under the glowing purple sign, the lit shop visible through the windows. Steady, one unbroken move, no cuts.

---

## Where it breaks (and the fix)

- **Clip 5 (inside → street)** is the riskiest: the location and the light both change.
  - The glass door is kept in frame at both ends and the interior lighting never changes, which is what makes it survivable.
  - If it still jumps, add **KF5b**: the camera on the threshold, half inside and half outside. Then split the move into two clips.
- **The hands drifting between clips.** If they change skin tone or gain rings, regenerate that keyframe with the previous one as a stronger reference before making the clip.
- **The stone changing shape.** Its chipped left facet and pale tip are the tell. If they vanish, the chain has drifted.

## Page copy mapping (the words say what the pictures can't)

- **I. The stone:** "Crystals World" wordmark and the address.
- **II. The hand:** "Every large piece is the only one."
- **III. The shelves:** 5.0 ★ from 203 Google reviews.
- **IV. The door:** "Retail and wholesale. Ships worldwide."
- **V. Guadalupe St:** "Come find the one that's yours." → **Get directions**.
