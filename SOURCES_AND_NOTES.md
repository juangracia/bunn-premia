# BUNN Premia — sources and modeling notes

Created from scratch in Blender 5.2.1 for an independent “just for fun” product demo. The native scene contains editable components, packed artwork, lighting and separate hero/front studio scenes.

## Official references

- [BUNN Premia landing page](https://commercial.bunn.com/premia): overall asymmetric silhouette, large left service door, right-side hopper bank and dispensing layout. Saved as `official_hero.png`, `official_left.png` and `official_front.png`.
- [Official front photograph](https://res.cloudinary.com/bunn-assets/image/upload/v1/site-2/development/JPG/61000.0000_Premia_Straight.jpg): front proportions, hopper skirts, screen, three nozzle assemblies, curved stainless inserts, accessibility controls and drip grate. Saved as `catalog_straight.jpg`, with dedicated detail crops. The display, BUNN mark and keypad artwork use small crops of this reference.
- [Official hero photograph](https://res.cloudinary.com/bunn-assets/image/upload/v1/site-2/development/JPG/61000.0000_Premia_Hero.jpg) and [opposite three-quarter photograph](https://res.cloudinary.com/bunn-assets/image/upload/v1/site-2/development/JPG/61000.0000_Premia_Left.jpg): cabinet depth, side seams, hinges, hopper shape, side latch and labels. Saved as `catalog_hero.jpg` and `catalog_left.jpg`. Side label artwork was rectified from the latter. Side geometry was inferred from these views; no separate orthographic side photo was available.
- [Official 61000.0002 catalog page](https://commercial.bunn.com/61000.0002): nominal 33.5 × 26.4 × 24.4 in height/width/depth and stainless/black finish. An official specification PDF is also included.

All references were downloaded on 7 September 2026. Exact download URLs are recorded in `references/reference_urls.json`.

## Model and review

The cabinet, panels, hopper shells and dividers, individually creased coffee beans, lids, latches, controller, nozzles, curved steel covers, drip basin, individual grate wires, hinges, fasteners and feet are actual geometry. The GLB contains no full-machine photo billboard. Hidden mechanisms are omitted; rear details and small blue standby dots are approximations/demo additions.

Three preview-and-revision passes are preserved in `reviews/`. Final refinements corrected plastic visibility, steel curvature, lid edges, camera framing and the seamless front-view studio backdrop. Both final PNGs are 1800 × 1800.

The GLB is approximately **10.4 MB / 665,668 triangles**, with five embedded textures. It passes Khronos glTF validation with **zero errors and zero warnings**. It uses portable PBR materials and slightly stronger hopper transparency than the Blender render for browser readability.

`viewer.html` embeds the GLB and its viewer library. It was successfully tested through localhost, including the front and hopper controls. Direct file-URL launch testing was blocked by the browser tool’s URL policy; no external model or script download is required by the HTML.

This is a visual approximation, not service CAD or a BUNN-endorsed asset. BUNN/Premia marks and reference artwork remain their owners’ property. The viewer library license is included separately.
