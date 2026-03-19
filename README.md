# Kong Agent Marketplace

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) for Kong agent plugins.

## Installation

Add this marketplace to Claude Code:

```shell
/plugin marketplace add Kong/agent-marketplace
```

Then install individual plugins:

```shell
/plugin install <plugin-name>@kong-agent-marketplace
```

## Repository Structure

```
agent-marketplace/
├── .claude-plugin/
│   └── marketplace.json        # Marketplace catalog
├── plugins/
│   └── <plugin-name>/          # One directory per plugin
│       ├── .claude-plugin/
│       │   └── plugin.json     # Plugin manifest
│       ├── skills/             # Skill definitions
│       │   └── <skill-name>/
│       │       └── SKILL.md
│       └── README.md           # Plugin docs
├── README.md
├── CONTRIBUTING.md
└── LICENSE
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add or modify plugins.

## License

Apache-2.0
