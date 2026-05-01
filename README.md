# claude-skills

Personal Claude Code skills collection, optimized for mobile remote control development via [cmux](https://cmux.dev).

## Design Principles

- **SKILL.md is under 50 lines** — flow and pointers only
- **No inline code blocks** — all logic lives in `scripts/`
- **Docs go in `references/`** — one file per topic
- **Script output goes to log files** — stdout prints only the path to save tokens

## Skills

| Skill | Description |
|-------|-------------|
| [rc-workspaces](skills/rc-workspaces/) | Bulk-start remote control sessions across all cmux workspaces |
| [create-skill](skills/create-skill/) | Create or refactor skills following the design principles above |
| [issue-implement](skills/issue-implement/) | Pick up a GitHub issue and deliver a PR end-to-end (1 issue = 1 PR) |

## Setup

Copy a skill into your Claude Code skills directory:

```bash
cp -r skills/<skill-name> ~/.claude/skills/
```

Or symlink for easy updates:

```bash
ln -s "$(pwd)/skills/<skill-name>" ~/.claude/skills/<skill-name>
```

## License

MIT
