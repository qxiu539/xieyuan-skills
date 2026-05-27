# Xieyuan Skills

#### 我自己常用的一些 AI Skills 和 Prompts，会慢慢整理到这里

![License](https://img.shields.io/badge/license-MIT-blue)
![Skills](https://img.shields.io/badge/skills-1-lightgrey)
![Prompts](https://img.shields.io/badge/prompts-0-lightgrey)
![AgentSkills](https://img.shields.io/badge/AgentSkills-compatible-brightgreen)
![Claude Code](https://img.shields.io/badge/Claude_Code-supported-black)
![Codex](https://img.shields.io/badge/Codex-supported-black)

中文 · [English](README.en.md)

这个仓库专门放我自己的 AI Skills 和 Prompt。

Skills 是 Agent 可以直接加载的结构化指令集，适合沉淀稳定、可重复使用的工作流。

Prompts 是可以直接复制到 ChatGPT、Claude、Gemini 等对话里的提示词，适合轻量使用。

## 目录

### Skills

| 名字 | 一句话 | 讲解 |
| --- | --- | --- |
| polish | 三遍审校文章并降低 AI 味，采用保守模式处理明确问题 | [SKILL.md](polish/SKILL.md) |

### Prompts

| 名字 | 一句话 | 讲解 |
| --- | --- | --- |
| 暂未添加 | 后续会把常用 prompt 放在这里 | 待补 |

## 安装方式

在 Claude Code、Codex、OpenCode、OpenClaw 等支持 Skill 的 Agent 里，可以直接说：

```text
帮我安装这个 skill：https://github.com/qxiu539/xieyuan-skills/tree/main/<skill-name>
```

把 `<skill-name>` 换成要安装的 skill 目录名。

## Skills

### polish

对文章进行三遍审校并降低 AI 味。适合直接粘贴文章，或提供文件路径后审校。

触发方式：`/polish`、帮我审校、降AI味、审校一下。

技能文件：[polish/SKILL.md](polish/SKILL.md)

每个 skill 建议直接放在仓库根目录，例如：

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

### 暂未添加

这里后续放 prompt 版能力。Prompt 文件建议放在 `prompts/` 目录下。

## 新增一个 Skill

复制 `templates/skill/`，改成真实 skill 名称，并放到仓库根目录。

目录名建议使用小写短横线格式，例如 `weekly-review`、`writing-style`、`research-helper`。

`SKILL.md` 顶部必须保留 `name` 和 `description`。这两个字段会影响 Agent 判断何时使用这个 skill。

如果 skill 需要长资料，放进 `references/`。如果需要稳定执行的代码，放进 `scripts/`。如果需要模板、图片、字体等素材，放进 `assets/`。

## 关于

这个仓库会优先放我自己真正使用过的 workflow。每个 skill 先保证能用，再考虑补充说明。

[MIT License](LICENSE) · 自由使用、修改和再分发

Made by [@qxiu539](https://github.com/qxiu539)
