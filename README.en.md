# Xieyuan Skills

#### A personal collection of AI Skills and Prompts

![License](https://img.shields.io/badge/license-MIT-blue)
![Skills](https://img.shields.io/badge/skills-0-lightgrey)
![Prompts](https://img.shields.io/badge/prompts-0-lightgrey)
![AgentSkills](https://img.shields.io/badge/AgentSkills-compatible-brightgreen)
![Claude Code](https://img.shields.io/badge/Claude_Code-supported-black)
![Codex](https://img.shields.io/badge/Codex-supported-black)

[中文](README.md) · English

This repository is a personal collection of AI Skills and Prompts.

Skills are structured instruction sets that agents can load directly. They are useful for stable and repeatable workflows.

Prompts are lightweight instructions that can be copied into ChatGPT, Claude, Gemini, and other chat interfaces.

## Contents

### Skills

| Name | Summary | Notes |
| --- | --- | --- |
| Coming soon | Personal skills will be added here after they are tested in real use | TBD |

### Prompts

| Name | Summary | Notes |
| --- | --- | --- |
| Coming soon | Reusable prompts will be added here | TBD |

## Installation

In Claude Code, Codex, OpenCode, OpenClaw, or another agent that supports Skills, say:

```text
Install this skill: https://github.com/qxiu539/xieyuan-skills/tree/main/<skill-name>
```

Replace `<skill-name>` with the skill directory name.

## Skills

### Coming soon

Each skill section will include its use cases, trigger phrases, and a link to `SKILL.md`.

Recommended skill layout:

```text
weekly-review/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
├── scripts/
└── assets/
```

## Prompts

### Coming soon

Prompt files should live in `prompts/`.

## Adding A Skill

Copy `templates/skill/`, rename it to the real skill name, and place it at the repository root.

Use lowercase kebab-case names, such as `weekly-review`, `writing-style`, or `research-helper`.

Keep `name` and `description` in the `SKILL.md` frontmatter. Agents use these fields to decide when the skill applies.

Use `references/` for long reference materials, `scripts/` for deterministic code, and `assets/` for templates or media files.

## About

This repository prioritizes workflows that have been tested in real personal use.

[MIT License](LICENSE)

Made by [@qxiu539](https://github.com/qxiu539)
