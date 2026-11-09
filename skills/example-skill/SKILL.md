---
name: example-skill
description: Help create a reusable agent skill or find an existing one. Use when asked how to author, discover, or adapt skills; ordinary task execution does not need this guide.
---

# Example skill: create or find a skill

## Create

1. Identify one repeatable task, when the skill should apply, required inputs, and the expected result.
2. Use the skill creator available in the chosen platform:
   - **Codex:** invoke `$skill-creator`. See the [official creator](https://github.com/openai/skills/tree/main/skills/.system/skill-creator) and [skill guide](https://learn.chatgpt.com/docs/build-skills).
   - **ChatGPT Work:** invoke `@skill-creator` where available; see the same skill guide.
   - **Claude:** use Anthropic's [skill-creator](https://github.com/anthropics/skills/tree/main/skills/skill-creator) if installed. Follow the [Claude skill guide](https://code.claude.com/docs/en/skills) for setup and invocation.
   - **Other compatible tools:** follow the [Agent Skills specification](https://agentskills.io/specification) and the tool's instructions for installing skills.
3. If no creator is available, write a small `skills/<skill-name>/SKILL.md` with `name`, `description`, inputs, steps, expected output, and checks. Do not assume a linked creator is installed.
4. Try a representative task and one missing-input example. Check the actual result and revise the skill before relying on it.

## Find existing skills

- [OpenAI skills](https://github.com/openai/skills): official Codex catalog.
- [Anthropic skills](https://github.com/anthropics/skills): official examples and reusable skills.
- [skills.sh](https://skills.sh/): community directory and discovery.

Prefer original publishers. Check maintenance, license, scripts, and required access before adopting a skill. Confirm installation instructions for the chosen tool; sharing a format does not guarantee identical behavior. Keep a single local source and never treat a skill as permission for external actions.
