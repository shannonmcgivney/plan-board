# Plan Board: a Claude skill

Say **"whiteboard this plan"** and paste your messy notes, and Claude lays them out on a shared Claude Whiteboard. You get a timeline with an owner and a date on every step, and a list of what's still open.

**[⬇️ Download plan-board.zip](https://github.com/shannonmcgivney/plan-board/releases/latest/download/plan-board.zip)**

Most plans live in someone's head, a voice memo or a long chat. Nobody else can see them, and nothing has an owner. Claude Whiteboards (beta, on paid plans since November 2026) put the plan on a board your team can edit live. This skill tells Claude how to turn a brain dump into a clear board without making up owners or dates, how to run a retro on one, and when to turn the board into a doc or a deck.

## What it does

| Mode | What you give it | What you get |
|---|---|---|
| **Plan** | A brain dump, voice memo, meeting transcript or Slack thread | A left-to-right timeline: one block per step with owner and date, arrows for real dependencies, an Open questions section |
| **Retro** | Everyone's notes from a project, class or launch | Went well / Slowed us down / Try next, grouped by theme, plus one drafted action item per person |
| **Hand-off** | A finished board | A doc (project plan) or a deck, linked back to the board |

## Install

**Claude.ai or the Claude desktop app:** download `plan-board.zip` (don't unzip it), then go to **Customize → Skills → + Add → Upload skill** and pick the zip.

**Claude Code:**

```bash
git clone https://github.com/shannonmcgivney/plan-board.git
cp -R plan-board/skills/plan-board ~/.claude/skills/
```

Whiteboards need a paid Claude plan. On an Enterprise plan, an admin may need to switch them on first (Organization settings → Artifacts).

## Try it

- "Whiteboard this: we launch the course Jan 12, Maria does the landing page, I record the videos, emails go out the week before..."
- "Run a retro on these notes from our workshop and draft an action item for each person."
- "Turn this board into a one-page project plan."

## What it won't do

- Invent owners or dates. Anything unknown goes under Open questions.
- Share, send or post a board. Boards stay private until you share them.
- Promise features Anthropic hasn't confirmed. The skill marks a few claims from social posts as unconfirmed.

## Works well with

- [Launch Week](https://github.com/shannonmcgivney/launch-week): plan the launch, then put the week on a board and run a retro after.

## Credit

The idea came from a bestapps.ai Instagram carousel on Claude Whiteboards. The facts were checked against Anthropic's launch post (claude.com/resources/articles/sheets-whiteboards-data). The skill text is original material by McGivney Media.

By McGivney Media.
