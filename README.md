# agent-recipes

Reusable agent skills: review, commit, refactor, test

## What it does

- Drop-in compatible with ~/.claude/skills
- Each skill is a folder with a single SKILL.md
- YAML frontmatter: name + when-to-use description
- Concrete instructions, output formats and examples
- Versioned like code: review changes in PRs

## Getting started

```bash
git clone <this repo>
cp -r skills/* ~/.claude/skills/
```

## How to use

```bash
# skills trigger automatically on matching tasks
# or invoke directly: /code-review
```

## Project structure

```text
├── .github/
│   └── dependabot.yml
├── docs/
│   ├── configuration.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── skills/
│   ├── code-review/
│   │   └── SKILL.md
│   ├── commit-message/
│   │   └── SKILL.md
│   ├── refactor-plan/
│   │   └── SKILL.md
│   └── test-writer/
│       └── SKILL.md
├── .editorconfig
├── .gitattributes
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
└── SECURITY.md
```
