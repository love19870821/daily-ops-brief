# Daily Ops Brief / 每日營運簡報

Turn email, calendar, tasks, notes, and pasted content into a concise daily brief with priorities, blockers, and next actions.

將電子郵件、行事曆、待辦事項、筆記與貼上的內容，整理成精簡清楚的每日重點簡報，包含優先事項、阻塞風險與下一步行動。

---

## Overview / 專案簡介

**Daily Ops Brief** is a low-maintenance OpenClaw skill designed for people who want a practical daily summary without risky automation.

**Daily Ops Brief** 是一個低維護、低風險的 OpenClaw skill，適合想快速取得每日重點摘要、但不希望導入高風險自動化流程的人使用。

It helps turn scattered information into one actionable brief that is easy to read, easy to share, and easy to trust.

它能將分散在不同來源的資訊整合為一份可立即使用的簡報，方便閱讀、方便分享，也更容易建立信任感。

---

## Why this skill exists / 為什麼要做這個 skill

Most daily work starts the same way: checking inboxes, calendars, task lists, chats, and notes.

多數人的工作日都是從同樣的流程開始：查看信箱、行事曆、待辦清單、聊天訊息與筆記。

That process is repetitive, fragmented, and mentally expensive.

這個流程很重複、很零碎，也很耗費注意力。

**Daily Ops Brief** exists to reduce that friction by producing one clean summary you can review in minutes.

**Daily Ops Brief** 的目的，就是把這些零碎資訊整理成一份乾淨清楚的摘要，讓你幾分鐘內就能掌握全局。

---

## Who this is for / 適用對象

This skill is especially useful for:

這個 skill 特別適合以下使用者：

- operators / 現場作業與營運人員
- team leads / 小組主管
- managers / 管理者
- founders / 創業者
- freelancers / 自由工作者
- admin staff / 行政與支援人員
- anyone who starts the day by reviewing multiple information sources / 任何每天一早都需要查看多個資訊來源的人

---

## What it does / 它能做什麼

Daily Ops Brief helps OpenClaw:

Daily Ops Brief 會協助 OpenClaw：

1. gather signals from available sources  
   收集可用來源中的關鍵資訊

2. identify what matters most  
   判斷哪些內容最重要

3. group priorities, blockers, and follow-ups  
   整理優先事項、阻塞風險與待追蹤項目

4. generate one compact brief in the user’s preferred language  
   以使用者偏好的語言產出一份精簡簡報

---

## Default behavior / 預設行為

This skill is intentionally conservative.

這個 skill 在設計上刻意採取保守策略。

By default, it is **read-only** and focused on summarization.

預設情況下，它是 **唯讀** 的，重點放在摘要整理，而不是主動執行操作。

It does **not** automatically:

它 **不會自動**：

- send messages / 發送訊息
- reply to email / 回覆電子郵件
- delete items / 刪除資料
- edit calendars / 修改行事曆
- modify files / 修改檔案
- perform risky automation / 執行高風險自動化流程

This makes it easier to adopt, easier to maintain, and easier to trust.

這樣的設計更容易導入、更容易維護，也更容易讓人放心使用。

---

## Supported input sources / 支援的輸入來源

Daily Ops Brief works with whichever sources are available in the environment.

Daily Ops Brief 會依照當前環境中可取得的來源來運作。

Possible sources include:

可用來源包含：

- installed mail tools / 已安裝的郵件工具
- installed calendar tools / 已安裝的行事曆工具
- installed task or document tools / 已安裝的待辦或文件工具
- pasted text / 直接貼上的文字
- uploaded files / 上傳檔案
- chat context / 對話上下文

If one source is missing, the skill should continue using the remaining available inputs instead of failing.

如果某個來源不存在，skill 應繼續使用其他可用來源，而不是直接失敗中止。

---

## Output modes / 輸出模式

### 1. Morning Brief / 晨間簡報

Best for start-of-day planning.

適合一天開始前快速掌握重點。

Includes:

內容包含：

- top priorities / 今日優先事項
- schedule snapshot / 行程快照
- items needing attention / 需要優先處理的項目
- blockers or risks / 阻塞與風險
- suggested next actions / 建議下一步

---

### 2. Manager Update / 主管回報版

Best for reporting upward or sharing status with leadership.

適合回報主管、管理層，或快速同步狀態。

Includes:

內容包含：

- overall status / 整體狀態
- on-track items / 正常進行中的項目
- blockers and risks / 阻塞與風險
- decisions needed / 需要決策的事項
- next actions / 下一步行動

---

### 3. Chat Brief / 聊天貼上版

Best for Telegram, Discord, WhatsApp, or team chat.

適合貼到 Telegram、Discord、WhatsApp 或團隊聊天群組。

Includes:

內容包含：

- short bullet digest / 精簡條列摘要
- one-line risk summary / 一行風險總結
- one-line next-step summary / 一行下一步總結

---

## Example prompts / 範例提示詞

### English

- Give me my morning brief.
- Summarize today’s priorities from my inbox and calendar.
- Make a manager update from these notes.
- Turn this task list into a short operations brief.
- Show me blockers, risks, and next actions.

### 繁體中文

- 幫我整理今天的晨間簡報。
- 幫我從信箱和行事曆整理今天重點。
- 依照這些筆記幫我做主管回報版。
- 把這份待辦清單整理成營運摘要。
- 幫我列出阻塞、風險與下一步。
- 今天有哪些事情最需要先處理？

---

## Why it is low-maintenance / 為什麼它適合低維護使用

This version is intentionally focused on a narrow, reliable workflow:

這個版本刻意聚焦在狹而穩定的工作流程上：

- reading / 讀取資訊
- summarizing / 摘要整理
- prioritizing / 判斷優先順序
- formatting / 格式化輸出

It avoids unnecessary complexity and reduces the chance of unexpected behavior.

它避免不必要的複雜度，也降低了意外行為與維護成本。

That makes it a better fit for long-term use.

這使它更適合長期穩定使用。

---

## Installation / 安裝方式

### Local skill folder / 本機技能資料夾

Place this skill folder in one of the following locations:

請將此 skill 資料夾放到以下任一位置：

```bash
<workspace>/skills/daily-ops-brief
~/.openclaw/skills/daily-ops-brief
