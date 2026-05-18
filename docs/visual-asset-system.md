# Visual asset system

This document defines how the course should use AI, online resources, open repositories, stock video, and original media as a constant source of figures and visual material.

## Core principle

Use different visual sources for different epistemic roles.

| Role | Best source | Use case | Risk |
|---|---|---|---|
| Scientific evidence | original data, microscopy, lab footage, primary literature, verified open repositories | claims, anatomy, mechanisms, measurements | misinterpretation or licensing error |
| Schematic explanation | SVG, Slidev components, AI draft images, manually corrected diagrams | teaching diagrams and conceptual simplification | oversimplification |
| Atmosphere and pacing | stock video, original field footage, AI backgrounds | transitions, manufacturing scenes, lab/field ambience | generic or visually misleading footage |
| Visual metaphor | AI images, abstract animation, symbolic graphics | intuition-building | mistaken for evidence |

## The rule for AI

AI-generated visuals may be used for:

- abstract backgrounds
- short conceptual transitions
- text-free schematic drafts
- metaphor images
- layout ideation
- storyboard thumbnails
- impossible zooms that are explicitly illustrative

AI-generated visuals should not be used as:

- evidence for biological anatomy
- evidence for material microstructure
- taxonomic reference images
- microscopy substitutes
- data plots
- images of specific species unless manually checked against real references

## Text-free generation rule

Generate AI images without embedded text. Add all labels manually in the slide system.

Reasons:

1. AI text is unreliable.
2. The course is bilingual.
3. Labels need typographic consistency.
4. Scientific terminology must remain under human control.

## Visual categories

### 1. Verified scientific visual

A visual can be marked `verified` when it comes from:

- original course footage
- original lab data
- original microscopy
- a properly licensed source from a scientific institution
- an open-access paper or repository whose reuse terms are checked
- a diagram rebuilt from primary literature and reviewed for accuracy

### 2. Schematic visual

A schematic is acceptable when it simplifies a real mechanism but does not pretend to be literal.

Examples:

- stress-strain curve
- materials triangle
- hierarchy ladder
- polymer network cartoon
- fibre-reinforced composite diagram

### 3. Visual metaphor

A visual metaphor explains intuition, not evidence.

Examples:

- crack deflection represented as a branching path
- toughness represented by a fibre bridge
- self-healing gel represented by reconnecting network strands

### 4. Stock b-roll

Stock b-roll is appropriate for generic context:

- manufacturing
- laboratory ambience
- forests
- materials processing
- cleanrooms
- machining
- construction timber

Avoid stock footage when species identity, microscopic structure, or experimental detail matters.

## Per-episode visual workflow

1. Write the episode script outline.
2. Identify every figure and video segment required.
3. Enter every asset into `assets/visual_asset_register.csv`.
4. Decide whether each asset is evidence, schematic, b-roll, or metaphor.
5. Generate, collect, film, or build each asset.
6. Record source URL, license, attribution, and modification notes.
7. Review scientific accuracy.
8. Export final lightweight assets for slides.
9. Keep raw/heavy media outside GitHub and record storage location.

## Recommended production pipeline

```text
script.md
  -> visual shot list
  -> visual_asset_register.csv
  -> AI prompt / stock search / original filming / data plotting
  -> SVG or edited image
  -> Slidev deck
  -> rendered video
```

## Module-level strategy

| Module | Visual emphasis |
|---|---|
| 1. What is a material? | biological tissue visuals, materials triangle, simple analogies |
| 2. Hierarchy | nested-scale diagrams, microscopy, zoom animations |
| 3. Quantifying material performance | data plots, stress-strain animations, mechanical testing footage |
| 4. Manufacturing | stock footage and diagrams of processing routes |
| 5. Material evolution | phylogenetic and comparative diagrams |
| 6. Functional materials | responsive biological examples and actuation diagrams |
| 7. Methodology | instrument footage, method cards, sample preparation visuals |
| 8. Wood case study | timber/wood processing footage, wood anatomy diagrams |
| 9. Comparative materiomics | kingdom-by-kingdom material matrices |
| 10. Orchids | original Orchidarc footage, lab microscopy, original data |

## Naming convention

Use stable IDs:

```text
M01-E01-0001
M01-E01-0002
M02-E03-0004
```

Pattern:

```text
M[module]-E[episode]-[asset number]
```

Example file names:

```text
M01-E01-0002_materials_triangle_en.svg
M01-E01-0002_materials_triangle_es.svg
M02-E01-0001_hierarchy_ladder_base.png
M03-E01-0001_stress_strain_animation.mp4
```

## Review labels

Use these in the asset register:

- `verified`
- `schematic`
- `visual_metaphor`
- `stock_broll`
- `ai_background`
- `needs_review`
- `do_not_use`

## Minimum acceptance checklist

Before using a visual in an episode:

- [ ] It has an asset ID.
- [ ] It has a source or generation record.
- [ ] License status is known.
- [ ] Attribution text is recorded if needed.
- [ ] Scientific role is clear.
- [ ] Labels are editable and bilingual where relevant.
- [ ] It is not misleading at small YouTube-screen size.
