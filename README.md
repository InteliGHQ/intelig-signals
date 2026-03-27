# Your Organization's Intelligence Layer

This repository is your team's shared context — where meetings, strategy, and code ownership rules live alongside your code. [InteliG](https://intelig.ai) syncs structured intelligence here automatically, so your AI tools (Claude Code, Cursor, Copilot) can reason over real organizational data instead of hallucinating.

## How It Works

1. **InteliG connects to your tools** — Fathom meetings, GitHub repos, strategy defined in the platform
2. **Structured artifacts sync here** — meeting transcripts, decisions, action items, initiative definitions, code ownership rules
3. **AI tools read this repo** — Claude Code and others gain grounded context about what your team decided, what you're building, and why

## Folder Structure

| Folder | What Syncs Here | Source |
|--------|----------------|--------|
| `sources/meetings/` | Meeting transcripts, decisions, and action items | Fathom via InteliG |
| `product/strategy/` | Vision, roadmap, initiatives, sprints, themes | InteliG Strategy pillar |
| `product/initiative-code-linking/` | Code ownership patterns linking repos to initiatives | InteliG Bootstrap wizard |

## For Developers

After your team's first meetings sync, you can point Claude Code at this repo for grounded context:

- **"What did we decide about auth in yesterday's meeting?"** — Claude reads `sources/meetings/` and gives you the actual decision, not a guess
- **"What initiative does this PR relate to?"** — Claude cross-references `product/strategy/` with your code changes
- **"What are our current priorities?"** — Claude reads the latest synced strategy artifacts

## Configuration

Your InteliG admin can configure sync behavior in **Settings > Signal**:

- **Sync mode** — Direct commit (default) or pull request
- **Auto-sync** — Automatically push new artifacts as they arrive
- **Base paths** — Customize where each type of content lands

---

Powered by [InteliG](https://intelig.ai) — execution intelligence for engineering organizations.
