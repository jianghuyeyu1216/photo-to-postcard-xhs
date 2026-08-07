---
name: photo-to-zine-postcard
description: Turn a user-provided photograph into a minimal two-sided 2:3 zine-style postcard. Preserve the original photo above, then create a sparse hand-drawn source-specific motif, minimal metadata, three sampled color swatches, and a matching functional postcard back.
---

# Photo to Zine Postcard

**Release:** v1.0.0  
**Design spec:** v3.3

This skill is fully self-contained. Use only the rules in this document. Do not retrieve or reference external style skills.

## Goal

Generate two coordinated images from one source photograph:

1. **Front** — original photo embedded above, minimal editorial composition below.
2. **Back** — unified, functional postcard back.

The design must remain minimal, airy, source-specific, visually attractive, lightly hand-crafted, and print-friendly. The source photo remains primary; the lower area contains one strong visual motif rather than a collection of samples.

## Default format

- card ratio: portrait `2:3`
- reference print size: `100 × 150 mm` / `4 × 6 in`
- background: warm off-white / ivory paper
- texture: very subtle paper grain
- original photo: embedded directly
- lower fragment style: `hand_drawn_first`
- color palette: enabled by default

## Fixed front structure

Do not redesign the overall layout. Use this structure:

1. original photo in the upper area
2. generous blank transition space
3. metadata block on the lower left
4. one large main visual motif on the lower right
5. optional one much smaller supporting motif
6. exactly three small color swatches near the lower area

Do not add other visual modules.

## Main photo

- Use the actual source photo.
- Preserve its exact original aspect ratio.
- Do not stretch, repaint, replace, or crop it by default.
- Place it in the upper half, centered horizontally.
- Add a very thin frame.
- Leave a small even paper gap between photo and frame.
- At most one tiny archival tape detail is allowed.

## Main motif selection

Select the **most visually attractive and source-defining motif**, not merely the easiest object to isolate.

Prioritize the strongest combination of:

1. distinctive source identity
2. visually appealing color
3. clear silhouette
4. strong contrast
5. elegant shape
6. relevance to the overall photograph

Prefer dominant visual features such as vivid water forms, illuminated ridges, expressive plant clusters, recognizable window-and-vine structures, elegant architecture, strong clouds, or distinctive shadows.

Avoid dull neutral fragments when a stronger colored subject exists. Do not choose visually insignificant debris simply because it is easy to isolate.

When the source contains a clearly dominant color feature, the main motif should normally come from that feature.

Examples:

- turquoise lake → turquoise water / shoreline motif
- mountain sunset → illuminated ridge or sky-lit peak
- ivy window → window + vine cluster
- flower close-up → flower, not pot or background

## Hand-drawn-first rule

The main motif should be hand-drawn by default whenever the subject is suitable.

Use a restrained editorial illustration treatment such as:

- watercolor
- gouache
- ink
- pencil
- cut-paper illustration
- painted contour
- soft hand-rendered texture

The result must preserve the original silhouette, major internal structure, recognizable identity, and source color character. It should feel more lively than a raw crop while remaining controlled and clearly derived from the source photograph.

Good hand-drawn candidates include water shapes, shorelines, islands, mountains, plants, branches, windows, clouds, rocks, simple buildings, facades, and natural contours.

Do **not** use a raw crop as the main motif when the motif is suitable for hand drawing.

### Crop fallback

Use a source crop only when exact fidelity is important, such as faces, hands, text/signage, precise machinery, complex perspective, dense repeated detail, or objects that lose identity when simplified.

When using crop fallback, keep it lightly softened and integrated with the paper.

## Main motif size and placement

Recommended size:

- width: approximately `28%–38%` of card width
- height: approximately `14%–22%` of card height

Placement:

- lower right
- lower center-right

The motif must remain subordinate to the main photo but should feel intentional and substantial.

## Supporting motif

Optional only:

- one supporting motif maximum
- approximately `20%–35%` of the main motif size
- placed close to the main motif
- must support the same visual story
- never equal in size to the main motif

## Color swatches

Color swatches are enabled by default.

Use exactly **three small swatches** sampled from the source photo:

1. dominant color
2. dark structural color
3. pale neutral or accent color

Rules:

- small and secondary
- simple painted squares or restrained swatches
- no texture sample cards
- no large palette strip
- no more than three
- never replace the main motif

## Metadata

Allowed text only:

- title
- optional short subtitle
- `LOCATION`
- `DATE`
- small index number

Keep metadata compact on the lower left.

Do not invent values such as `Unknown` or `Undated`. Leave location and date blank when the user did not provide them.

Do not add keyword lists, descriptive paragraphs, multiple labels, or long captions.

## Forbidden front elements

Do not add:

- rows of multiple cutouts
- multiple main motifs
- texture sample boxes
- material sample cards
- image sample grids
- large color blocks
- generic circles or decorative dots
- wave doodles
- badges, seals, or logos
- keyword lists
- long captions
- full-width lower compositions
- rounded card corners unless explicitly requested

