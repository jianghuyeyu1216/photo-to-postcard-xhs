# Photo to Zine Postcard

Turn your own photographs into minimal editorial zine-style postcards with ChatGPT.

The project provides a reusable `SKILL.md` specification that defines how to transform a photo into a coordinated postcard set:

- **Front**: original photo embedded at the top, preserved aspect ratio, quiet frame, large whitespace, source-derived hand-drawn editorial motif, and subtle color language.
- **Back**: matching postcard layout with stamp area, divider, address lines, and writing space.

## Quick Start

1. Give ChatGPT this repository or upload `SKILL.md`.
2. Upload your photo.
3. Ask ChatGPT:

```text
Please read SKILL.md from this repository and follow it as the only design specification.
Generate a Photo to Zine Postcard front and back from my uploaded photo.
```

If repository access is unavailable, simply upload `SKILL.md` together with your image.

## Design Philosophy

Photo to Zine Postcard follows four principles:

1. Keep the original photograph as the visual anchor.
2. Use generous whitespace instead of filling the page.
3. Extract one strong visual motif from the photograph.
4. Reinterpret that motif carefully with a restrained editorial / hand-crafted feeling.

The goal is not a generic AI poster. It is a printable personal postcard system.

## Customization

The repository is designed for forking and modification.

You can customize:

- illustration style
- paper texture
- typography
- postcard ratio
- metadata layout
- front/back composition
- motif extraction strategy

## Repository Structure

```text
photo-to-zine-postcard/
├── SKILL.md
├── README.md
├── CHANGELOG.md
├── LICENSE
├── docs/
│   └── CUSTOMIZATION.md
├── examples/
└── assets/
```

## Current Version

`v1.0.0`

Initial public release of the Photo to Zine Postcard skill.

## License

MIT License
