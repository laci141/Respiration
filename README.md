# Respiration

Interactive breathing app in **4 languages** (HU · RO · DE · EN). A single HTML file, no build step, no dependencies, no tracking.

**Live:** https://laci141.github.io/Respiration/

---

## What it does

**Guided practice** — 10 breathing techniques with an animated timer. A soft glowing orb expands on the inhale and contracts on the exhale, and each phase has its own colour. Tap the orb to start or pause; it resumes exactly where it stopped.

**Mind map** — the journey of air through the body in 11 stations, from the nose to the mitochondrion and back. Every station opens a panel with a hand-drawn anatomical diagram, the science, key figures, and the link back to the breathing exercises.

## The 10 techniques

| Technique | Pattern | Best time |
|---|---|---|
| Box breathing | 4·4·4·4 | any time |
| 4-7-8 | 4·7·8 | morning, evening |
| Belly breathing | 4·6 | any time |
| Coherent breathing | 5.5·5.5 | any time |
| Alternate nostril | nadi shodhana | morning, evening |
| Ujjayi (ocean breath) | 5·5 | daytime |
| Bee breath | bhramari | evening |
| Kapalabhati (breath of fire) | 20 pumps × 3 | morning only |
| Tummo (inner fire) | 15 + hold × 3 | morning only |
| Wim Hof | 30 + hold × 3 | morning only |

## Colour schemes

Three pastel palettes, all on a warm background, switchable in-app. Each assigns a distinct colour to the four phases (inhale · hold full · exhale · hold empty).

- **Sunset** — apricot `#F3C6A0` · rose `#E2A9AF` · sage `#A9C4A5` · lavender `#C0B3CC`
- **Sage and linen** — `#AFC9B9` · `#D8CEB5` · `#C3B9CE` · `#B1BDC5`
- **Candlelight** — `#F6D2A4` · `#DE9F86` · `#C4837E` · `#A38879` — near-zero blue light, best for evening use

## Running it

Open `index.html` in any browser. That is the whole thing.

## Structure

Everything lives in `index.html`: CSS, the SVG diagrams, the breathing engine and all four language packs. Language-independent data (timings, colours, geometry, figures) is stored once in `META`, `SMETA` and `DIA`; only the text lives in the per-language `L` object, so adding a fifth language means adding one more block.

## Sources

Physiological figures are drawn from standard respiratory-physiology references (StatPearls, OpenStax, Britannica, MSD Manual) and from the primary literature on nasal nitric oxide (Lundberg), slow-breathing vagal effects (Gerritsen & Band; Noble & Hochman), and tummo thermogenesis (Benson et al., 1982).

## Disclaimer

This is educational material, not medical advice. Breath-holding and rapid-breathing techniques carry real risks — never practise them in or near water, while driving, or standing. If you have cardiovascular disease, lung disease, epilepsy, or you are pregnant, talk to your doctor first.

## Licence

MIT — see `LICENSE`.
