Skills are organized into bucket folders under `skills/`:

- `engineering/` — daily code work
- `productivity/` — daily non-code workflow tools
- `misc/` — kept around but rarely used
- `personal/` — tied to my own setup, not promoted
- `in-progress/` — drafts not yet ready to ship
- `deprecated/` — no longer used

Every skill in `engineering/`, `productivity/`, or `misc/` must have a reference in the top-level `README.md` and an entry in `.claude-plugin/plugin.json`. Skills in `personal/`, `in-progress/`, and `deprecated/` must not appear in either.

`.claude-plugin/marketplace.json` exposes this repo as a Claude Code plugin marketplace (`/plugin marketplace install TotalMarriageSupport/grill-me-skills`). It references the plugin as a whole via `source: "./"`, so individual skill additions do **not** require updating `marketplace.json` — only `plugin.json` and `README.md`. Bump `metadata.version` in `marketplace.json` only on meaningful releases.

Each skill entry in the top-level `README.md` must link the skill name to its `SKILL.md`.

Each bucket folder has a `README.md` that lists every skill in the bucket with a one-line description, with the skill name linked to its `SKILL.md`.
