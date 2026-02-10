# Prompt Anatomy and Structure

A reliable prompt follows a clear internal structure.

## Core Components

### Role
Defines who the model is supposed to be.
Example:
"You are an expert prompt engineer."

### Task
Defines what the model must do.
Example:
"Rewrite the following prompt to improve clarity."

### Context
Provides background information needed to perform the task correctly.

### Constraints
Rules that limit or guide the output:
- Tone
- Length
- Style
- Forbidden content
- Required elements

### Output Format
Defines how the response must be structured.
Examples:
- JSON
- Markdown
- Bullet points
- Tables

## Why Structure Matters
Without structure:
- The model must infer priorities
- Outputs vary significantly
- Automation becomes unreliable

Structured prompts reduce cognitive load and improve consistency.

## Common Structural Failures
- Missing output format
- Implicit role assumptions
- Mixed or conflicting tasks
- Overloaded instructions
