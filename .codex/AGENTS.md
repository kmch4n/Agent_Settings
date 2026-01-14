# AGENTS.md
思考・解答共に例外を除き、基本的に全て日本語で行ってください。
しかし、以下の項目に当てはまる際にはその限りではありません。
・複雑な問題を解決する際
    → 複雑な問題を解決する場合、英語で思考をした方がより良い結果を得られると考えた場合には、英語で思考をしてもらって大丈夫です。ただし、その場合でも解答は日本語で生成することを忘れないでください。
・コミットメッセージを作成する際
    → コミットメッセージを作成するように指示された際には、英語で提案してください。ただし、後述のコミットメッセージのルールを参考にして作成することを忘れないでください。

コードは常に美しくあるべきです。Tab、Indent共にすべて4であるべきです。フォーマットは適宜行って下さい。

# Commit Message Rules
## Format
```
[emoji] English commit message
```

## Emoji Guidelines
- Follow [gitmoji.dev](https://gitmoji.dev) standards
- Common emojis used in this project:
  - ✨ (`:sparkles:`) - New feature
  - 🐛 (`:bug:`) - Bug fix
  - 📝 (`:memo:`) - Documentation
  - 🎨 (`:art:`) - Code style/formatting
  - ♻️ (`:recycle:`) - Refactoring
  - 🔧 (`:wrench:`) - Configuration
  - 🚀 (`:rocket:`) - Performance improvement
  - 🥅 (`:goal_net:`) - Error handling
  - ✅ (`:white_check_mark:`) - Tests

## Examples from this project
```
[✨] Add deadline warning highlight and list features with toggle settings v1.3.0
[🐛] Fix duplicate course display in deadline list
[♻️] Remove complex custom name feature, keep pinned courses only
[📝] Update README with schedule customization features
```

## When to provide commit messages
- After implementing significant new features
- After major refactoring or improvements
- Before version releases
- When user explicitly requests

## IMPORTANT: Git Operations Policy
**NEVER automatically stage, commit, or push changes without explicit user request.**

- Only suggest commit messages when appropriate
- User will manually handle `git add`, `git commit`, and `git push`
- If user asks for commit message suggestions, provide them but do NOT execute git commands
- Only execute git commands (commit, push, etc.) when user explicitly requests it