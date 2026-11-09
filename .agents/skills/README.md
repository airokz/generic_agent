# Skills

A skill is a reusable procedure for one kind of task. Keep one folder per skill,
with a `SKILL.md` containing YAML `name` and `description`, followed by
instructions. The folder name must match `name` and use hyphens.

This `.agents/skills/` location is discovered natively by Codex, Cursor,
GitHub Copilot, and Gemini CLI. `CLAUDE.md` points Claude Code here.

Start with [skill-guide/SKILL.md](skill-guide/SKILL.md) for help creating a
skill and finding existing ones.

Keep rules in `rules/`, background in `context/`, and progress in `memory.md`.
Add supporting scripts or references only when needed. Check a third-party
skill's contents, license, and tool requirements before using it.
