# jrock2004-ai-marketplace

Claude skills by John Costanzo, free for anyone to install.

## Install

Add the marketplace once in Claude Code:

```text
/plugin marketplace add jrock2004/jrock2004-ai-marketplace
```

Then install any plugin from it:

```text
/plugin install <plugin-name>@jrock2004
```

To get new versions later, run:

```text
/plugin marketplace update jrock2004
```

## Plugins

| Plugin | What it does |
| ------ | ------------ |
| _None yet_ | |

## Add a skill

Skills are grouped into plugins, so people can install only the ones they want.

1. Copy `templates/plugin/` to `plugins/<plugin-name>/`, or use an existing plugin if the skill fits it.
2. Replace `plugin-name` and `skill-name` with real names, and write the skill in `SKILL.md`.
3. For a new plugin, add it to `.claude-plugin/marketplace.json` and to the table above:

   ```json
   {
     "name": "plugin-name",
     "source": "./plugins/plugin-name",
     "description": "One sentence on what this plugin helps with."
   }
   ```

4. Check your work:

   ```bash
   claude plugin validate .
   ```

To try a plugin before publishing it, run `claude --plugin-dir ./plugins/<plugin-name>`.

## License

[MIT](LICENSE)
