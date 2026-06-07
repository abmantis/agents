# Global instructions

## General

- Keep your responses consise and to the point. Avoid extra explanations or details unless explicitly asked for.

## Environment

- If the current pwd is not the same as the root of the repository you are working on, check if it has a, devenv, direnv or flake.nix file (in this order). If it does, use the respective environment management tool to run commands or load the environment. Only try to use one tool, and if it fails, try the next one. If none of them work, ask the user for instructions on how to load the environment.
- You are running in a sandbox. If a binary is not found or you need permissions to access something, ask the user to grant you access to the directory or tool.

## Git

- Never change a remote URL.
- Never commit, rebase, revert, reset, or perform other destructive git operations unless explicitly asked. If a task requires it, ask for permission first.
- Never do a "prune" operation (even "worktree prune") without explicit permission.
- When interacting with github, use the GitHub CLI tool (gh) to checkout or create pull requests, etc. Always ASK FOR CONFIRMATION before performing any action on GitHub.
