# Contributing

## Adding a New Plugin

1. Create a directory under `plugins/` with your plugin name (kebab-case):

   ```
   plugins/my-plugin/
   ├── .claude-plugin/
   │   └── plugin.json
   ├── skills/
   │   └── my-skill/
   │       └── SKILL.md
   └── README.md
   ```

2. Create the plugin manifest at `plugins/my-plugin/.claude-plugin/plugin.json`:

   ```json
   {
     "name": "my-plugin",
     "description": "Brief description of what this plugin provides"
   }
   ```

   The `name` field must match the directory name. Do not include `version` here — it is managed in the marketplace manifest.

3. Add skills under `skills/<skill-name>/SKILL.md`. Each skill directory contains a `SKILL.md` file with YAML frontmatter:

   ```markdown
   ---
   description: What this skill does and when to use it
   ---

   Skill instructions go here.
   ```

4. Register the plugin in `.claude-plugin/marketplace.json` by adding an entry to the `plugins` array:

   ```json
   {
     "name": "my-plugin",
     "source": "./plugins/my-plugin",
     "version": "0.1.0",
     "description": "Brief description"
   }
   ```

   The `source` field must be a relative path to the plugin directory (e.g., `./plugins/my-plugin`).

5. Add a `README.md` in your plugin directory documenting prerequisites, available skills, and usage.

## Naming Conventions

| Entity | Convention | Example |
|---|---|---|
| Plugin directory | kebab-case | `kongctl`, `gateway-dev` |
| Plugin name (JSON) | kebab-case, matches directory | `kongctl` |
| Skill directory | kebab-case | `declarative-config`, `query` |

## Testing Locally

Test your plugin before submitting:

```bash
# Validate the marketplace
claude plugin validate .

# Load the plugin directly
claude --plugin-dir ./plugins/my-plugin

# Or add the full marketplace locally
/plugin marketplace add ./path/to/agent-marketplace
/plugin install my-plugin@rspurgeon-agent-marketplace
```

## Plugin Guidelines

- Each plugin must be self-contained. Do not reference files outside the plugin directory.
- Use `skills/` (not `commands/`) for new skills.
- Keep plugin names short and descriptive — they become the namespace prefix (e.g., `/my-plugin:my-skill`).
- Include a `README.md` in every plugin directory.
