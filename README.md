# monolink-skill

This repository contains the packaged `monolink-skill.zip` Codex skill.

The skill generates relation-first monochrome poetic collage photography prompts or images. It preserves the original MonoLink core idea: visual relationship comes before surface style.

The package uses this Codex skill structure:

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

- `SKILL.md`: core workflow, trigger metadata, relationship rules, prompt strategy, and failure checks.
- `agents/openai.yaml`: Codex UI metadata and the default `$monolink-skill` invocation prompt.
- `references/composition-grammar.md`: layout, boundary, negative space, and relationship placement guidance.
- `references/examples.md`: example relationship judgments and finished prompts.
- `references/prompt-template.md`: base and relationship-strengthened prompt templates.
- `references/relation-first-rules.md`: stricter relationship-first rules and inspection questions.
- `references/style-analysis.md`: monochrome photobook style, texture, subject language, and mood.

Install by extracting `monolink-skill.zip` into your Codex skills directory.
