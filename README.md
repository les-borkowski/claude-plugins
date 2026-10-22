# claude-plugins

Claude Code plugin marketplace for my plugins. Each plugin lives in its own repository; this repo
only lists them.

```
/plugin marketplace add les-borkowski/claude-plugins
/plugin install expediter@les-borkowski
/plugin install expediter-handoff@les-borkowski
/plugin install warden@les-borkowski
```

| Plugin | Repository | What it does |
| --- | --- | --- |
| `expediter` | [claude-expediter](https://github.com/les-borkowski/claude-expediter) | Feature tickets through role agents, each result checked before it ships |
| `expediter-handoff` | claude-expediter, `mods/expediter-handoff` | `/handoff`: write the resume checkpoint and clear |
| `warden` | claude-warden (private) | Security scanning MCP server; needs the `warden` CLI installed |

To publish a plugin, add an entry with a `github` (whole repo) or `git-subdir` (a folder of a repo)
source, then run `claude plugin validate .`.
