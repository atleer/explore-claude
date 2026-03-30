# Explore Claude Code

A hands-on learning project for mastering [Claude Code](https://claude.ai/code) by following the tutorials at [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto).

## Learning Goals

1. Improve understanding of slash commands
2. Learn how to orchestrate subagents
3. Learn how to use model context protocols
4. More to be added

## Tutorial Modules

The [claude-howto](https://github.com/luongnv89/claude-howto) guide covers 10 modules, progressing from basic usage to advanced workflows:

| # | Module | Description |
|---|--------|-------------|
| 1 | **Slash Commands** | User-invoked shortcuts stored as Markdown files |
| 2 | **Memory** | Persistent context across sessions via `CLAUDE.md` files |
| 3 | **Skills** | Reusable, auto-invoked capabilities with scripts |
| 4 | **Subagents** | Specialized AI assistants with isolated contexts |
| 5 | **MCP Protocol** | Model Context Protocol for external tool integration |
| 6 | **Hooks** | Event-driven shell automation across 25 event types |
| 7 | **Plugins** | Bundled feature collections for complete workflows |
| 8 | **Checkpoints** | Session snapshots enabling safe experimentation |
| 9 | **Advanced Features** | Planning mode, extended thinking, background tasks |
| 10 | **CLI Reference** | Terminal commands and automation |

## Project Structure

```
.claude/
  skills/
    commit/        # Skill: auto-commit with context-aware messages
    my-command/    # Skill: template for custom skill definitions
```

## Resources

- [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code)
- [claude-howto tutorials](https://github.com/luongnv89/claude-howto)