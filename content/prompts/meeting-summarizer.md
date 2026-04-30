---
title: "Meeting Summarizer"
date: 2026-02-20
description: "Turn messy meeting notes or a transcript into a clean summary with decisions, action items, and owners."
categories: ["productivity", "business"]
tags: ["meetings", "productivity", "summarization", "action-items"]
models: ["claude", "gpt"]
author: "promptchef"
difficulty: "beginner" 
draft: false
---

## Purpose

Saves time after every meeting by extracting the key decisions and action items from raw notes or a transcript. Works with any meeting type: standup, planning, retrospective, sales call.

## The Prompt

```
Summarize the following meeting notes/transcript. Extract only the most important information.

Meeting type: {{meeting_type}}
Date: {{date}}
Participants: {{participants}}

---
{{transcript_or_notes}}
---

Produce output in this exact format:

## Summary (2-3 sentences)
...

## Key Decisions
- ...

## Action Items
| Owner | Task | Due Date |
|-------|------|----------|
| ...   | ...  | ...      |

## Open Questions
- ...

Keep the summary concise. If no due date is mentioned for an action item, write "TBD".
```

## Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `{{meeting_type}}` | Type of meeting | "Sprint planning" |
| `{{date}}` | Meeting date | "2024-01-20" |
| `{{participants}}` | Attendees list | "Alice (PM), Bob (Eng), Carol (Design)" |
| `{{transcript_or_notes}}` | Raw notes or transcript | paste here |

## Usage Tips

- Works great with auto-transcripts from Zoom, Google Meet, or Teams.
- If participants aren't mentioned by name in the notes, remove the `{{participants}}` variable.
- Chain with the **Blog Post Writer** prompt to turn key decisions into an internal announcement.
