# Delalify Agent Skills

Public agent skills for Delalify's platforms.

## Platforms

This repository organizes skills across three categories:

- **`skills/delalify/`** - Company-wide skills that apply across all Delalify platforms
- **`skills/apps-platform/`** - Skills for the Delalify Apps Platform, which provides integrated tools for relationship management, communication, file storage, and team access control
- **`skills/conjoin-platform/`** - Skills for the Conjoin Platform, Delalify's cloud infrastructure APIs for messaging, auth, storage, AI, billing, and relay

## Available Skills

| Skill                                                                     | Platform | Description                                                                         |
| ------------------------------------------------------------------------- | -------- | ----------------------------------------------------------------------------------- |
| [delalify-brand-guidelines](./skills/delalify/delalify-brand-guidelines/) | Delalify | Brand colors, typography, and design tokens for applying Delalify's visual identity |

## Installation

Install all skills:

```bash
npx skills add delalify/agent-skills
```

Install a specific skill:

```bash
npx skills add delalify/agent-skills --skill delalify-brand-guidelines
```

Install globally (available across all projects):

```bash
npx skills add delalify/agent-skills --skill delalify-brand-guidelines -g
```

Target a specific agent:

```bash
npx skills add delalify/agent-skills -a claude-code
```

## Managing Skills

```bash
npx skills list          # View installed skills
npx skills check         # Check for updates
npx skills update        # Update all installed skills
npx skills remove        # Remove installed skills
```
