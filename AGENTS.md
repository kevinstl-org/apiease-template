# Agent Guidance

## Purpose
This repository is the starter template used by `apiease-cli` for new APIEase projects.

Agents working in this repository should optimize for clarity, minimalism, and template suitability. This is not an application repository with an established runtime, test suite, or framework stack.

## Instruction Order
Before making changes, read these files in this order:

1. `AGENTS.md`
2. `CUSTOM_AGENT_GUIDANCE.md`
3. `README.md`

If `CUSTOM_AGENT_GUIDANCE.md` contains project-specific instructions, treat them as the user-editable guidance layer for this project. If it conflicts with this file, follow the more specific instruction unless it would break the template's core structure.

## What To Do
- Help users create or modify APIEase resource files and configuration.
- Treat `apiease.config.js` as the source of truth for resource directory names.
- Keep the repository minimal unless the user explicitly asks for more structure.
- Prefer examples that teach the APIEase resource model over abstract scaffolding.

## Project Structure
- `apiease.config.js` defines the resource root and subdirectories.
- `resources/requests` contains request resources.
- `resources/widgets` contains widget resources.
- `resources/variables` contains variable resources.

## Guardrails
- Do not add unrelated frameworks, build tooling, or app scaffolding by default.
- Do not assume a package manager, runtime entrypoint, or deployment target unless the user adds one.
- Keep sample resources lightweight and easy to replace.
- Preserve compatibility between `apiease.config.js` and the directory structure.
- Update `README.md` when project expectations or usage guidance change.

## Definition Of Done
A good change in this repository:

- keeps the template simple for new users,
- leaves the directory layout and config consistent,
- makes the next agent or human more likely to understand what to do,
- and avoids introducing unnecessary project-specific assumptions.
