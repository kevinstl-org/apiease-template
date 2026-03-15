# APIEase Template

This repository is the minimal starter template used by `apiease-cli` for new APIEase projects.

Most users should consume this template through the CLI with `apiease init` instead of cloning the repository directly.

The goal of this template is to provide a small, neutral starting point with a simple configuration file and a `resources/` directory that mirrors the core APIEase resource model:

- `resources/requests`
- `resources/widgets`
- `resources/variables`

The included example files are intentionally lightweight so they can act as reference points without adding unnecessary structure to a new project.

## Agent Guidance

This template is designed to work well with coding agents such as Codex, Claude, and GitHub Copilot.

- `AGENTS.md` contains the template-owned default guidance for agents.
- `CUSTOM_AGENT_GUIDANCE.md` is the intended place for users to add project-specific agent instructions.
- `CLAUDE.md` and `.github/copilot-instructions.md` provide compatibility entry points for tools that look for those filenames.

When extending this template into a real project, keep custom agent instructions in `CUSTOM_AGENT_GUIDANCE.md` so the project-specific guidance stays separate from the template defaults.
