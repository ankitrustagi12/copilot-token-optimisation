# Spec-driven token optimization

## Goal
Create specs that are easy for AI tools to process with minimal token waste.

## Why this works
Spec-driven development reduces token usage because it forces the task into stable, repeatable sections. Instead of rewriting context every time, you define the same structure once and keep only the task-specific details variable.

## Rules
- Write one feature per spec.
- State the goal in one sentence.
- Keep background to only what changes the outcome.
- Put constraints in a dedicated section.
- Use acceptance criteria instead of long explanations.
- Avoid duplicating the same rule in multiple places.
- Prefer examples only when they clarify edge cases.
- Use consistent headings across all specs.

## Recommended spec format
- Title
- Objective
- Scope
- Non-goals
- Constraints
- Dependencies
- Acceptance criteria
- Example input/output
- Open questions

## Prompt style
- Be explicit about the output.
- Ask for only one artifact at a time.
- Keep references short and stable.
- Use repository docs as the source of truth.
- Tell the model what not to return when needed.

## Anti-patterns
- Large copy-pasted context blocks.
- Repeating architecture details in every prompt.
- Vague requests like "improve this".
- Mixing planning, coding, and review in one prompt.
- Attaching unnecessary logs, stack traces, or old chat history.

## Reusable workflow
1. Create a short spec.
2. Validate scope and non-goals.
3. Ask for one output only.
4. Review response against acceptance criteria.
5. Use a second prompt only for corrections.
