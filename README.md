# generic_agent

A small bootstrap folder for AI-assisted research, writing, analysis, operations, or code.

```text
AGENTS.md                         Shared agent instructions
CLAUDE.md                         Loads the same instructions for Claude
memory.md                         Progress, decisions, and next steps
rules/example_rule.md             A standing requirement
workflows/example_workflow.md     A repeatable process
skills/example-skill/SKILL.md      Help creating and finding skills
context/                          Background knowledge
inputs/                           Original task materials
output/                           Generated deliverables
templates/example_template.md     A reusable result format
```

## Get started

1. Add your background to `context/` and task materials to `inputs/`.
2. Adapt or remove the example rule, workflow, and template.
3. Open the folder in your agent tool and describe the task and desired result.

> Read AGENTS.md and memory.md. Use the relevant rules, workflow, and inputs to [task]. Save [result] in output/, check [success criteria], and update memory.md.

`memory.md` is a plain file for continuing work across chats. It is maintained through these instructions, independently of any tool's built-in memory.

Skills live in the visible `skills/` folder. The instructions tell agents to read the relevant `SKILL.md`; native skill menus may require registration in your tool's supported location. No tools or skills are downloaded automatically.

Inputs, generated outputs, and local scratch files are ignored by Git. Rules, context, memory, templates, and skills are tracked: keep them suitable for sharing. For code tasks, use the project's source and test folders; add them only as needed.
