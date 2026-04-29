---
title: "About PromptChef"
description: "A community-driven library of AI prompts and skills, created and maintained by ZeroString Tech Ventures."
date: 2024-01-01
layout: about
draft: false
---

## What is PromptChef?

PromptChef is a free, open-source library of AI prompts and skills maintained by the community on GitHub. Every prompt and skill is a plain markdown file — no accounts, no paywalls, no lock-in.

The goal is simple: make high-quality prompts and skills easy to find, copy, and contribute to.

## How to Contribute

Adding a prompt or skill is as easy as creating a markdown file and opening a pull request — no coding knowledge needed.

Each prompt lives in `content/prompts/` as a single markdown file. Use the following structure:

```markdown
---
title: "Your Prompt Title"
date: 2024-01-01
description: "One sentence describing what this prompt does."
categories: ["writing"]
tags: ["tag1", "tag2"]
models: ["claude-3", "gpt-4"]
author: "your-github-username"
license: "CC BY 4.0"
source: ""
difficulty: "beginner"   # beginner | intermediate | advanced
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

Each skill lives in `content/skills/` as a single markdown file. Skills describe prompting techniques and patterns rather than task-specific prompts.

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
difficulty: "beginner"   # beginner | intermediate | advanced
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


Read the [Contribution Guide](https://github.com/zerostring-tech/promptchef/blob/main/CONTRIBUTING.md) to get started.

## License

The PromptChef platform code built with Hugo and is licensed under the [MIT License](https://github.com/zerostring-tech/promptchef/blob/main/LICENSE).

Individual prompts and skills carry their own license as specified in the `license` field on each page. 

## About ZeroString Tech Ventures

PromptChef is created and maintained by **[ZeroString Tech Ventures](https://zerostring.tech)** as an open community project.  