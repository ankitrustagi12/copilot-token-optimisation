# copilot-token-optimisation

A reusable repository for reducing token usage in AI-assisted development, including spec-driven workflows and general instruction patterns that can be copied into any project.

## What this repo is for

This repo helps teams and individual developers:
- write smaller, clearer prompts,
- structure specs so AI tools use fewer tokens,
- reuse instruction templates across projects,
- create consistent developer workflows for Copilot and other AI assistants.

## Core ideas

1. Prefer one objective per prompt.
2. Put reusable rules in files, not in chat.
3. Keep specs short, structured, and predictable.
4. Separate must-have constraints from nice-to-have guidance.
5. Ask for outputs in the smallest useful format.

## How to use in any project

1. Clone or copy this repo into your project workspace.
2. Reuse the files under `docs/instructions/` as your prompt and spec standards.
3. Start each feature with the template in `templates/spec-prompt-template.md`.
4. Review large prompts with `templates/review-checklist.md` before sending them.
5. Keep one source of truth for rules and naming.

## Repo structure

```text
copilot-token-optimisation/
├── README.md
├── LICENSE
├── docs/
│   └── instructions/
│       ├── speckit-token-optimization.md
│       └── general-token-optimization.md
├── examples/
│   ├── java/
│   │   └── prompt-example.md
│   └── spring-boot/
│       └── spec-example.md
└── templates/
    ├── spec-prompt-template.md
    └── review-checklist.md
```

## Spec-driven development approach

Use this structure:
- Problem statement
- Scope
- Non-goals
- Constraints
- Expected output
- Acceptance criteria

This reduces prompt size, removes repetition, and improves response consistency.

## Token optimization principles

- Avoid long context dumps.
- Replace repeated explanations with links to project docs.
- Use bullet points instead of long paragraphs.
- Use precise task names.
- Reuse standard templates.
- Ask the model to respond only with the required artifact.
- Separate planning, coding, and review into different prompts.

## Example prompt pattern

```text
Task: Generate a service method for invoice validation.
Context: Java 17, Spring Boot, existing validation layer.
Constraints: No new dependencies. Follow current naming conventions.
Output: Only the code and a short explanation.
```

## Who can use this

- Developers using GitHub Copilot or other AI coding assistants.
- Teams standardizing prompt structure across repositories.
- Engineering managers creating reusable internal AI usage guidelines.
- Open source maintainers who want a lightweight, portable instruction pack.

## Contribution rules

- Keep guidance reusable.
- Prefer short examples.
- Avoid tool-specific lock-in unless clearly marked.
- Keep templates portable across projects.

## License

This repository includes an MIT License so that it can be reused across projects and by other contributors.
