# Global Prompt Engineering Principles

Prompt engineering is the practice of designing inputs that reliably guide Large Language Models (LLMs) toward high-quality, predictable outputs.

This document defines universal principles that apply across models such as ChatGPT, Claude, and Gemini.

## Core Principle: Explicitness Over Assumption
LLMs do not infer intent reliably. Any ambiguity forces the model to guess.

Always prefer:
- Explicit roles
- Explicit tasks
- Explicit constraints
- Explicit output formats

## Determinism vs Creativity
- More constraints = more deterministic output
- Fewer constraints = more creative but less predictable output

Prompt optimization is the act of finding the optimal balance for a given task.

## Instruction Hierarchy
LLMs tend to follow instructions in this order:
1. System-level instructions
2. Explicit task definitions
3. Constraints
4. Examples
5. Implicit cues

Well-structured prompts align all layers.

## Prompt Engineering Is Iterative
High-quality prompts are refined through:
- Generation
- Evaluation
- Revision

One-shot prompting is rarely optimal for complex tasks.

## Positive Instruction Bias
LLMs follow positive instructions more reliably than negative ones.

Prefer:
"Include X, follow Y"

Avoid:
"Do not do Z"
