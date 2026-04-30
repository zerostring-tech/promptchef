# PromptChef 🍳

A community-driven library of AI prompts and skills, free and open source.

**Live site:** https://zerostring-tech.github.io/promptchef/

---

## What is PromptChef?

PromptChef is a searchable library of AI prompts and skills maintained by the community on GitHub. Every prompt and skill is a plain markdown file — no accounts, no paywalls, no lock-in.

The goal is simple: make high-quality prompts and skills easy to find, copy, and contribute to.

---

## Contributing

Adding a prompt or skill is as easy as creating a markdown file and opening a pull request. No coding knowledge required.

### Adding a Prompt

Create a file at `content/prompts/your-prompt-name.md` using this structure:

```markdown
---
title: "Your Prompt Title"
date: 2024-01-01
description: "One sentence: what does this prompt do?"
categories: ["writing"]
tags: ["tag1", "tag2"]
models: ["claude-3", "gpt-4"]
author: "your-github-username"
license: "CC BY 4.0"
source: ""
difficulty: "beginner"
draft: false
---

## Purpose
...

## The Prompt
\```
Your prompt here. Use {{placeholders}} for variables.
\```

## Variables
| Variable | Description | Example |
|----------|-------------|---------|
| `{{placeholder}}` | What to replace | "example value" |

## Usage Tips
- ...
```

### Adding a Skill

Create a file at `content/skills/your-skill-name.md` using this structure:

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
source: ""
difficulty: "beginner"
draft: false
---

## Overview
...

## How It Works
...

## Prompt Template
\```
The skill prompt template here.
\```

## Example
...
```

### Guidelines

- Test your prompt with at least one model before submitting
- Keep descriptions specific — they power the search
- No personal data in example outputs
- If derived from another source, fill in the `source` field
- Always specify a `license` — if unknown, write `"Unknown"`

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide including categories and best practices.

---

## License

The PromptChef platform code is licensed under the [MIT License](LICENSE).

Individual prompts and skills carry their own license as specified in the `license` field on each page. When no license is stated, it defaults to unknown.

---

## About

PromptChef is created and maintained by [ZeroString Tech Ventures](https://zerostring.tech) as an open community project.
