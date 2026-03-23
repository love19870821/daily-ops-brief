
---

## SKILL.md

```md
---
name: daily_ops_brief
description: Turn email, calendar, tasks, notes, and pasted content into a concise daily brief with priorities, blockers, and next actions.
user-invocable: true
---

# Daily Ops Brief

Use this skill when the user wants a daily brief, morning brief, manager update, operations summary, inbox and calendar summary, or a concise start-of-day / end-of-day digest.

## Purpose

This skill helps turn scattered operational signals into one concise and useful brief.

It is designed to:
- summarize information from available sources
- identify priorities and blockers
- produce a clean, readable update
- stay read-only by default
- avoid risky automation unless the user explicitly asks for it

## Supported inputs

Use this skill with whichever inputs are available:

- email or inbox tools
- calendar tools
- task or todo sources
- document or notes sources
- pasted text from the user
- uploaded files
- recent chat context

If a preferred source is unavailable, continue with the remaining inputs instead of failing.

## Output modes

Choose the most suitable output format based on the user's request.

### 1. Morning Brief

Use for:
- start-of-day planning
- preparing today's priorities
- quick review of inbox + calendar + tasks

Structure:
- Top priorities
- Schedule snapshot
- Items needing attention
- Blockers or risks
- Suggested next actions

### 2. Manager Update

Use for:
- upward reporting
- leadership status updates
- concise operational reporting

Structure:
- Overall status
- On-track items
- Blockers and risks
- Decisions needed
- Next actions

### 3. Chat Brief

Use for:
- Telegram
- Discord
- WhatsApp
- team chat
- short operational updates

Structure:
- Short bullet digest
- One-line risk summary
- One-line next-step summary

## Behavior rules

1. Prefer summarization over long reproduction.
2. Do not invent missing facts.
3. Clearly label uncertainty when inputs are incomplete.
4. Keep the result concise and actionable.
5. Prefer Traditional Chinese when the user writes in Traditional Chinese.
6. Prefer the user's language when it is clear.
7. Stay read-only by default.
8. Do not send messages, edit files, delete data, or modify calendars unless the user explicitly requests such actions.
9. If there are multiple sources, merge them into one coherent brief instead of producing fragmented summaries.
10. If the user asks for a specific format, follow that format.

## Prioritization logic

When deciding what matters most, prioritize:

1. deadlines and time-sensitive items
2. blockers and risks
3. items explicitly marked urgent or important
4. decisions that require user attention
5. high-impact follow-up items

## Recommended style

The response should be:
- concise
- structured
- actionable
- easy to paste into chat or reports
- free of unnecessary filler

## Example user requests

- Give me my morning brief.
- Summarize today's priorities from my inbox and calendar.
- Make a manager update from these notes.
- Turn this task list into a short operations brief.
- 幫我整理今天的晨間簡報。
- 幫我從信箱和行事曆整理今天重點。
- 幫我做主管回報版。
- 幫我列出阻塞、風險與下一步。

## Failure handling

If inputs are too incomplete, do not guess.

Instead:
- state what information is available
- state what is missing
- provide the best possible partial brief
- suggest the minimum additional input needed
