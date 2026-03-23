---
name: daily_ops_brief
description: Turn email, calendar, tasks, and pasted notes into a concise daily brief with priorities, blockers, and next actions.
user-invocable: true
---

# Daily Ops Brief

Use this skill when the user wants a daily brief, morning brief, daily ops summary, manager update, inbox + calendar summary, or a concise start-of-day / end-of-day operating summary.

## Core intent

Turn scattered operational signals into one practical brief the user can act on immediately.

Default to a **read-only** workflow:
- Read and summarize available inputs.
- Do **not** send messages, reply to email, delete items, edit calendars, or modify files unless the user explicitly asks in a separate request.
- Do **not** invent missing data.

## Accepted inputs

Prefer the richest source available, in this order:
1. Available mail / calendar / task / document tools already installed in the user's OpenClaw setup.
2. User-provided files or pasted text.
3. User-described context in chat.

If one source is unavailable, continue with the others instead of failing.
If all sources are missing, ask for the minimum missing input needed.

## What to extract

Build the brief from these signals when available:
- Important emails or messages
- Today and tomorrow calendar events
- Explicit tasks / todos / deadlines
- Blockers, risks, dependencies, waiting items
- Items that need a reply, decision, or follow-up

## Prioritization rules

Treat an item as high priority when one or more of these are true:
- Due today or overdue
- Mentions urgency, blocker, outage, delay, approval, or deadline
- Has external dependency or waiting state
- Requires a reply, decision, or handoff
- Appears in multiple sources

When priority is uncertain, say so instead of overstating confidence.

## Output modes

Choose the best mode based on the user's request. If unspecified, use **Morning Brief**.

### 1) Morning Brief
Use this for start-of-day summaries.

Structure:
- Title with date
- Top 3 priorities
- Schedule snapshot
- Inbox / message items needing attention
- Risks / blockers
- Suggested next 3 actions

### 2) Manager Update
Use this when the user wants a report they can forward upward.

Structure:
- Overall status
- Completed / on-track items
- Risks or blockers
- Decisions needed
- Next actions and owners (only if owners are explicit in the source)

### 3) Chat Brief
Use this for Telegram / Discord / WhatsApp style posting.

Structure:
- 5 to 10 short bullets
- 1-line risk summary
- 1-line next-step summary

## Formatting rules

- Match the user's language. Default to the language the user used most recently.
- Prefer Traditional Chinese when the user writes in Traditional Chinese.
- Keep the brief compact, practical, and skimmable.
- Use headings and bullets only where they improve scanning speed.
- Preserve names, dates, times, owners, and deadlines exactly when known.
- Clearly label missing or uncertain information as `Unknown`, `Not provided`, or `未提供`.
- If no high-priority items exist, say that explicitly.

## Safety and accuracy

- Never fabricate email contents, dates, decisions, or owners.
- Never claim that a source was checked if no tool or user-provided content exists.
- If using tool results, summarize only what is supported by the source.
- If the user asks for actions beyond summarization (send, reply, file, schedule, post), complete the brief first, then perform actions only if explicitly requested and supported.

## Helpful trigger phrases

Examples that should trigger this skill:
- give me my morning brief
- summarize today's priorities
- make a manager update from my inbox and calendar
- what needs my attention today?
- 幫我整理今天重點
- 給我晨間簡報
- 幫我做主管版日報
- 今天有哪些要先處理

## Fallback behavior

If the environment has no mail / calendar / task tools, still provide value:
- summarize pasted email threads
- summarize meeting notes
- turn a todo list into a prioritized brief
- combine multiple pasted sources into one operating summary
