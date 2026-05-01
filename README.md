# claude-skills

Personal Claude Code plugins and skills marketplace by tetsumaru.

## Structure

- **`/plugins`** - Plugins developed and maintained in this repository
- **`/external_plugins`** - Third-party or community plugins

## Installation

```bash
/plugin install <plugin-name>@claude-skills
```

or browse via `/plugin > Discover`

## Design Principles

- **SKILL.md is under 50 lines** -- flow and pointers only
- **No inline code blocks** -- all logic lives in `scripts/`
- **Docs go in `references/`** -- one file per topic
- **Script output goes to log files** -- stdout prints only the path to save tokens

## Plugin Structure

```
plugin-name/
├── .claude-plugin/
│   └── plugin.json      # Plugin metadata (required)
├── .mcp.json            # MCP server configuration (optional)
├── commands/            # Slash commands (optional)
├── agents/              # Agent definitions (optional)
├── skills/              # Skill definitions (optional)
└── README.md            # Documentation
```

## License

MIT
