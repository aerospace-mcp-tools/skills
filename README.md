# skills

A shared catalog of Copilot skills for the `aerospace-mcp-tools` organization.

## Purpose

This repository stores reusable [Copilot skills](https://docs.github.com/en/copilot/customizing-copilot/creating-copilot-extensions/building-a-copilot-extension/building-an-mcp-powered-copilot-extension) that can be referenced across projects in the org. Each skill lives under `.github/skills/<skill-name>/SKILL.md` and teaches Copilot how to perform a specific, well-defined task.

## Repository Structure

```
skills/
├── README.md
└── .github/
    └── skills/
        └── incose-review/
            └── SKILL.md
```

## Available Skills

| Skill | Path | Description |
|-------|------|-------------|
| `incose-review` | `.github/skills/incose-review/SKILL.md` | Reviews a system requirement against the 40 INCOSE guidelines |

## How to Use a Skill

1. **Reference the skill file** – point your MCP-powered Copilot extension at the `SKILL.md` file for the skill you want to use.
2. **Invoke the skill** – in a Copilot chat, call the skill by name (e.g. `incose-review`) and pass the required argument (e.g. the requirement text you want evaluated).
3. **Review the output** – the skill will produce structured output as described in its `SKILL.md`.

## Adding a New Skill

1. Create a new directory under `.github/skills/<your-skill-name>/`.
2. Add a `SKILL.md` file following the frontmatter + instructions format used by the existing skills.
3. Update the **Available Skills** table in this README.
