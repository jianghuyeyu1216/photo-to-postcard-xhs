# Photo to Zine Postcard

Turn your own photographs into minimal editorial zine-style postcards with ChatGPT.

The project provides a reusable `SKILL.md` specification that transforms one photo into a coordinated postcard set:

- **Front** — original photo embedded at the top, preserved aspect ratio, quiet frame, large whitespace, a source-derived hand-drawn editorial motif, and three sampled color swatches.
- **Back** — matching postcard layout with stamp area, divider, address lines, and writing space.

<p align="center">
  <img src="assets/gallery.webp" alt="Photo to Zine Postcard example gallery" width="720" />
</p>

The gallery above contains nine official examples covering forest, mountain, lake, aerial landscape, architecture, garden, and dusk scenes.

## Quick Start

1. Give ChatGPT this repository, or upload [`SKILL.md`](SKILL.md).
2. Upload a photo you took.
3. Ask ChatGPT:

```text
Please read SKILL.md from this repository and follow it as the only design specification.
Generate a Photo to Zine Postcard front and back from my uploaded photo.
```

If repository access is unavailable, simply download `SKILL.md` and upload it together with your image.

### 中文快速使用

1. 把这个仓库提供给 ChatGPT，或直接上传 [`SKILL.md`](SKILL.md)。
2. 上传一张你拍的照片。
3. 输入：

```text
请读取 SKILL.md，并把它作为唯一的设计规范。
把我上传的照片生成一套 Photo to Zine Postcard 明信片正反面。
```

## Design Philosophy

Photo to Zine Postcard follows five principles:

1. Keep the original photograph as the visual anchor.
2. Preserve its original aspect ratio.
3. Use generous whitespace instead of filling the page.
4. Choose one visually strong, source-defining motif.
5. Reinterpret that motif carefully with a restrained hand-drawn editorial feeling.

The goal is not a generic AI poster. It is a printable personal postcard system.

## Default Output

- portrait `2:3`
- reference size `100 × 150 mm / 4 × 6 in`
- warm ivory paper
- embedded original photograph
- one main hand-drawn source motif
- optional one supporting motif
- exactly three source-derived color swatches
- matching functional postcard back

## Customize Your Own Version

The repository is designed for forking and modification.

You can customize:

- illustration style
- paper texture
- typography
- postcard ratio
- metadata layout
- front/back composition
- motif extraction strategy

See [`docs/CUSTOMIZATION.md`](docs/CUSTOMIZATION.md) for a practical guide. For major stylistic experiments, creating a variant is preferable to making the default skill more complicated.

## Official Examples

The current example set includes:

- Forest Homestead
- Alpine Glow
- Turquoise Lake
- Green Door
- Blue Arc Lake
- Turquoise Basin
- Lake at Dusk
- College Garden
- Valley Current

See [`examples/README.md`](examples/README.md) for the example index.

## Repository Structure

```text
photo-to-zine-postcard/
├── SKILL.md
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── docs/
│   └── CUSTOMIZATION.md
├── examples/
│   └── README.md
└── assets/
    ├── gallery.webp
    └── README.md
```

## Current Version

**v1.0.0** — first public release of the Photo to Zine Postcard skill.

The current version is optimized for ChatGPT image generation and for clean, detailed output suitable for later 4× super-resolution enlargement.

## Contributing

Pull requests and derivative styles are welcome. See [`CONTRIBUTING.md`](CONTRIBUTING.md).

## License

MIT License. See [`LICENSE`](LICENSE).
