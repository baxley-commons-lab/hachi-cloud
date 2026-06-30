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
| SW-001 | Source Well | `source-well/SW-001.md` | Active | — | Source Well (repo-canonical) | Yes | Constitution. Root of continuity. Repo is canonical; intentionally no Notion mirror. |
| REPLIT-001 | Initial Replit Build Sequence | — | — | [Notion](https://app.notion.com/p/38f1b7d9700a8068b233e23ae8e1d131) | Replit Build | No | Reclassified from a Notion page formerly titled `< Source well >`; its content is the Replit build sequence, not the Source Well. |
| LAW-BC-01 | Descendant Rule | — | — | — | Governing Law | No | Referenced from `GC-SOURCE-WELL-002` ID map. The descendant rule is the operational basis of SW-001. |
| LAW-BC-02 | Source Well Rule | — | — | [Notion](https://app.notion.com/p/38d1b7d9700a8142bb38cc903f18bd61) | Governing Law | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| ARB-004 | Mission | — | — | — | Arboretum | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| ARB-005 | Ceiling | — | — | — | Arboretum | No | Referenced from `GC-SOURCE-WELL-002` ID map. |
| CC-001 | Claude Code Session | — | — | — | Claude Code Session | No | Referenced from `GC-SOURCE-WELL-002` ID map. Template card for the session record pattern. |

## How to update

- When a card lands in `/source-well/`, flip its row to `Resolved? = Yes` and fill `File path`, `Status`, and `Notion URL`.
- When a card references a new unresolved ID, add a placeholder row immediately. Do not let the pointer leak unnamed.
- Keep `Type` family labels consistent with the prefix taxonomy below.

## Prefix taxonomy

- `GC-*` — Grove Card
- `SW-*` — Source Well (repo-canonical; SW-001 is the constitution)
- `LAW-*` — Governing Law (e.g. `LAW-BC-*` for Baxley Commons laws)
- `ARB-*` — Arboretum
- `REPLIT-*` — Replit Build
- `CC-*` — Claude Code Session
- `RQ-*` — RainQ

A standalone `TAXONOMY.md` is planned (see SW-001 § "What lives in /source-well/"); this section is the working source until it lands.
