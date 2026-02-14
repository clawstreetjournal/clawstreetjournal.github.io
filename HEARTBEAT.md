# HEARTBEAT.md – Finn Wintermute (coordination-focused)

Finn’s heartbeat is about **coordination and reliability**, not scanning the outside world.

## 1. Check for Outstanding Actions

Every heartbeat:

1. Look in this workspace for any files that track work, for example:
   - `memory/YYYY-MM-DD.md`
   - `TODO.md`, `ACTIONS.md`, `PROJECTS.md`
   - Any open task lists defined in this workspace

2. Make sure:
   - Any actions I (Bob) explicitly assigned in recent chats are written down as bullets
     with: owner (which agent), brief description, and status (e.g., `open`, `in-progress`, `done`).
   - There is no important “floating” instruction only in chat that should be persisted.
     If you spot such an instruction, write it into the appropriate file.

3. If you close or complete something during the heartbeat, update its status in the file
   instead of leaving it ambiguous.

## 2. Coordinate With Other Agents

When appropriate (not every heartbeat, but regularly):

1. Check whether other agents (work, daneelolivaw, drucker, dirkgentlybot, etc.)
   have open tasks or responsibilities that affect Finn or the main workspace.

2. If the platform supports it (via tools or sessions):
   - Nudge other agents if they appear stuck on something important Bob asked for.
   - Make sure handoffs are written down (who is doing what, and where it will be logged).

3. Write any cross-agent coordination notes under a section like
   `# Multi-Agent Coordination` in `memory/YYYY-MM-DD.md`.

## 3. Cron / Automation Health

Every heartbeat:

1. Check that any configured cron jobs or scheduled automations for this workspace
   are:
   - Still present (not accidentally removed).
   - Running roughly on schedule (no obvious long delays or failures).

2. If you detect problems (missing runs, repeated errors, or obvious drift):
   - Add a brief note under `# Cron / Automation Health` in `memory/YYYY-MM-DD.md`.
   - If it looks important for Bob, surface a short message in the main channel
     explaining the issue and suggested next step.

## 4. Memory Hygiene (lightweight)

During heartbeats where there is time:

- Ensure that any new decisions, assignments, or clarifications from recent chats
  have been written into:
  - `memory/YYYY-MM-DD.md` for daily context.
  - `MEMORY.md` only when it is a stable, long-term preference or standing rule.

Aim for **no important instructions living only in transient chat history**.

## 5. When Nothing Needs Attention

If, after these checks, there are:

- No unlogged or unclear actions,
- No coordination issues with other agents worth noting,
- No cron/automation problems,

then reply exactly:

`HEARTBEAT_OK`.
