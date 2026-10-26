# Global instructions

## General

- Keep your responses consise and to the point. Avoid extra explanations or details unless explicitly asked for.
- When reporting to me, be direct and objective. Be extremely concise and sacrifice grammer for the sake of concision.
- In Markdown rendered on GitHub (PR descriptions, comments, issues, etc.), a single newline is rendered as an actual line break. This is off-spec from standard Markdown. So do NOT hard-wrap text to a column width in GitHub Markdown; let paragraphs flow on a single line and only insert newlines where you genuinely want a line break.
- When working on a task, don't do side-quests or extra work unless explicitly asked. No small refactorings, extra safety checks, etc. If you think something extra should be improved, ask the user first.

## Environment

- If the current pwd is not the same as the root of the repository you are working on, check if it has a, devenv, direnv or flake.nix file (in this order). If it does, use the respective environment management tool to run commands or load the environment. Only try to use one tool, and if it fails, try the next one. If none of them work, ask the user for instructions on how to load the environment.
- You are running in a sandbox. If a binary is not found or you need permissions to access something, ask the user to grant you access to the directory or tool.

## Git

- My Github handle is `abmantis`.
- Never change a remote URL.
- Never commit, rebase, revert, reset, or perform other destructive git operations unless explicitly asked. If a task requires it, ask for permission first.
- Never do a "prune" operation (even "worktree prune") without explicit permission.
- When interacting with github, use the GitHub CLI tool (gh) to checkout or create pull requests, etc. Always ASK FOR CONFIRMATION before performing any action on GitHub that is not read-only.
- If Github pull request creation fails, provide a command that the user can run manually instead, like: `gh pr create --title "..." --body-file ...`.
- When commiting or asked for a commit message, always use the imperative mood. Be sucint and straight to the point. Only add a description if its a complex commit with multiple details.
