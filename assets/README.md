# Visual asset library

This folder tracks figures, diagrams, stock footage, AI-generated visuals, microscopy, lab material, and final exports used in the course.

GitHub should not be treated as the storage location for heavy raw footage. Use it for:

- asset metadata
- source URLs
- license and attribution records
- AI prompts
- lightweight web-ready images or SVGs
- final figures used directly in slides

## Folder logic

Suggested local working structure:

```text
assets/
  visual_asset_register.csv
  prompts/
  licenses/
  final/
  svg/
  thumbnails/
```

For large material, use external storage and record the location in the asset register:

```text
Drive / OneDrive / Dropbox / local archive / YouTube source / stock-library account
```

## Asset status categories

Use these values in the `scientific_status` column:

- `verified` — original data, original footage, or a scientifically reliable source
- `schematic` — simplified but scientifically controlled explanatory diagram
- `visual_metaphor` — concept illustration; not evidence
- `stock_broll` — generic footage or atmosphere
- `ai_background` — generated filler or transition material
- `needs_review` — not ready for publication
- `do_not_use` — rejected or legally/scientifically unsafe

## Minimum rule

No visual should enter an episode unless it has an entry in `visual_asset_register.csv` or is generated directly from version-controlled slide code.
