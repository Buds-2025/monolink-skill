# monolink-skill

`monolink-skill.zip` is a packaged Codex skill for generating monochrome poetic collage photography prompts or images.

The current version focuses on **cross-domain visual translation**: the main image and companion image must share a clear visual relationship, but they should not simply stay in the same subject, material, or scene category.

## Core Idea

The skill follows this priority:

1. Cross-domain translation first
2. Visual relationship second
3. Monochrome photobook style third

It is designed to avoid weak same-domain pairings such as:

- floral dress -> flower field
- swallows -> sky or clouds
- sunset road -> another road or road texture

Instead, it pushes pairings such as:

- floral dress -> moth wings, old map islands, mildew stains, star clusters
- swallows -> feather barbs, stitching, human silhouettes, music notation
- sunset road -> palm lines, blood vessels, river paths, film scratches

## Hard Rules

- The two images must cross at least two domains, preferably three: subject type, material, scale, scene system, or behavior.
- The relationship must remain visually readable through contour, direction, rhythm, structure, scale contrast, extension, or replacement.
- The white gutter between panels must stay completely clean. No subject, line, smoke, crack, shadow, petal, stroke, or visual bridge may enter or cross the gutter safety zone.
- Black-and-white grain, wide borders, dust, scratches, and quiet mood are only the outer style layer. They must not compensate for a weak relationship.

## Package Structure

```text
monolink-skill/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── composition-grammar.md
    ├── examples.md
    ├── prompt-template.md
    ├── relation-first-rules.md
    └── style-analysis.md
```

## Install

Extract `monolink-skill.zip` into your Codex skills directory.

The zip contains the complete skill folder and is the artifact intended for installation or sharing.

## Generated Output Naming

AI-generated images created for this project should be saved under `output/`.

Before naming, inspect each image and identify its actual theme. Use this filename format:

```text
YYYYMMDD-theme-##.png
```

- `YYYYMMDD`: generation or batch date, such as `20260525`
- `theme`: Chinese image theme, such as `思念`, `选择`, or `高兴`
- `##`: two-digit sequence number, such as `01`, `02`, `14`

Example: `20260525-思念-07.png`
