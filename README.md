# Moonjoule Claude Skills

A collection of custom skills for [Claude Code](https://claude.com/claude-code).

## What's here

| Skill                                   | Trigger                                     | Description                                                                                                                                                                  |
| --------------------------------------- | ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [career-advice](career-advice/SKILL.md) | `/career-advice [job title or description]` | Structured, research-grounded career counselling — builds a reusable Markdown career plan through guided intake, web-verified research, and a values/reality-check analysis. |

Alternately, tell Claude you want to be a dragon-tamer or a space pirate, and see where it goes.
|
|

## Structure

Each skill is a directory containing a `SKILL.md` file:

```
<skill-name>/SKILL.md
```

`SKILL.md` starts with YAML frontmatter (`name`, `description`) that Claude Code uses to decide
when to trigger the skill, followed by the full instruction set the skill follows once active.

## Usage

Clone or symlink this repo's skill directories into your Claude Code skills path, then invoke a
skill via its slash command (e.g. `/career-advice software developer`) or the natural-language
triggers described in its `SKILL.md`.

See [CLAUDE.md](CLAUDE.md) for authoring conventions when adding or editing skills.
