# Claude Code — Skills Repository

This repository is a collection of Claude Code skills. Each skill provides structured rules and examples that guide Claude to follow best practices for a specific technology.

## Repository Structure

```
skills-copy/
├── README.md              # Skills list and usage
├── AGENTS.md              # Agent guidance and rule priorities
├── CLAUDE.md              # This file
├── .gitignore
└── laravel-inertia-vue/   # Laravel + Inertia.js + Vue 3 skill
    ├── SKILL.md
    ├── AGENTS.md
    ├── README.md
    ├── metadata.json
    └── rules/
```

## Using Skills in a Project

Copy any skill into your project's `.claude/skills/` directory:

```bash
cp -r laravel-inertia-vue /your-project/.claude/skills/
```

## Contributing a New Skill

1. Create a new directory at the repo root (e.g., `laravel-livewire/`)
2. Add `SKILL.md`, `AGENTS.md`, `README.md`, `metadata.json`, and a `rules/` directory
3. Update the skills table in `README.md` and `AGENTS.md`
4. Keep rules atomic — one clear pattern per file

## Conventions

- **Commits**: Use [Conventional Commits](https://www.conventionalcommits.org/) (`feat:`, `fix:`, `docs:`, `chore:`)
- **Rule files**: Named `category-topic.md` (e.g., `form-useform-basic.md`)
- **Priority levels**: CRITICAL → HIGH → MEDIUM
- **Examples**: Always include a good/bad example in every rule
