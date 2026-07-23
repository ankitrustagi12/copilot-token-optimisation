# General token optimization

## Goal
Reduce token usage in AI conversations without losing important context.

## Rules
- Use concise prompts.
- Prefer structured bullets over paragraphs.
- Put reusable context in files.
- Reference docs instead of rewriting them.
- Ask for only the needed depth.
- Split large tasks into smaller steps.
- Remove duplicate instructions.
- Keep examples short.
- Avoid asking for unnecessary explanations.

## Good patterns
- "Summarize this diff in 5 bullets."
- "Generate only the method body."
- "Compare these two approaches with pros and cons."
- "Refactor this class without changing behavior."
- "Return only the SQL query."

## Bad patterns
- "Explain everything in detail."
- "Consider every possible edge case and rewrite the whole design."
- "Here is all the background again..." repeated in each prompt.
- "Optimize this" without constraints or target output.

## Practical instruction design
- Put project standards in a repo file.
- Keep prompts task-specific.
- Prefer deterministic output formats.
- Ask for markdown, code, or JSON only when truly needed.
- Reuse the same headings across tasks.

## Minimal prompt recipe
- Task
- Context
- Constraints
- Output format
- Done criteria
