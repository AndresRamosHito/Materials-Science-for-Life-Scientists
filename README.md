# Materials Science for Life Scientists

Repository for the bilingual course **Materials Science for Life Scientists / Ciencia de Materiales para Biólogos**.

This repository is intended to hold the written course structure, scripts, slide source files, reusable diagrams, visual asset documentation, and licensing records. Large raw video, microscopy, and stock footage should normally live outside GitHub, with this repository storing manifests, notes, prompts, and final lightweight web-ready exports.

## Working production model

The course is designed as a hybrid lecture-and-video format:

- slide-based explanation, diagrams, typography, animation, microscopy, and data visualisation
- inserted video segments: field footage, lab demonstrations, stock footage, microscopy in motion, and short AI-generated conceptual sequences
- bilingual delivery: English and Spanish treated as parallel first-class products rather than one primary version plus a late translation

## Repository structure

```text
assets/
  visual_asset_register.csv       # Master tracking sheet for all figures, footage, AI images, and stock assets
  README.md                       # How to use the visual asset system
  prompts/                        # Reusable AI figure and video prompts
  licenses/                       # License notes, attribution text, and source records

docs/
  visual-asset-system.md          # Full visual supply-chain policy
  source-policy.md                # Practical source and licensing rules

episodes/
  README.md                       # Episode planning and asset checklist
```

## Core visual principle

AI gives volume. Stock video gives motion. Open repositories give breadth. Original data and footage give authority.

Scientific claims should be supported by verified primary material: original data, your own footage/microscopy, open licensed scientific images, or properly cited literature. AI-generated visuals should be treated as schematics, metaphors, or design scaffolds unless manually verified and rebuilt.

## Immediate workflow

1. Plan the episode.
2. List every needed visual in `assets/visual_asset_register.csv`.
3. Mark each asset as one of: `verified`, `schematic`, `visual_metaphor`, `stock_broll`, `ai_background`, `needs_review`, or `do_not_use`.
4. Generate or collect visuals.
5. Store license/source details before using the asset.
6. Add final labels manually in the slide system, especially for bilingual figures.
