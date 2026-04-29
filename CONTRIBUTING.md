# Contributing to PromptChef

Thank you for contributing! PromptChef is community-powered — every new prompt or skill is a markdown file. No coding knowledge required.

PromptChef is created and maintained by [ZeroString Tech Ventures](https://zerostring.tech).

## Quick start

1. **Fork** this repository
2. Create a new branch: `git checkout -b add/my-prompt-name`
3. Add your file (see below)
4. Open a **Pull Request** with a short description

---

## Adding a Prompt

Create a new file at `content/prompts/your-prompt-name.md`.
Use lowercase words separated by hyphens for the filename (e.g. `email-rewriter.md`).

Run the archetype generator (optional, requires Hugo installed):

```bash
hugo new prompts/your-prompt-name.md
```

Or copy the template below:

```markdown
---
title: "Your Prompt Title"
date: 2024-01-01
description: "One sentence: what does this prompt do?"
categories: ["writing"]           # pick one primary category
tags: ["tag1", "tag2"]            # 2–5 lowercase tags
models: ["claude-3", "gpt-4"]     # models you tested it with
author: "your-github-username"
license: "CC BY 4.0"              # license for this prompt
source: ""                        # original source URL if applicable
difficulty: "beginner"            # beginner | intermediate | advanced
draft: false
---

## Purpose

What problem does this prompt solve?

## The Prompt

\```
Your prompt text here. Use {{placeholders}} for variables.
\```

## Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `{{placeholder}}` | What to replace | "example value" |

## Usage Tips

- Tip one
- Tip two
```

---

## Adding a Skill

Skills describe prompting techniques and patterns (chain-of-thought, few-shot, role prompting, etc.) rather than task-specific prompts. The file goes in `content/skills/skill-name.md`.

```bash
hugo new skills/your-skill-name.md
```

Or copy the template below:

```markdown
---
title: "Your Skill Title"
date: 2024-01-01
description: "One sentence describing this technique."
categories: ["prompting-technique"]
tags: ["tag1", "tag2"]
models: ["claude-3", "gpt-4"]
author: "your-github-username"
license: "CC BY 4.0"
source: ""                        # original source URL if applicable
difficulty: "beginner"            # beginner | intermediate | advanced
draft: false
---

## Overview

What is this skill and when is it useful?

## How It Works

Explain the technique or concept.

## Prompt Template

\```
The skill prompt template here.
\```

## Example

A concrete before/after or input/output example.
```

---

## Guidelines

- **Test your prompt** with at least one model before submitting.
- **Be specific** in descriptions — helps users find the right prompt via search.
- **No personal data** in example outputs.
- **English only** for now (translations are a future milestone).
- Prompts should be general-purpose, not vendor-specific marketing.
- Always specify a `license` field. If the license is unknown or unclear, leave the field empty or write `"Unknown"`.
- If the prompt or skill is derived from another source, fill in the `source` field.

## Categories

Prompts and skills should use one of these primary categories:

| Category | Use for |
|----------|---------|
| `writing` | Blog posts, emails, copy, documentation |
| `coding` | Code generation, review, debugging |
| `research` | Summarization, analysis, literature review |
| `productivity` | Meetings, planning, task management |
| `education` | Tutoring, explanations, quizzes |
| `business` | Sales, marketing, HR, legal |
| `prompting-technique` | Meta-skills: CoT, few-shot, role prompting |
| `image` | Image generation prompts |
| `data` | Data analysis, SQL, spreadsheets |

## License

The PromptChef platform code is licensed under the [MIT License](https://github.com/zerostring-tech/promptchef/blob/main/LICENSE).

Individual prompts and skills carry their own license as specified in the `license` frontmatter field on each page. When no license is stated, content defaults to unknown.

## Questions?

Open an [issue](../../issues) or start a [discussion](../../discussions).
