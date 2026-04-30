---
title: "7-Day Weight Loss Meal Plan"
date: 2024-01-15
description: "Generate a balanced 7-day meal plan for weight loss with calorie targets, daily meals, snacks, and a complete grocery list."
categories: ["health", "nutrition"]
tags: ["meal-plan", "weight-loss", "diet", "healthy-eating"]
models: ["claude-3", "gpt-4"]
author: "promptchef"
difficulty: "beginner"
draft: false
---

## Purpose

Create a structured weekly meal plan tailored for weight loss goals. Useful for individuals looking to maintain a calorie-controlled, balanced diet without manually planning meals.

## The Prompt

```
Create a {{days}}-day healthy meal plan for weight loss.

Profile:
- Age: {{age}}
- Gender: {{gender}}
- Daily calorie target: {{calories}}

Diet preferences: {{diet_type}} (e.g. vegetarian, keto, high-protein, no restrictions)
Allergies or restrictions: {{restrictions}}

The meal plan should include:
- Breakfast, lunch, dinner, and 1–2 snacks per day
- Approximate calories per meal
- Balanced macronutrients (protein, carbs, fats)
- Simple and practical recipes or meal ideas
- A categorized grocery list for the full week

Ensure meals are easy to prepare and suitable for a sustainable weight loss plan.
```

## Variables

| Variable           | Description                       | Example        |
| ------------------ | --------------------------------- | -------------- |
| `{{days}}`         | Duration of the plan              | "7"            |
| `{{age}}`          | Age of the individual             | "30"           |
| `{{gender}}`       | Gender                            | "female"       |
| `{{calories}}`     | Daily calorie intake              | "1800"         |
| `{{diet_type}}`    | Diet preference                   | "high-protein" |
| `{{restrictions}}` | Allergies or dietary restrictions | "no dairy"     |

## Usage Tips

- Adjust {{calories}} based on activity level and goals (deficit vs maintenance).
- Specify {{diet_type}} for better personalization (e.g., vegetarian or low-carb).
- Add constraints like “budget-friendly” or “meal prep friendly” for more practical outputs.
- Always cross-check nutritional accuracy if using for strict diet tracking.


