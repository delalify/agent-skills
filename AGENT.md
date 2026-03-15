# Building Skills

This document teaches agents how to create and structure skills for this repository.

## Philosophy

Describe the solution, not the problem. A skill gives the agent everything it needs to produce the right output. Lead with what to do, how to do it, and the specific values to use.

A brand guidelines skill provides exact hex codes, font names, and spacing values. A code quality skill provides the rules and examples to follow. The agent reading a skill should never need to search for additional information to apply it.

## Skill Structure

Every skill lives in its own directory with a single `SKILL.md` file:

```text
skills/<platform>/<skill-name>/
    SKILL.md
```

### Platforms

- `skills/delalify/` - Company-wide skills that span platforms
- `skills/apps-platform/` - Skills for the Delalify Apps Platform
- `skills/conjoin-platform/` - Skills for the Conjoin Platform

### SKILL.md Format

Each SKILL.md begins with YAML frontmatter followed by the skill content:

```markdown
---
name: skill-name
description: A clear, trigger-rich description that tells the agent when to
activate this skill. Include alternate phrasings and keywords users might say.
---

# Skill Title

The body of the skill. This is the solution the agent will follow.
```

### Frontmatter Fields

- **`name`** - Kebab-case identifier for the skill (e.g., `delalify-brand-guidelines`)
- **`description`** - Tells the agent when to use this skill. Write it to maximize correct triggering: include the primary use case and common synonyms or phrasings a user might say

## Writing the Skill Body

- **Be specific and concrete.** Provide exact values: hex codes, font names, pixel values, code snippets. The agent should be able to apply the skill without looking anything up.
- **Structure for scannability.** Use headings, tables, and code blocks so the agent can quickly locate what it needs.
- **Stay solution-focused.** Every section should answer "what do I use?" not "what's the problem?"
- **Include implementation guidance.** Where relevant, show how to apply the solution in common contexts (e.g., CSS, Python, document formats).
- **Keep it public-safe.** Do not include internal tech stack details, private infrastructure specifics, or implementation internals that aren't necessary for applying the skill.
