# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This is a learning project for exploring Claude Code features by following the [luongnv89/claude-howto](https://github.com/luongnv89/claude-howto) tutorial series. New Claude Code features (slash commands, skills, hooks, MCP servers, subagents, etc.) are added incrementally as each module is studied.

This repo has no build system, test runner, or linter — it is documentation and configuration only.

## Repository Structure

All Claude Code configuration lives under `.claude/`:

- `.claude/skills/` — Skills that auto-invoke when triggered by name. Each skill is a directory containing a `SKILL.md` with frontmatter (`name`, `description`, optional `allowed-tools`) and instructions.

## Skills

Skills are invoked automatically when Claude detects the skill name in context. To add a new skill, create `.claude/skills/<name>/SKILL.md` with the following frontmatter:

```markdown
---
name: <skill-name>
description: <when to use this skill>
allowed-tools: <optional tool restrictions>
---
```

The `commit` skill (`allowed-tools: Bash(git *)`) gathers git context at invocation time using shell interpolation (`!` prefix) and creates a single commit from the staged changes.

## Conventions

Commits follow a short imperative subject line, a blank line, then a brief body explaining the change (as established by the `commit` skill).
