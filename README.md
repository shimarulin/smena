# smena

## Repository tooling

- `mise.toml` — Python, uv, pre-commit and commit-check; installed with `mise install`.
- `commit-check.toml` — commit (Conventional Commits 1.0.0) and branch (Conventional Branch 1.1.0) policy.
- `.pre-commit-config.yaml` — hooks: `check-branch` at the `pre-commit` stage, `check-message` at the `commit-msg` stage.
- `.agents/skills/commit-check` — agent skill: checks the message and branch name against `commit-check.toml` before committing.

After cloning:

```sh
mise install
mise exec -- pre-commit install
```
