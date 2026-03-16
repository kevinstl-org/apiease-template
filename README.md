# APIEase Template

This repository is the minimal starter template used by `apiease-cli` for new APIEase projects.

Most users should consume this template through the CLI with `apiease init` instead of cloning the repository directly.

The goal of this template is to provide a small, neutral starting point with a simple configuration file and a `resources/` directory that mirrors the core APIEase resource model:

- `resources/requests`
- `resources/widgets`
- `resources/variables`

The included example files are intentionally lightweight, but they now use the strict public API field shapes so they can serve as valid starting points instead of loose placeholders.

Current examples:

- `docs/knowledge/examples/resources/requests/example-request.json`: HTTP request example covering the common top-level fields, all HTTP parameter types, and all trigger types.
- `docs/knowledge/examples/resources/requests/example-liquid-request.json`: Liquid request example showing the `liquid` field.
- `docs/knowledge/examples/resources/requests/example-system-request.json`: System request example showing the required `system` parameters.
- `docs/knowledge/examples/resources/widgets/example-widget.json`: Widget example using canonical public widget field names.
- `docs/knowledge/examples/resources/variables/example-variable.json`: Variable example including the `sensitive` field.

The template also includes a bundled APIEase knowledge base at `docs/knowledge/apiEaseDocsConsolidated.md` so coding agents can understand the platform and configure project resources correctly.

## Customization Files

This template keeps the default template guidance separate from project-specific customization.

- `README.md` and `AGENTS.md` are the template-owned defaults.
- `docs/knowledge/apiEaseDocsConsolidated.md` is the template-owned APIEase product reference.
- `CUSTOM_README.md` is the intended place for user-specific project documentation.
- `CUSTOM_AGENT_GUIDANCE.md` is the intended place for user-specific agent instructions.

## Agent Guidance

This template is designed to work well with coding agents such as Codex, Claude, and GitHub Copilot.

- `AGENTS.md` contains the template-owned default guidance for agents.
- `docs/knowledge/apiEaseDocsConsolidated.md` contains the APIEase product knowledge agents should use when configuring resources.
- `CUSTOM_README.md` contains project-specific documentation for humans and agents.
- `CUSTOM_AGENT_GUIDANCE.md` is the intended place for users to add project-specific agent instructions.
- `CLAUDE.md` and `.github/copilot-instructions.md` provide compatibility entry points for tools that look for those filenames.

When extending this template into a real project, keep project-specific documentation in `CUSTOM_README.md` and project-specific agent instructions in `CUSTOM_AGENT_GUIDANCE.md` so those customizations stay separate from the template defaults.