If uncertain, simplify.

## Back

Generate a unified postcard back with:

- thin outer border
- one vertical divider slightly right of center
- stamp box in the upper-right
- 3 or 4 address lines on the right
- large blank message area on the left

Optional:

- small `POST CARD` text near upper-left
- tiny metadata or index near lower-left
- one extremely faint source-derived watermark

Do not add a large collage, large palette, decorative sample blocks, or anything that reduces writing space.

## Quality requirements

Target:

- highest detail quality
- sharp and clear rendering
- crisp edges
- refined hand-drawn texture
- clean paper texture
- low noise
- no blur
- no muddy watercolor
- no smudged edges
- suitable for later `4×` super-resolution upscaling

Quality requirements improve rendering only; they must not increase the number of visual elements.

## Priority order

Always follow this order:

1. original photo embedded correctly
2. fixed minimal layout preserved
3. large white space preserved
4. choose the most visually attractive source-defining motif
5. use hand-drawn rendering when suitable
6. make the main motif large enough to read clearly
7. optional one small supporting motif
8. include exactly three small source-derived color swatches
9. minimal metadata
10. omit everything else

If any later rule conflicts with an earlier rule, keep the earlier rule.

## Front generation instruction

```text
Create a minimal portrait postcard front using the fixed Photo to Zine Postcard structure.

Use the actual source photo in the upper area. Preserve its exact original aspect ratio. Do not repaint, replace, stretch, or crop it unless cropping was explicitly requested. Center it horizontally, keep generous margins, add a very thin frame, and leave a small even paper gap between the photo and frame.

Keep a large blank transition area below the photo.

In the lower area, use:
- one compact metadata block on the lower left
- one large source-specific main motif on the lower right
- optionally one much smaller supporting motif near it
- exactly three small color swatches sampled from the source photo

Select the main motif based on visual attractiveness and source identity, not ease of extraction. Prefer the most distinctive color-rich and elegant feature in the image. When the source contains a dominant color feature, choose that feature as the main motif. Do not choose a dull neutral fragment when a stronger colored motif exists.

Render the main motif as a restrained hand-drawn editorial illustration whenever suitable. Preserve its original silhouette, major internal structure, identity, and source color character. Use controlled watercolor, gouache, ink, pencil, or cut-paper illustration treatment. Keep it clean, sharp, and clearly derived from the source photo.

Use a source crop only when exact fidelity is essential.

The main motif should occupy roughly 28% to 38% of the card width and remain subordinate to the photo.

Use exactly three tiny source-derived color swatches: dominant color, dark structural color, and pale neutral or accent color.

Add only:
- title
- optional short subtitle
- LOCATION
- DATE
- small index number

Leave location and date values blank if the user did not provide them.

Do not add keyword lists, sample boxes, rows of cutouts, image cards, generic circles, large color blocks, wave doodles, badges, seals, logos, or long text.

Use warm ivory paper with subtle grain.

Quality: highest detail quality, sharp and clear, crisp edges, refined hand-drawn texture, low noise, no blur, suitable for later 4× super-resolution upscaling.

Overall mood: minimal, airy, refined, source-specific, lightly hand-crafted, and collectible.
```

## Back generation instruction

```text
Create a matching unified postcard back using the same portrait 2:3 ratio, paper tone, thin-line style, and restrained visual language as the front.

Keep it functional and mostly blank.

Include:
- thin outer border
- one vertical divider slightly right of center
- stamp box in the upper-right
- 3 or 4 address lines on the right
- large blank message area on the left

Optionally add small POST CARD text near the upper-left and tiny metadata or index near the lower-left.

Do not add a large collage, palette, sample blocks, or decoration that reduces writing space.

Quality: clean sharp lines, refined paper texture, low noise, no blur, suitable for later 4× super-resolution upscaling.
```

## Quick checklist

### Front

- [ ] original photo embedded
- [ ] original aspect ratio preserved
- [ ] thin frame and even paper gap
- [ ] large whitespace remains
- [ ] main motif selected for visual attractiveness
- [ ] dominant color feature preferred
- [ ] hand-drawn style used when suitable
- [ ] main motif large enough
- [ ] at most one small supporting motif
- [ ] exactly three small color swatches
- [ ] no keyword list
- [ ] no sample boxes
- [ ] no decorative overload
- [ ] output sharp and high-detail

### Back

- [ ] unified functional layout
- [ ] writing space preserved
- [ ] no large collage
- [ ] output clean and sharp

## One-line definition

**Embed the original photo unchanged in the upper area of a 2:3 postcard, choose the most visually attractive source-defining motif below, render it as a large restrained hand-drawn editorial illustration when suitable, retain one optional supporting motif, include exactly three small source-derived color swatches, and pair it with a clean unified postcard back.**
