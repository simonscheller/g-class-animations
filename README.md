# Andes / G

A single-file scroll essay — a photographic field study of a Mercedes-Benz G-Class
crossing the central Andes, from the Salar de Uyuni to the cloud forest of Manú.

Four chapters, four animation ideas:

| Chapter         | Scene                                | Animation                                                                |
| --------------- | ------------------------------------ | ------------------------------------------------------------------------ |
| I · Salt        | Black G on the Salar de Uyuni        | Parallax media + word-mask title, line-grouped lede reveal               |
| II · Stone      | Pisac terraces → Cusco stone alley   | Pinned 180% scrub, clip-path slide between panels, type crossfade        |
| III · Color     | Vinicunca, the Rainbow Mountain      | Per-character variable-font weight/SOFT morph + clip-path image reveal   |
| IV · Green      | Manú cloud forest, mist on a green G | Pinned mist-lift, brightness scrub, line-grouped title reveal            |

## Stack

- Vanilla HTML / CSS / JS — no build step.
- [GSAP 3.12](https://gsap.com/) + [ScrollTrigger](https://gsap.com/scrolltrigger/) for scroll-driven animation.
- [Lenis 1.1](https://github.com/darkroomengineering/lenis) for smooth scrolling, bridged to ScrollTrigger.
- Typography: [Fraunces](https://fonts.google.com/specimen/Fraunces) (variable `opsz`, `wght`, `SOFT`) and [Newsreader](https://fonts.google.com/specimen/Newsreader).
- Respects `prefers-reduced-motion`: every pin, clip, and morph is short-circuited; the page reads as a static essay.

## Run

```sh
# any static server works
python3 -m http.server 8000
# open http://localhost:8000
```

No npm install. No bundler. One HTML file.

## Image assets

The demo expects five JPEGs in `assets/peru/`. Filenames are referenced directly
from the HTML; renaming them will break the page.

| File                   | Scene                                            |
| ---------------------- | ------------------------------------------------ |
| `01-salar.jpg`         | Black G on Salar de Uyuni, sunset reflection     |
| `02-sacred-valley.jpg` | White G aerial on the Pisac terraces             |
| `03-cusco.jpg`         | Burgundy G in a Cusco Inca-stone alley           |
| `04-vinicunca.jpg`     | Silver G at Vinicunca (Rainbow Mountain)         |
| `05-cloud-forest.jpg`  | Green G on a muddy road in the Manú cloud forest |

Target ≈ 2,400 px on the long edge, JPEG q82–88, sRGB.

## Keyboard

- `1` Cover · `2` Salt · `3` Stone · `4` Color · `5` Green

## License

© S. Scheller, 2026. All rights reserved.
