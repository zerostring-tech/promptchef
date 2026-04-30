---
title: "Code Reviewer"
date: 2024-01-18
description: "Get a thorough code review covering bugs, security issues, performance, and style — as if from a senior engineer."
categories: ["coding", "engineering"]
tags: ["code-review", "debugging", "security", "performance", "engineering"]
models: ["claude-3", "gpt-4", "gemini-pro"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Simulate a senior engineer code review. The model will identify bugs, security vulnerabilities, performance issues, and style improvements in any language.

## The Prompt

```
You are a senior software engineer conducting a code review. Review the following {{language}} code and provide structured feedback.

```{{language}}
{{code}}
```

Evaluate the code across these dimensions:

1. **Correctness** – Are there bugs or logic errors?
2. **Security** – Any injection risks, exposed secrets, or unsafe operations?
3. **Performance** – Inefficient loops, N+1 queries, unnecessary allocations?
4. **Readability** – Naming, comments, complexity?
5. **Best practices** – Does it follow idiomatic {{language}} conventions?

For each issue found, provide:
- Severity: Critical / Major / Minor / Nitpick
- Location: line or function name
- Problem: what is wrong
- Fix: concrete code suggestion
```

## Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `{{language}}` | Programming language | "Python" |
| `{{code}}` | The code to review | paste your code here |

## Usage Tips

- Paste only the relevant function or class — models perform better on focused code blocks than entire files.
- For security-sensitive code (auth, payments), request a separate pass: "Focus only on security issues in the previous code."
- Add context: "This runs on user-supplied input from a public API" to get more targeted security feedback.

## Example Output

> **Review: Python login function**
>
> **Security – Critical** | Line 12 | SQL query uses string concatenation instead of parameterized query. Risk: SQL injection.
> Fix: `cursor.execute("SELECT * FROM users WHERE email = %s", (email,))`
>
> **Performance – Major** | Line 24 | Password compared with `==` instead of `hmac.compare_digest`. Risk: timing attack.
