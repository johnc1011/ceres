# scenes.md — slide1.html Animation Breakdown

12 scenes. Each pauses at its end — UFO appears top-center, press SPACE to continue.
All durations at 2× playback speed.

---

## Scene 1 — Sky Reveal
**~0.5s**

Black canvas fades to deep space gradient (`#07091c` top → `#020309` bottom). 600 stars appear with twinkling (warm orange, cool blue, white tints, varying sizes). Faint diagonal Milky Way band renders. Sun appears bottom-right with corona, radial glow, and 16 animated rays. Horizon silhouette (city/hill profile) at ~90% screen height in near-black.

Nothing disappears. Camera at default (1× zoom, unrotated, centred).

**Pauses:** sky and stars fully revealed.

---

## Scene 2 — Taurus Constellation + First Ceres Sighting
**~0.5s** *(begins during Scene 1)*

14 Taurus stars fade in with colour-accurate glows: Aldebaran large orange (`#FF9944`), Pleiades cluster in blue (`#88AAFF`), remainder warm white. 8 constellation lines connect them in dim blue (38% opacity).

Partway through (~0.25s in), the first Ceres observation dot appears as a yellow-gold point. A big red arrow fades in from upper-right pointing directly at it — flagging it as the discovery position.

Nothing disappears. No camera change.

**Pauses:** Taurus fully visible, dot 0 and discovery arrow at full opacity.

---

## Scene 3 — Subsequent Observations
**~1.5s**

Discovery arrow fades out over ~0.75s. Meanwhile the 18 remaining Ceres dots appear one by one, each extending the dashed gold trail from dot 0. Dots are yellow-gold (`#FFD060`). Final dot (obs 18) is larger and orange-red (`#FF6644`) — the last known position before loss.

Disappears: discovery arrow. Appears: 18 more dots, full trail.

**Pauses:** all 19 dots visible, trail complete.

---

## Scene 4 — Arrow Toward Sun
**~0.5s**

Orange dashed arrow (`#FF8844`) fades in from last Ceres dot, pointing straight at the Sun with an arrowhead just outside the solar disc. Represents Ceres' predicted path — heading behind the Sun and about to be lost to glare.

Trail and dots remain. No camera change.

**Pauses:** arrow fully opaque.

---

## Scene 5 — Solar Glare Expands
**~1s** *(begins slightly after Scene 4 starts)*

Sun's glare radius grows from 50% to 100% of full size. Stars within the inner glare zone disappear; stars in the transition zone fade proportionally. The bright wash around the Sun swells — Ceres vanishing into solar glare.

Stars near Sun disappear. Arrow and trail remain. No camera change.

**Pauses:** glare fully expanded.

---

## Scene 6 — Camera Zoom In
**~1.1s**

Camera zooms from 1× to 2.2×, focus shifts toward the Ceres trail area. Canvas rotates −5.7°. Horizon silhouette fades out (tied to zoom progress). Milky Way dims by 60%. Everything scales up with the zoom.

Disappears: horizon silhouette. Milky Way mostly gone.

**Pauses:** zoom and rotation complete.

---

## Scene 7 — Three Anchor Points Highlighted
**~0.5s**

Observations 0 (first), 9 (middle), and 18 (last) pulse brightly in cyan-white (`#CCFFFF`) with large glow halos (±18% sinusoidal pulse). All other Ceres dots dim to 50%. These three will be the anchors for the circumscribed-circle orbit estimate.

Other dots dim. No further camera change.

**Pauses:** anchors at full glow.

---

## Scene 8 — First Orbit Ellipse
**~1.25s**

Cyan-blue circle (`rgba(80,210,255,0.80)`, 2.5px, blue glow) sweeps in clockwise from the first anchor, completing a full revolution. This is the circumscribed circle through exactly the 3 highlighted observations — the simplest orbit estimate from Piazzi's chosen points.

Anchors and trail remain visible.

**Pauses:** circle fully drawn.

---

## Scene 9 — Error Lines Appear
**~1.25s**

Red lines (`#FF2222`, glow) fade in simultaneously from each of the 16 non-anchor dots to the nearest point on the blue circle — the residuals showing how far each observation deviates from the 3-point orbit.

Nothing disappears. Blue circle and anchors remain.

**Pauses:** all 16 error lines at full opacity.

---

## Scene 10 — Error Emphasis
**~1s**

Error lines thicken (3px → 5.5px) and glow intensifies (shadow blur 4 → 22px). Simultaneously, the cyan anchor highlights and blue ellipse fade out — attention shifts entirely to the large, dramatic errors.

Disappears: anchor highlights, blue ellipse.

**Pauses:** errors at maximum thickness/glow.

---

## Scene 11 — LSQ Ellipse Replaces Old Fit
**~1.75s**

Old blue ellipse and red error lines fade out completely in the first ~0.75s. Then a new green circle (`rgba(120,255,180,0.85)`, green glow) sweeps in clockwise from the leftmost to rightmost Ceres point — the least-squares best-fit circle through all 19 observations.

Disappears: old blue circle, old red lines. New: green LSQ circle.

**Pauses:** green circle fully drawn.

---

## Scene 12 — New Error Lines (All 19 Points)
**~1s**

Red error lines fade in for all 19 Ceres dots (including the 3 former anchors, excluded in Scene 9). Lines run from each dot to the nearest point on the green LSQ circle. Residuals are visibly smaller and more uniform — the LSQ fit minimises total squared error across all observations.

Final state: green LSQ circle + 19 red residuals + full gold trail.

**Pauses:** animation complete.
