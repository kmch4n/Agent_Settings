# Claude Code Settings

This repository contains my personal Claude Code configuration files for consistent development workflow across projects.

## Structure

```
.claude/
├── commands/              # Custom slash commands
│   ├── commit_message_suggestion.md
│   └── diff_summary.md
└── rules/                 # Project-wide rules
    └── commit_message.md
```

## Commands

### `/commit_message_suggestion`
Reviews recent code diffs and suggests an appropriate commit message following the gitmoji format defined in the rules.

### `/diff_summary`
Analyzes recent code changes and provides:
- Summary of what changed
- Impacted modules/files
- Potential risks/regressions
- Suggested follow-up checks

## Rules

### Commit Message Format
All commits follow the gitmoji format:
```
[emoji] English commit message
```

Common emojis used:
- ✨ `:sparkles:` - New feature
- 🐛 `:bug:` - Bug fix
- 📝 `:memo:` - Documentation
- 🎨 `:art:` - Code style/formatting
- ♻️ `:recycle:` - Refactoring
- 🔧 `:wrench:` - Configuration
- 🚀 `:rocket:` - Performance improvement
- 🥅 `:goal_net:` - Error handling
- ✅ `:white_check_mark:` - Tests

## Usage

To use these settings in your projects, copy the `.claude/` directory to your project root:

```bash
# Clone this repository
git clone https://github.com/yourusername/Claude_Settings.git

# Copy to your project
cp -r Claude_Settings/.claude /path/to/your/project/
```

## Safety

All commands are configured to **never** automatically perform git operations (commit, push, etc.) without explicit user request.
