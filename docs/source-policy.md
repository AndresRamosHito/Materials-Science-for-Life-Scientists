# Source and licensing policy

This is a practical policy for using AI, online resources, open repositories, and stock video in the course.

## Source hierarchy

Preferred order for scientific visuals:

1. Original data, original microscopy, original lab footage, original field footage.
2. Open scientific or institutional repositories with clear reuse terms.
3. Open-access articles with explicit compatible licenses.
4. Wikimedia Commons or similar repositories, checked file by file.
5. Paid stock, when the footage is generic and non-scientific.
6. AI-generated visuals, only as schematic/metaphoric/non-evidentiary material.

## Commercial caution

The course may eventually be monetised through YouTube, Patreon, consulting, workshops, or institutional teaching. Therefore, avoid assuming that `educational use` means unrestricted reuse.

For every external asset, record:

- license name
- source URL
- creator
- whether commercial use is allowed
- whether attribution is required
- whether derivatives/modifications are allowed
- any special restrictions

## Open resources: practical notes

### Wikimedia Commons

Useful for biodiversity, anatomy, historical instruments, and general scientific images. Check each file individually because licenses vary.

### NASA

Useful for earth systems, materials in extreme environments, and space/planetary context. Still check use restrictions, especially logos, endorsement, and identifiable people.

### Pexels and Pixabay

Useful for generic b-roll and backgrounds. They are not scientific sources. Use for atmosphere, not evidence.

### Scientific articles

Only reuse figures when license terms permit it. A paper being open-access does not automatically mean every figure is safe for course reuse. Some figures may contain third-party material.

### BioRender and similar services

Useful for constructing clean diagrams. Check the exact plan/license before using figures in monetised course material or public repositories.

### AI image/video generators

Use when the purpose is visual scaffolding, metaphor, or style. Keep prompts and model/source notes in `assets/prompts/` or the asset register.

## Do not use without special review

- images scraped from random blogs
- screenshots from papers without a compatible license
- figures from textbooks
- identifiable people in stock footage unless model release status is clear
- trademark-heavy footage or images
- AI images of specific species used as taxonomic reference
- AI microscopy or AI-generated material microstructures presented as real
- copyrighted diagrams redrawn too closely from a source without permission

## Attribution format

When attribution is required, store it in the register in a ready-to-paste form:

```text
Creator, Title, Source, License, URL
```

Example:

```text
Jane Doe, "Cellulose fibres", Wikimedia Commons, CC BY-SA 4.0, [URL]
```

## Scientific review rule

Every figure should be reviewed according to its role:

- `verified`: factual accuracy and source/license checked
- `schematic`: mechanism simplified but not wrong
- `visual_metaphor`: not likely to be mistaken for literal evidence
- `stock_broll`: does not imply a false process, place, scale, or species
- `ai_background`: visually useful and non-misleading

## Bilingual rule

Prefer text-free base visuals. Labels should be added in the slide layer, not baked into images.

For final exports:

```text
*_base.png      # no labels
*_en.svg        # English labels
*_es.svg        # Spanish labels
```

## Repository rule

Do not commit large raw assets unless necessary. Keep large media in external storage and commit:

- manifests
- prompt files
- small thumbnails
- final compressed slide assets
- SVGs
- CSV license records
