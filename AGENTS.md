# Instructions for AI Agents

## Project Context

This repository is part of the openBIM ecosystem of buildingSMART International, supporting open, vendor-neutral, and interoperable digital workflows for the built environment.

AI agents contributing to this project must prioritise correctness, maintainability, interoperability, and alignment with applicable buildingSMART International standards.

Before making changes, read the repository's [README](./README.md), [Contributing Guidelines](./CONTRIBUTING.md) (particularly on [AI Assisted Contributions](./CONTRIBUTING.md#ai-assisted-contributions)), and relevant technical documentation to understand the project's purpose, architecture, and conventions.

Follow any additional project-specific documentation and instructions relevant to the task.

## General Principles

- **Make minimal, focused changes.** Avoid unrelated modifications, unnecessary refactoring, or introducing dependencies without justification.
- **Follow existing conventions.** Respect the repository's architecture, naming conventions, coding style, and established patterns.
- **Prefer clarity over complexity.** Produce readable, maintainable code and documentation.
- **Preserve compatibility.** Avoid breaking existing APIs, schemas, data structures, or supported workflows unless explicitly requested.
- **Do not invent requirements.** When specifications or expected behaviour are unclear, identify the ambiguity rather than making unsupported assumptions.
- **Respect human oversight.** Propose significant architectural, semantic, or normative changes for maintainer review.

## openBIM Standards and Interoperability

When working with openBIM-related functionality:

- Follow the applicable buildingSMART standards and their specified versions, including IFC, IDS, BCF, and bSDD, where relevant.
- Use official specifications and documentation as authoritative references: [buildingSMART Standards](https://www.buildingsmart.org/standards/).
- Preserve the intended semantics of standardised entities, attributes, relationships, classifications, and identifiers.
- Do not introduce vendor-specific assumptions or dependencies that unnecessarily restrict interoperability.
- Maintain compatibility with existing standard-compliant implementations and data exchanges.
- Do not silently modify schemas, validation rules, or expected interpretations of standards.
- Distinguish between normative requirements, implementation decisions, and recommendations.

**AI agents must not independently redefine or reinterpret buildingSMART standards.** 
Potential ambiguities, inconsistencies, or proposed normative changes must be raised for human review.

## Development Workflow

Before modifying code:

1. Review the relevant source files, tests, and documentation.
2. Identify existing implementations or utilities that can be reused.
3. Determine the smallest change that addresses the task.
4. Consider the impact on compatibility, interoperability, and existing users.

When implementing changes:

- Follow the programming language and tooling conventions already established in the repository.
- Avoid introducing new frameworks, libraries, or architectural patterns without clear justification.
- Keep changes scoped to the requested functionality.
- Update relevant documentation when behaviour or interfaces change.
- Do not modify generated files manually unless explicitly required by the project.

## Testing and Validation

AI agents should verify their changes using the repository's existing testing and validation tools.

- Run relevant tests, linters, formatters, and type checks where available.
- Add or update tests when introducing or changing functionality.
- Include regression tests for bug fixes where practical.
- Test relevant edge cases, including invalid, incomplete, or unexpected input.
- For openBIM data processing, use representative standards-compliant test data where available.
- Never modify tests solely to conceal a defect or make failing behaviour appear correct.
- Clearly report any tests that could not be executed and explain why.

Do not claim that changes have been tested or validated unless the corresponding checks were actually performed.

## Documentation

- Use clear, precise, and technically accurate language.
- Follow existing documentation structure and terminology.
- Use official buildingSMART terminology consistently.
- Reference relevant standards, specifications, or repository issues where appropriate.
- Provide examples when they improve understanding.
- Do not present assumptions, experimental behaviour, or implementation-specific limitations as normative requirements.

## Security and Data Protection

- Never expose secrets, credentials, tokens, or confidential information.
- Avoid introducing insecure dependencies or unsafe data-handling practices.
- Treat external files, model data, and user input as potentially untrusted.
- Do not upload or transmit repository contents or user data to external services unless explicitly authorised.
- Report suspected security vulnerabilities through the designated private reporting process following [SECURITY.md](./SECURITY.md).

## Contributions and Pull Requests

When preparing changes for review:

- Provide a concise summary of what changed and why.
- Reference related issues or specifications where relevant.
- Highlight potential breaking changes, compatibility concerns, or limitations.
- Describe the tests and validation performed.
- Clearly identify unresolved questions or decisions requiring maintainer input.
- Follow the repository's `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md`.

Do not merge pull requests, publish releases, or make other consequential repository changes without explicit authorisation.

## Naming conventions

- Official spelling of the keywords is:  `buildingSMART` (or `bSI` in short), `openBIM`, `bSDD`, `IFC`, `IDS`, `BCF`, `mvdXML`, `Validation Service`, `IFCX`, `openBIM API`.
- Versioning of the standards should follow SemVer, and be separated with one whitespace. For example: `IFC 4.3.2`, `IDS 1.1`, `IFCX 0.1`.

## When in Doubt

If a task involves unclear requirements, conflicting specifications, potentially breaking changes, or decisions affecting openBIM interoperability:

1. Do not guess or invent expected behaviour.
2. Consult existing documentation, specifications, and tests.
3. Explain the uncertainty and possible implications.
4. Request clarification or human review before proceeding.

**The primary objective is to support reliable, interoperable, and maintainable openBIM standards.**
