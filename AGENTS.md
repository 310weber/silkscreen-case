# Silkscreen e-reader: industrial design concepts

This repo holds industrial design concept work for the Silkscreen e-reader.
Record new instructions and decisions from the user in this file as they come up.

## Reference renders

The renders in `reference/` show the baseline device. Pass them to Painter as
references when generating concepts.

- `reference/front_left.png`: front view from the left, with orange, purple, green and red keys
- `reference/front_right.png`: front view from the right, with red, blue, yellow and pink keys
- `reference/front_right_usb_detail.png`: right-side detail showing the side buttons and USB-C port

## Baseline device

- **Body:** a portrait slab with large rounded corners and a deep profile with soft edges. The finish is warm off-white matte plastic or silicone.
- **Display:** an e-ink panel with a narrow bezel on the top and sides. The bezel is slightly recessed into the front face.
- **Chin:** a tall bottom chin, about 19% of the device height. The large "silkscreen" wordmark spans about 60% of the chin width and sits directly above the keys, raised tone-on-tone.
- **Front keys:** four colored keys in a row, together spanning about 75% of the bottom edge and centered on it.
  - Each key is a wide, short rectangle, about 3:1, with narrow gaps between keys of about a quarter of a key's width.
  - The keys are wedges: each has a slanted top, and its front protrudes past the bottom edge onto the bottom face.
- **Right side buttons:** three low-profile rectangular plates that protrude only slightly. Measured along the device length from the top end:
  - Button 1 runs from about 8% to 21%, so it is the longest.
  - Button 2 runs from about 30% to 40%.
  - Button 3 runs from about 42% to 51%, with only a small gap after button 2.
- **USB-C port:** on the right side at about 57–66% of the device length from the top end. Its long axis runs along the side. The last third of the side, nearest the bottom, is plain. Leave out the mic hole/pinhole that appears below the port in the reference renders.

## Concept rules

- Keep the layout of the buttons and the port the same across concepts unless the user says otherwise.
- Save draft images for the user to review under `.amp/in/artifacts/`.
- Once the user approves a concept, copy it to `concepts/` as `NN-name.png` and commit it.
- When a design language is developed further, it gets its own folder, `concepts/<language>/`, for example `concepts/retro/`. Number the files in it separately, starting from `01-<language>-baseline.png`.

## 3D printing constraints

Every concept must stay simple enough to 3D print on a consumer FDM printer. Check each concept against these rules before presenting it, and do not draw details that would break them.

- **Few parts:** a shell of two or three parts (for example, front bezel, back and buttons) that snap or screw together. Avoid inserts, overmolding and parts made of several materials.
- **Simple forms:** flat or gently curved faces, with constant fillets and chamfers. No compound curves, organic sculpting or thin fins.
- **Overhangs:** keep them at 45° or less from vertical in a sensible print orientation. Avoid undercuts that need support material, and use chamfers instead of fillets on edges that face the print bed.
- **Minimum feature sizes:**
  - Walls at least 1.6 mm thick.
  - Raised or debossed details, such as the wordmark and textures, at least 0.6 mm deep.
  - No lettering or ribs finer than about 1 mm.
- **Buttons:** separate printed parts with simple prismatic shapes. Include about 0.3 mm of clearance around each opening, and use simple guides or flexures rather than complex mechanisms.
- **Color and finish:** color comes from the filament of each part, such as colored keys in a different filament. Do not rely on paint, printed graphics or glossy finishes. A matte, slightly layered surface is acceptable.
- **Openings:** use simple rectangular or slotted cutouts for the screen window and the USB-C port.
- **Textures:** do not use raised dots, bumps or knurls, especially on vertical walls; the user rejected these as hard to print. Instead use:
  - Slicer "fuzzy skin" on the side walls, which needs no extra geometry.
  - A textured build plate for the face that prints against the bed.
  - Recessed V-grooves with 45° flanks, at least 1 mm wide and generously spaced.

## Sketch style

