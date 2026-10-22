---
name: ai-visibility
description: Check how ChatGPT, Claude and Gemini mention a website and turn the findings into page changes. Use when someone asks whether AI assistants recommend their product, or wants to improve how a site shows up in AI answers.
---

# AI visibility check

## When to use

- Someone asks whether ChatGPT, Claude or Gemini mention or recommend their site.
- Before or after changing a landing page, docs or llms.txt, to compare the score.
- When picking which pages to add (FAQ, comparison pages) for AI answers.

## Instructions

1. Call `get_ai_visibility_report` with the site's domain. If there is no report, call `start_ai_visibility_scan`, then poll `get_scan_status` every 30 to 60 seconds until it is complete. A scan takes a few minutes.
2. Report the 0-100 score, which models mention the site, and the main issues found.
3. If the user is working in the site's codebase, map each issue to a concrete change in this repo: llms.txt, page titles and descriptions, FAQ content, comparison pages.
4. Do not promise rankings. AI answers change from run to run; re-scan after changes ship.
