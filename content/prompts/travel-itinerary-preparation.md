---
title: "Travel Itinerary Preparation Template"
date: 2026-02-15
description: "Generate a structured multi-day travel itinerary with daily plans, accommodation, transport, activities, and budget estimates."
categories: ["travel", "planning"]
tags: ["itinerary", "vacation", "writing", "budgeting"]
models: ["claude", "gpt"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Quickly generate a well-structured travel itinerary for any destination. Useful for travelers who want a clear day-by-day plan including logistics, accommodation, and budget considerations.

## The Prompt

```
Create a structured {{days}}-day travel itinerary for {{destination}}.

Traveler type: {{traveler_type}} (e.g. solo, couple, family)
Budget level: {{budget}} (e.g. low, mid-range, luxury)
Travel style: {{style}} (e.g. relaxed, adventurous, cultural)

The itinerary should include:
- A day-by-day schedule with morning, afternoon, and evening activities
- Recommended accommodation options or types
- Transportation planning (local travel and intercity if needed)
- Key sightseeing spots and experiences
- Estimated daily and total budget

Ensure the plan is practical, well-paced, and adaptable. 
```

## Variables

| Variable            | Description           | Example                |
| ------------------- | --------------------- | ---------------------- |
| `{{days}}`          | Number of travel days | "5"                    |
| `{{destination}}`   | Travel location       | "Bali, Indonesia"      |
| `{{traveler_type}}` | Type of traveler      | "couple"               |
| `{{budget}}`        | Budget preference     | "mid-range"            |
| `{{style}}`         | Travel preference     | "relaxed and cultural" |


## Usage Tips

- Be specific with {{destination}} to get better recommendations (e.g., "Kyoto" instead of "Japan").
- Adjust {{style}} to shape the itinerary—adventurous trips will include more activities, while relaxed ones will have downtime.
- You can extend the prompt by adding constraints like "vegetarian food only" or "kid-friendly activities."
- Always verify accommodation and transport details before booking.


