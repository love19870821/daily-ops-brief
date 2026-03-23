# Daily Ops Brief

Turn email, calendar, tasks, and pasted notes into a concise daily brief with priorities, blockers, and next actions.

Daily Ops Brief is a low-maintenance OpenClaw skill for people who want a clear start-of-day or manager-ready summary without risky automation.

## Why this skill exists
 
Most daily information is scattered across inboxes, calendars, task lists, chat, and notes. This skill turns that noise into one practical brief you can act on immediately.

It is designed to be:
- **Read-only by default**
- **Fast to use**
- **Useful even without custom plugins**
- **Safe for chat-first workflows**

## Who this is for

- operators
- team leads
- managers
- founders
- freelancers
- anyone who starts the day by checking multiple sources

## What it does

Daily Ops Brief helps OpenClaw:
1. gather signals from available sources,
2. identify what matters most,
3. group priorities, blockers, and follow-ups,
4. output one compact brief in the user's language.

By default, it **does not** send messages, reply to email, delete items, edit calendars, or modify files.

## Supported input sources

This skill works with whichever source is available:
- installed mail, calendar, task, or document tools
- pasted text
- uploaded files
- chat context

If one source is missing, it should continue with the others instead of failing.

## Output modes

### 1. Morning Brief
Best for start-of-day planning.

Includes:
- top 3 priorities
- schedule snapshot
- items needing attention
- blockers or risks
- suggested next actions

### 2. Manager Update
Best for forwarding upward.

Includes:
- overall status
- on-track items
- blockers and risks
- decisions needed
- next actions

### 3. Chat Brief
Best for Telegram, Discord, WhatsApp, or team chat.

Includes:
- short bullet digest
- one-line risk summary
- one-line next-step summary

## Example prompts

- Give me my morning brief.
- Summarize today's priorities from my inbox and calendar.
- Make a manager update from these notes.
- Turn this todo list into a short operations brief.
- 幫我整理今天重點。
- 給我晨間簡報。
- 幫我做主管版日報。
- 今天有哪些要先處理？

## Why it is low-maintenance

This version intentionally avoids high-risk automation.

It focuses on:
- reading
- summarizing
- prioritizing
- formatting

That makes it easier to adopt, easier to keep stable, and easier to trust.

## Installation

### Local skill folder

Place this folder in one of these locations:

```bash
<workspace>/skills/daily-ops-brief
~/.openclaw/skills/daily-ops-brief
