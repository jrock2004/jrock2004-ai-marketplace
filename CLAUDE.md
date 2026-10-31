# jrock2004-ai-marketplace

A public Claude Code plugin marketplace. Its id is `jrock2004`. Skills ship inside plugins, and each plugin lives in `plugins/<plugin-name>/`.

## Adding a skill

- Add it to an existing plugin if it fits that plugin's theme. Otherwise, copy `templates/plugin/` to `plugins/<plugin-name>/` and replace the placeholder names.
- The folder name in `skills/` must match the `name` in that skill's `SKILL.md`.
- For a new plugin, add an entry to `plugins` in `.claude-plugin/marketplace.json` and a row to the table in `README.md`.
- Bump `version` in the plugin's `plugin.json` when changing a released plugin. Users only get an update when the version changes.
- Run `claude plugin validate .` before committing.

## Rules

- This repo is public. Never include secrets, personal data, or paths from a specific machine.
- Skills must work for other people, so don't assume John's setup or tools unless the skill says what it needs.
