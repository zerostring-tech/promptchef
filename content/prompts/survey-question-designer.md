---
title: "Survey Question Designer"
date: 2026-03-15
description: "Generate well-structured surveys with a mix of question types to collect meaningful and actionable feedback."
categories: ["research", "productivity"]
tags: ["survey", "feedback"]
models: ["claude", "gpt"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Help users design effective surveys that gather clear, actionable feedback. Useful for product teams, researchers, marketers, or anyone collecting structured insights.

## The Prompt

```
Design a survey to gather feedback about {{topic}}.

Target audience: {{audience}}
Goal of the survey: {{goal}} (e.g. improve product, measure satisfaction, validate idea)

Requirements:
- Include 10–15 questions
- Use a mix of question types:
  - Multiple choice
  - Likert scale (e.g. 1–5 rating)
  - Open-ended questions
- Ensure questions are clear, unbiased, and easy to answer
- Group questions logically (e.g. demographics, experience, feedback)

Optional:
- Add brief instructions or introduction for respondents
- Suggest how responses could be analyzed

Format the output in a clean, structured way.
```

## Variables

| Variable       | Description           | Example                                           |
| -------------- | --------------------- | ------------------------------------------------- |
| `{{topic}}`    | Subject of the survey | "user experience of a mobile banking app"         |
| `{{audience}}` | Target respondents    | "existing customers aged 25–45"                   |
| `{{goal}}`     | Purpose of the survey | "identify usability issues and improve retention" |



## Usage Tips

- Be specific with {{goal}} to get more targeted and useful questions.
- Keep the survey length reasonable to avoid drop-offs (10–12 is often ideal).
- Avoid leading or biased wording in questions.
- Pair this with a follow-up prompt to analyze survey responses.


