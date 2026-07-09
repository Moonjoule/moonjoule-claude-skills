# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A collection of custom Claude Code skills. There is no build system, package manager, or test
suite — the repository is purely Markdown-based skill definitions consumed by Claude Code at
runtime.

## Structure

Each skill lives in its own top-level directory containing a `SKILL.md` file:

```
<skill-name>/SKILL.md
```

`SKILL.md` has two parts:

1. **YAML frontmatter** (`name`, `description`) — the `description` is what Claude Code uses to
   decide when to trigger the skill, so it must enumerate concrete trigger phrases/commands
   (e.g. `/career-advice`) as well as natural-language variants a user might type.
2. **Body** — the full instruction set the skill follows once triggered: mode detection,
   required inputs, process steps, output template, and tone/guardrail notes.

## Authoring conventions (from existing skills)

- Skills are written as detailed operating procedures for Claude, not documentation for humans —
  write imperative instructions, not descriptions.
- Where a skill produces a user-facing artifact (e.g. a plan), include the exact Markdown
  template in the skill body so output is consistent across runs.
- Skills that use external/real-world data (labour market stats, program names, credentials,
  etc.) must instruct Claude to verify via web search rather than guess or hallucinate.
- Include an explicit guardrails section for any skill that role-plays a persona (e.g.
  counsellor), clarifying that the persona is a mode of engagement and does not override
  Claude's core safety behaviour.
