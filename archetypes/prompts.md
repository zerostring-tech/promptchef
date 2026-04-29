---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: "A short description of what this prompt does"
categories: ["general"]
tags: []
models: ["gpt-4", "claude-3", "gemini"]
author: ""
license: "CC BY 4.0"
source: ""
difficulty: "beginner"   # beginner | intermediate | advanced
draft: false
---

## Purpose

Explain what problem this prompt solves or what task it helps with.

## The Prompt

```
Paste your prompt here.
```

## Variables

List any `{{placeholder}}` variables the user should replace:

| Variable | Description | Example |
|----------|-------------|---------|
| `{{topic}}` | The subject matter | "climate change" |

## Usage Tips

- Tip 1
- Tip 2

## Example Output

Show a sample response from an AI model using this prompt.
