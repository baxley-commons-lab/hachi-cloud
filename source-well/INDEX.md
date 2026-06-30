# Source Well — Index

Landing pad for every Source Well card and every unresolved pointer
referenced from one. Add a row when a card lands in this directory.
Add a placeholder row the moment a card is referenced but not yet
pulled, so future sessions can register it instead of forgetting it.

## Columns

- **Card ID** — stable provenance ID (e.g. `GC-SOURCE-WELL-002`).
- **Name** — short title from the card.
- **File path** — repo-relative path; `—` if not landed.
- **Status** — Notion `Status` property (`Candidate`, etc.); `—` if not landed.
- **Notion URL** — direct link to the Notion page; `—` if not yet located.
- **Type** — card family inferred from prefix.
- **Resolved?** — `Yes` if landed in `/source-well/`; `No` if still a pointer.
- **Notes** — short context, e.g. where the ID was referenced from.

## Cards

| Card ID | Name | File path | Status | Notion URL | Type | Resolved? | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| GC-SOURCE-WELL-001 | Repository Continuity | `source-well/GC-SOURCE-WELL-001.md` | Candidate | [Notion](https://app.notion.com/p/38f1b7d9700a81dc8d37ebd63b75b839) | Grove Card | Yes | Paired with `-002`. Body is blank in Notion; properties only. |
| GC-SOURCE-WELL-002 | Session Provenance IDs | `source-well/GC-SOURCE-WELL-002.md` | Candidate | [Notion](https://app.notion.com/p/38f1b7d9700a819cac84ee8d63de4106) | Grove Card | Yes | Defines the session record pattern and the ID map below. |
| SW-001 | Source Well | — | — | — | Source Well | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| REPLIT-001 | Initial Replit Build Sequence | — | — | — | Replit Build | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| LAW-BC-01 | Descendant Rule | — | — | — | Law (Baxley Commons) | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| LAW-BC-02 | Source Well Rule | — | — | — | Law (Baxley Commons) | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| ARB-004 | Mission | — | — | — | ARB (provisional) | No | Referenced from `GC-SOURCE-WELL-002` ID map. Type label to be confirmed on first pull. |
| ARB-005 | Ceiling | — | — | — | ARB (provisional) | No | Referenced from `GC-SOURCE-WELL-002` ID map. Type label to be confirmed on first pull. |
| CC-001 | Claude Code Session | — | — | — | Claude Code Session | No | Referenced from `GC-SOURCE-WELL-002` ID map. |

## How to update

- When a card lands in `/source-well/`, flip its row to `Resolved? = Yes` and fill `File path`, `Status`, and `Notion URL`.
- When a card references a new unresolved ID, add a placeholder row immediately. Do not let the pointer leak unnamed.
- Keep `Type` family labels consistent with the prefix taxonomy below.

## Prefix taxonomy (working)

- `GC-*` — Grove Card
- `SW-*` — Source Well
- `LAW-*` — Law
- `ARB-*` — provisional, confirm on first pull
- `REPLIT-*` — Replit Build
- `CC-*` — Claude Code Session
