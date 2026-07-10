# Moonjoule Claude Skills

A collection of custom skills for [Claude](https://claude.ai) or [Claude Code](https://claude.com/claude-code).

## What's here

| Skill                                                                                                                                      | Trigger                                     | Description                                                                                                                                                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [career-advice](career-advice/SKILL.md)                                                                                                    | `/career-advice [job title or description]` | Structured, research-grounded career counselling — builds a reusable Markdown career plan through guided intake, web-verified research, and a values/reality-check analysis.<br><br>Alternately, tell Claude you want to be a dragon-tamer or a space pirate, and see where it goes. |
| [marketplace-advisor](marketplace-advisor/SKILL.md)                                                                                        | `/marketplace-advisor` or paste a listing   | Evaluates secondhand marketplace listings (Facebook Marketplace, Kijiji, Craigslist, eBay, and similar) like a savvy, well-researched friend — flags scams and red-flag categories, researches fair pricing, and preps you for viewings and negotiation.<br><br>                     |
| Will give you completely serious advice, even when you ask it about this strange listing you've found for "a slightly enchanted mirror..." |

## Structure

Each skill is a directory containing a `SKILL.md` file:

```
<skill-name>/SKILL.md
```

`SKILL.md` starts with YAML frontmatter (`name`, `description`) that Claude Code uses to decide
when to trigger the skill, followed by the full instruction set the skill follows once active.

Some skills also include a `references/` subfolder with supporting files that the skill loads
on demand (see `marketplace-advisor` for an example).

## Installing a skill

### Claude Code (CLI)

Skills work natively off the filesystem, including any `references/` subfolder.

1. Copy or symlink the skill directory into your Claude Code skills path:
   - `~/.claude/skills/<skill-name>/` — available in every project (personal skills)
   - `.claude/skills/<skill-name>/` inside a specific repo — available in that project only
2. Invoke it via its slash command (e.g. `/career-advice software developer`) or the
   natural-language triggers described in its `SKILL.md`.

```bash
# example: install marketplace-advisor for all projects
cp -r marketplace-advisor ~/.claude/skills/
```

### Claude.ai (web, desktop, mobile)

Custom skills require a Pro, Max, Team, or Enterprise plan with code execution enabled —
free-tier accounts can't install them.

1. Zip the skill's folder so the folder itself (not just `SKILL.md`) is at the root of the zip —
   e.g. zipping `marketplace-advisor/` should produce a zip containing
   `marketplace-advisor/SKILL.md` and `marketplace-advisor/references/...`.
   ```bash
   zip -r marketplace-advisor.zip marketplace-advisor
   ```
2. In Claude.ai, go to **Settings → Capabilities → Skills → Upload** and upload the zip
   (menu wording has shifted between app versions — look for "Skills" under Settings if the
   exact path differs).
3. Claude automatically reads `SKILL.md` and any referenced files in `references/` — no manual
   consolidation into a single file is needed.

The same `SKILL.md` format works unmodified on both surfaces, so a skill built for Claude Code
can be zipped and uploaded to Claude.ai as-is.

See [CLAUDE.md](CLAUDE.md) for authoring conventions when adding or editing skills.
