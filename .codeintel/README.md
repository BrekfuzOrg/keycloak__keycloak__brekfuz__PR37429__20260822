# breken

Merging this gave everyone on this repository a map of the codebase, in whatever
coding agent they use. Nothing was installed on anybody's machine — `npx` fetches
it on first use and caches it.

## What changed

- `.mcp.json` — the tools. Ask "what calls this?" or "what breaks if I delete it?"
  and the answer comes from the call graph rather than from a text search.
- `.claude/settings.json` — loads the exact repository wiki commit when a Claude Code
  session starts or resumes. Pull-request reviews run on GitHub after you push.

## What it costs

Structural wiki answers use no model, no network. Model reviews run only from GitHub pull-request events.

## Removing it

Delete the `breken` entry from `.mcp.json`. Nothing else is left behind.
