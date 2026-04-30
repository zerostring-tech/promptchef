---
title: "Legal Document Summarizer"
date: 2026-03-14
description: "Summarize complex legal documents into clear, plain language with key obligations, rights, risks, and actionable insights."
categories: ["legal", "productivity"]
tags: ["legal", "summarization", "contracts"]
models: ["claude", "gpt"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Help users quickly understand legal documents by converting complex legal language into simple, structured, and actionable summaries. Ideal for non-lawyers reviewing contracts, agreements, or policies.

## The Prompt

```
Summarize the following legal document in plain, easy-to-understand language for a non-lawyer audience.

Requirements:
- Explain the document’s purpose and who it applies to
- Break down the main sections in simple terms
- Highlight and define key terms (e.g., obligations, rights, penalties, timelines)
- Clearly state:
  - What someone must do
  - What they can do
  - What they cannot do
- Call out any risks, consequences, or important deadlines

Formatting:
- Use short paragraphs or bullet points
- Bold key terms and important phrases
- Avoid legal jargon where possible (or explain it plainly if unavoidable)

End with:
- A brief “What this means for you” section
- A short disclaimer that this is not legal advice

Document:
{{document}}
```

## Variables

| Variable       | Description                 | Example                             |
| -------------- | --------------------------- | ----------------------------------- |
| `{{document}}` | The legal text to summarize | "This Agreement is made between..." |

## Usage Tips

- Works best with contracts, terms of service, NDAs, and policy documents.
- If the document is very long, summarize section-by-section for better clarity.
- You can extend this by adding “jurisdiction” for more context-specific summaries.
- Always validate important legal decisions with a qualified professional.


