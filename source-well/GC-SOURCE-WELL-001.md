---
card_id: GC-SOURCE-WELL-001
name: Repository Continuity
status: Candidate
parent: 01 Grove Card Library
notion_url: https://app.notion.com/p/38f1b7d9700a81dc8d37ebd63b75b839
purpose: |
  Keep AI continuity inside the repository instead of relying on chat memory.
when_to_use: |
  At the start of every new coding session or repository.
inputs: |
  Project architecture, brand spec, manifests, operating rules.
outputs: |
  Consistent AI behavior across Claude Code, Replit, and future sessions.
constraints: |
  Repository is the source of truth. No redesigns. Read source well before changes.
fail_conditions: |
  AI invents tokens, ignores spec, bypasses manifest, or relies on prior chat memory.
notes: |
  Introduce a Source Well layer containing CLAUDE.md, START_HERE.md,
  REPLIT-BUILD-MANIFEST.md, BAXLEY_SPEC, and system architecture docs.
  Every coding agent must read these before making changes.
  Continuity lives in the repo, not the conversation.
---

# GC-SOURCE-WELL-001 — Repository Continuity

_No long-form body in Notion. The card is fully expressed by its properties above._
