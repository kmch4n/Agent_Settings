# Agent Settings

A unified configuration repository for managing AI assistant behavior across multiple platforms (Claude, Codex, Gemini).

## Overview

This repository centralizes the rules and instructions for AI coding assistants, ensuring consistent behavior across different AI platforms used in development workflows.

## Directory Structure

```
Agent_Setting/
├── .claude/                    # Claude AI configuration
│   ├── CLAUDE.md               # Main instructions
│   ├── commands/               # Custom command definitions
│   │   ├── commit_message_suggestion.md
│   │   └── diff_summary.md
│   └── rules/                  # Rule definitions
│       └── commit_message.md
├── .codex/                     # Codex configuration
│   └── AGENTS.md
├── .gemini/                    # Gemini configuration
│   └── GEMINI.md
└── README.md
```

## Common Rules

All AI assistants in this repository follow these shared guidelines:

| Rule | Description |
|------|-------------|
| **Language** | Responses should be in Japanese by default |
| **Exceptions** | English thinking allowed for complex problems; commit messages in English |
| **Code Style** | Tab and indent size: 4 spaces |
| **Git Policy** | Never execute git operations without explicit user request |

## Commit Message Format

All commit messages follow the [Gitmoji](https://gitmoji.dev) standard:

```
[emoji] English commit message
```

### Common Emojis

| Emoji | Code | Usage |
|-------|------|-------|
| ✨ | `:sparkles:` | New feature |
| 🐛 | `:bug:` | Bug fix |
| 📝 | `:memo:` | Documentation |
| 🎨 | `:art:` | Code style/formatting |
| ♻️ | `:recycle:` | Refactoring |
| 🔧 | `:wrench:` | Configuration |
| 🚀 | `:rocket:` | Performance improvement |
| 🥅 | `:goal_net:` | Error handling |
| ✅ | `:white_check_mark:` | Tests |

## Custom Commands

### commit_message_suggestion
Analyzes code differences and suggests appropriate commit messages following the Gitmoji format.

### diff_summary
Provides a concise summary of code changes in the current working directory.

## License

This project is for personal use.
