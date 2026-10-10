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

## Open questions

- Which design directions to explore.
- Whether the layout is strictly fixed, or whether key shape and side-button grouping can change.
