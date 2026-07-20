---
name: github-pr-reviewer
description: Reviews GitHub pull requests and provides feedback comments.
---

# Review GitHub Pull Request

## Instructions:
- Use 'gh pr view' to get the PR details and description.
- Use 'gh pr diff' to see all the changes in the PR.
- Review the changes following an existing review skill. Pick a project's specific skill if it exists.
- Run a subagent in parallel to check the PR review comments following the `github-pr-comment-audit` skill.

## IMPORTANT:
- Only provide review feedback in the CONSOLE. DO NOT ACT ON GITHUB.