- Draw every sketch in the style of Koos Eissen and Roselien Steur, as in their books *Sketching* and *Sketching: The Basics*. That means:
  - Fine-liner or ballpoint linework on white paper, with light construction lines and ellipses left visible.
  - Varied line weight: heavier outlines on the silhouette and on edges facing away from the light, thinner lines inside.
  - Marker rendering in cool or warm greys, plus at most one or two accent colors, such as the colored keys.
  - White pencil or gouache highlights on edges and the screen, and a simple cast shadow under the device.
  - A loose, confident, hand-drawn look. It should not look like a CAD render or a photo.
- Show one hero view of the device per sketch, focused on the front-bottom-right corner. Use parallel projection, so parallel edges stay parallel.
  - That corner is nearest the viewer and sits low in the centre of the picture.
  - The front face's bottom edge (the short edge with the keys) recedes up and to the left at roughly 45°.
  - The front face's right edge (the long edge) recedes up and to the right at roughly 45°.
  - The screen face rises above the corner, as if the device is tipped back with the screen facing the viewer.
  - The bottom side face and the right side face show as thin bands below those two edges. The thickness edge at the corner points straight down.
  - The right side band shows the three side buttons on the half toward the top of the device, and the USB-C port on the half nearer the corner.
  - Keep the device portrait: the long edge is about 1.6 times the short edge, and the body is a slim slab.
- Keep the wordmark fully clear of the front keys, with its baseline parallel to the bottom edge.

## Concepts

- `concepts/01-minimalist-baseline.png` (approved): the baseline minimalist concept. One soft radius on the body, an off-white body, sage green keys and no extra decoration. The user confirmed its button and port layout is correct, so use it as the layout reference for later concepts.
- `concepts/02-cut-sheet-design-languages.png` (approved): a quick 2×2 cut sheet of four design languages. Its proportions are looser than the baseline (stubbier body, shorter chin, smaller keys). Fix those when developing any of them further.
  - **Soft:** a pillowy slab with large constant radii. Off-white body with pastel keys.
  - **Rugged:** a charcoal bumper frame with chamfered corner guards, a recessed screen, screw heads and side grip ribs. Mid-grey body with orange keys and side buttons.
  - **Angular:** moderate flat 45° chamfers, the same width on every edge, with flat corner facets. Light grey face, graphite chamfer bands and electric blue keys. The user rejected both narrower and much wider chamfers.
  - **Retro:** cream body with a chocolate-brown chin panel with grooves, and red, orange, mustard and brown keys.
- `concepts/03-cut-sheet-design-languages-2.png` (approved): a second 2×2 cut sheet. It has the same loose proportions as sheet 02, so fix them the same way when developing further.
  - **Bauhaus:** calm Braun-style geometry with small radii and flat dimpled keys. White body, with one signal orange key and three light grey keys.
  - **Bookish:** reads like a hardback. Page-edge grooves on the bottom and right faces, in a cream separate part, and a raised oxblood cover border. Keys in cream, tan, oxblood and brown.
  - **Sporty:** off-white body with a lime wrap-around grip band with ridges. The buttons and port pass through openings in the band, and there is a lanyard loop at the near corner. Charcoal keys.
  - **Tactile:** monochrome warm grey. Fuzzy-skin texture on the side faces, smooth around the buttons and port, and recessed V-grooves on either side of the wordmark. Slightly darker keys.

### Retro (`concepts/retro/`)

- `01-retro-baseline.png` (approved): the full hero sketch at baseline proportions and layout.
  - Cream shell with tight constant radii.
  - The whole chin is a separate chocolate-brown faceplate with a small chamfer, sitting flush. It carries a raised cream wordmark and a block of five recessed speaker-grille V-grooves to the right of the wordmark.
  - Thin brown stepped frame around a slightly recessed screen window.
  - Recessed brown pinstripe along the middle of the bottom and right side faces, broken around the buttons and port.
  - Chunky wedge keys in red, orange, mustard and brown, and chocolate-brown side buttons.
  - Printing has not been decided for the pinstripe: it could be a filled groove, a plain shadow groove or a filament color change between layers.

## Open questions

- Which of the eight design languages to develop into full sketches.
- Whether the layout is strictly fixed, or whether key shape and side-button grouping can change.
