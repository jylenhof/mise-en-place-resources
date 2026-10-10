# Agent instructions

All tools in this repository are managed by [mise](https://mise.jdx.dev/) (see `.mise.toml`).
Always run them through mise so the pinned versions are used:

- Run all checks: `mise x -- prek run --all-files`
- Commit (pre-commit and commit-msg hooks need the mise tools): `mise x -- git commit ...`
- GitHub CLI: `mise x gh@latest -- gh ...`
