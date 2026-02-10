# Prompt Anti-Patterns

Anti-patterns are prompt designs that consistently produce poor results.

## Vague Prompts
Example:
"Write something about AI."

Why it fails:
- No scope
- No goal
- No output expectations

Fix:
Add task, scope, and format.

## Conflicting Instructions
Example:
"Be concise and extremely detailed."

Fix:
Clarify priority or choose one constraint.

## Missing Output Format
Why it fails:
The model must guess structure.

Fix:
Always specify format when automation is involved.

## Overloaded Prompts
Too many tasks in a single instruction reduce reliability.

Fix:
Split into chained prompts.
