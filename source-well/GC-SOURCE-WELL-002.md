---
card_id: GC-SOURCE-WELL-002
name: Session Provenance IDs
status: Candidate
parent: 01 Grove Card Library
notion_url: https://app.notion.com/p/38f1b7d9700a819cac84ee8d63de4106
purpose: |
  Connect repo files, Notion records, and Claude Code sessions using stable
  IDs instead of relying on chat memory.
when_to_use: |
  Use when starting or resuming Claude Code, Replit, or other AI build
  sessions that need continuity across tools.
inputs: |
  Source Well ID, session ID, related laws, repo name, files touched,
  artifacts implemented, Notion links.
outputs: |
  A traceable session record that links implementation events back to
  governing source, laws, and artifacts.
constraints: |
  Do not make sessions the source of truth. Sessions are implementation
  events. The Source Well and repository remain canonical.
fail_conditions: |
  PASS: every session declares Source Well, related laws, files touched, and outcome.
  EDGE: session has notes but weak links.
  FAIL: work depends on remembering a chat or browsing hidden session history.
---

# GC-SOURCE-WELL-002 — Session Provenance IDs

## Core lock

Continuity should not depend on whether Claude, Claude Code, Replit, or mobile UI can surface the right prior session.
Continuity should be reconstructed through stable provenance IDs.

## Model

Every meaningful object gets a stable ID.
The session does not become the source of truth. It becomes an implementation event linked back to the source.

## Example ID map

- SW-001 — Source Well
- REPLIT-001 — Initial Replit Build Sequence
- LAW-BC-01 — Descendant Rule
- LAW-BC-02 — Source Well Rule
- ARB-004 — Mission
- ARB-005 — Ceiling
- GC-SOURCE-WELL-001 — Repository Continuity
- CC-001 — Claude Code Session

## Session record pattern

A Claude Code or Replit session should begin by declaring:

- Session ID
- Repository
- Source Well
- Related laws
- Related artifacts
- Files touched
- Work performed
- Open questions
- Next action

## Key distinction

Source Well = current governing truth.
Notion = historical reasoning, decisions, and relationships.
Sessions = implementation events performed against the source.

## Why this matters

If a session is missing from mobile or a coding tool does not expose prior history, the project can still reconstruct continuity through IDs and source records.
This turns a session from hidden memory into a traceable artifact.

## Practical rule

At the top of every build session, create or update a session record that references the active Source Well ID.
The repo should include the same ID in its source-well files, so Notion and the repo can point to each other without depending on chat history.
