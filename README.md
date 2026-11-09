# generic_agent

A small bootstrap folder for AI-assisted research, writing, analysis,
operations, or code. Plain Markdown only: no scripts, no dependencies, and it
works the same on macOS, Linux, and Windows.

```text
AGENTS.md                            Shared agent instructions
CLAUDE.md                            Loads AGENTS.md for Claude Code
GEMINI.md                            Loads AGENTS.md for Gemini CLI
memory.md                            Progress, decisions, and next steps
.agents/skills/skill-guide/SKILL.md  Help creating and finding skills
rules/example_rule.md                A standing requirement
workflows/example_workflow.md        A repeatable process
templates/example_template.md        A reusable result format
context/                             Background knowledge
inputs/                              Original task materials
output/                              Generated deliverables
```

## Supported tools

| Tool            | Instructions                  | Skills in `.agents/skills/`      |
|-----------------|-------------------------------|----------------------------------|
| Codex           | `AGENTS.md`                   | Discovered natively              |
| Cursor          | `AGENTS.md`                   | Discovered natively              |
| GitHub Copilot  | `AGENTS.md`                   | Discovered natively              |
| Gemini CLI      | `GEMINI.md` → `AGENTS.md`     | Discovered natively              |
| Claude Code     | `CLAUDE.md` → `AGENTS.md`     | Read on demand via `CLAUDE.md`   |

Other tools that read `AGENTS.md` or follow the
[Agent Skills specification](https://agentskills.io/specification) should work
too. Note that `.agents/` is a hidden folder on macOS and Linux.

## Get started

1. Create your copy: click **Use this template** on GitHub, or run
   `git clone https://github.com/airokz/generic_agent.git my-project`, then
   remove the `.git` folder and run `git init` to start fresh history.
2. Fill in the **Project** section at the top of `AGENTS.md`.
3. Add your background to `context/` and task materials to `inputs/`.
4. Adapt or remove the example rule, workflow, and template.
5. Open the folder in your agent tool and describe the task and desired result:

> Read AGENTS.md and memory.md. Use the relevant rules, workflow, and inputs to [task]. Save [result] in output/, check [success criteria], and update memory.md.

`memory.md` is a plain file for continuing work across chats. It is maintained
through these instructions, independently of any tool's built-in memory.

No tools or skills are downloaded automatically.

Inputs, generated outputs, and local scratch files are ignored by Git. Rules,
context, memory, templates, and skills are tracked: keep them suitable for
sharing. For code tasks, use the project's source and test folders; add them
only as needed.

## License

[MIT](LICENSE)
