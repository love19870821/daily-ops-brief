# Daily Ops Brief

Turn email, calendar, tasks, and pasted notes into a concise daily brief with priorities, blockers, and next actions.

This skill is designed to be:
- **low maintenance**
- **read-only by default**
- **useful even without custom plugins**
- **good for chat-first workflows**

## Best use cases

- morning brief
- manager update
- inbox + calendar summary
- end-of-day wrap-up
- concise chat-ready status post

## What this skill does

The skill tells OpenClaw to:
1. gather signals from available sources,
2. prioritize what matters,
3. produce one compact brief in the user's language,
4. avoid sending or editing anything unless explicitly asked.

## Why this design

This version avoids high-maintenance logic and risky automation.
It works with:
- installed mail/calendar/task tools,
- pasted text,
- uploaded files,
- chat context.

That makes it easier to publish, easier to adopt, and easier to keep stable.

## Included output modes

### Morning Brief
Default start-of-day summary with top priorities, schedule snapshot, blockers, and next actions.

### Manager Update
Forwardable summary with status, risks, decisions needed, and next steps.

### Chat Brief
A short bullet digest that can be pasted into Telegram, Discord, WhatsApp, or similar tools.

## Install locally

Place this folder in one of these locations:
- `<workspace>/skills/daily-ops-brief`
- `~/.openclaw/skills/daily-ops-brief`

Then start a new OpenClaw session and verify with:

```bash
openclaw skills list
```

## Suggested publish metadata

- **slug**: `daily-ops-brief`
- **name**: `Daily Ops Brief`
- **tags**: `daily-brief,productivity,ops,summary,workflow`

## Publish example

```bash
clawhub publish ./daily-ops-brief \
  --slug daily-ops-brief \
  --name "Daily Ops Brief" \
  --version 0.1.0 \
  --changelog "Initial public release" \
  --tags daily-brief,productivity,ops,summary,workflow
```

## Example prompts

- Give me my morning brief.
- Summarize today's priorities from my inbox and calendar.
- Make a manager update from these notes.
- Turn this todo list into a short operations brief.
- 幫我整理今天重點。
- 幫我做主管版日報。
- 幫我把這些待辦整理成晨間簡報。

## Recommended next step before publishing

Edit the skill description, README, and optional homepage to point to your own GitHub repo or profile.
That gives you a public landing page for stars, issues, updates, and optional sponsor links.
