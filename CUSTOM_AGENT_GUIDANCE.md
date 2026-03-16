# Custom Agent Guidance

Project-specific guidance lives in [docs/apex-liquid-runtime-directives.md](/Users/kevin/IdeaProjects/apiease-template/docs/apex-liquid-runtime-directives.md).

Agents working on Liquid requests should read that file before generating or modifying APIEase Liquid.

## Project Goals
- Build APIEase resources for a real client implementation.
- Preserve working runtime behavior in APIEase over generic Liquid assumptions.

## Preferred Patterns
- Treat [docs/apex-liquid-runtime-directives.md](/Users/kevin/IdeaProjects/apiease-template/docs/apex-liquid-runtime-directives.md) as required guidance for Liquid authoring.
- Prefer defensive Liquid patterns that match observed APIEase runtime behavior.

## Constraints
- Do not use Liquid filters directly inside `if` comparisons.
- Do not dereference nested response properties until key presence has been confirmed.

## Workflow Notes
- Add new APIEase runtime lessons to [docs/apex-liquid-runtime-directives.md](/Users/kevin/IdeaProjects/apiease-template/docs/apex-liquid-runtime-directives.md) so Apex and other agents can reuse them.
