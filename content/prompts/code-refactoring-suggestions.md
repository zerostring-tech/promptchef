---
title: "Code Refactoring Suggestions"
date: 2024-01-15
description: "Analyze code and suggest refactoring improvements focused on readability, maintainability, and clean design principles."
categories: ["programming", "code-quality"]
tags: ["refactoring", "clean-code", "best-practices"]
models: ["claude-3", "gpt-4"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Help developers improve existing code by identifying refactoring opportunities that enhance readability, structure, and maintainability without changing functional behavior.

## The Prompt

```
Review the following code and suggest refactoring improvements focused on readability and maintainability.

Code:
{{code}}

Evaluate the code specifically on:

- Naming of variables, functions, and classes
- Function length and responsibility (Single Responsibility Principle)
- Code structure and logical flow
- Duplication and opportunities for abstraction
- Comment quality (missing, redundant, or misleading comments)
- Consistency in formatting and style

For each suggestion:
- Clearly explain why the change improves readability or maintainability
- Provide before/after code snippets where helpful
- Ensure behavior and output remain functionally identical unless explicitly stated

Guidelines:
- Avoid performance micro-optimizations unless they also improve clarity
- Focus on clean code principles over stylistic preferences
- Prioritize practical, actionable improvements
```

## Variables

| Variable   | Description           | Example                          |
| ---------- | --------------------- | -------------------------------- |
| `{{code}}` | Source code to review | "function calc(a,b){return a+b}" |



## Usage Tips

- Works best when code is reasonably self-contained (functions, classes, modules).
- You can extend this prompt by adding a “language” variable for stricter style rules.
- Ideal for code review workflows, onboarding, or learning clean code practices.
- Combine with a follow-up prompt for “apply all refactorings automatically.”


