# 🧠 Promptable
**Open-Source artefact for Prompt Optimization**

![status](https://img.shields.io/badge/status-stable-green)
![license](https://img.shields.io/badge/license-MIT-blue)
![contributions](https://img.shields.io/badge/contributions-welcome-brightgreen)

## 📌 Overview

**Promptable** is an open-source artefact designed to **analyze, rewrite, and optimize prompts** for Large Language Models (LLMs).

It transforms vague, ambiguous, or poorly structured prompts into **clear, explicit, and reliable prompts**, while **strictly preserving the original intent**.

The project focuses on **automation**, **prompt quality**, and **production-grade reliability**, rather than prompt “tricks” or hacks.

## 🎯 Goals

- Improve prompt clarity and consistency
- Reduce ambiguity and hallucinations
- Enforce structure, constraints, and output formats
- Adapt prompts to specific LLMs (ChatGPT, Claude, Gemini)
- Enable automated prompt optimization pipelines
- Provide a reusable open-source knowledge base for prompt engineering

## 🤖 Supported Models

- ChatGPT (OpenAI)
- Claude (Anthropic)
- Gemini (Google)

If no target model is specified, prompts are optimized using **model-agnostic best practices**.

## 🏗️ Architecture

The system is composed of **two complementary layers**:

### 1. System Prompt (Control Layer)

Defines:
- The role of the GPT
- Optimization rules
- Model-specific adaptations
- Output formatting rules
- Edge-case handling

This layer acts as the **reasoning engine**.

### 2. Knowledge Base (Expert Memory)

A curated, structured collection of prompt engineering knowledge used to:
- Detect prompt anti-patterns
- Select optimization techniques
- Apply best practices consistently
- Support long-term evolution of the system


## 📚 Knowledge Base Structure

```bash
/knowledge_base
│
├── 00_global_prompt_engineering_principles.md
├── 01_prompt_anatomy_and_structure.md
├── 02_prompt_optimization_heuristics.md
├── 03_prompt_anti_patterns.md
│
├── 10_chatgpt_prompt_engineering.md
├── 11_claude_prompt_engineering.md
├── 12_gemini_prompt_engineering.md
│
├── 20_reasoning_and_chain_of_thought.md
├── 21_prompt_chaining_and_decomposition.md
├── 22_meta_prompting_and_reflection.md
│
├── 30_output_formats_and_schemas.md
├── 31_constraints_and_control.md
│
├── 40_prompt_templates_core.md
├── 41_prompt_templates_optimization.md
│
├── 50_prompt_evaluation_and_quality_checks.md
├── 51_automated_prompt_optimization_workflows.md
│
└── 99_glossary_and_definitions.md
```

Each file is:
- Focused on a single concept
- Action-oriented
- Optimized for retrieval (RAG-friendly)
- Written in clear, technical English

## 🧠 How Prompt Optimization Works

1. **Prompt Analysis**
   - Identify ambiguity
   - Detect missing context, constraints, or output format
   - Detect known anti-patterns

2. **Knowledge Retrieval**
   - Relevant techniques are retrieved from the knowledge base

3. **Prompt Rewriting**
   - Apply structure: role, task, context, constraints, output format
   - Adapt to the target LLM if specified

4. **Optional Validation**
   - Self-critique
   - Variant generation
   - Constraint compliance checks

## 🧪 Example

### Input Prompt

```
Write something about AI for marketing.
```

### Optimzed Prompt

```
You are a marketing content specialist.

TASK:
Write a concise marketing article introducing artificial intelligence to a non-technical audience.

CONSTRAINTS:
- Tone: professional and approachable
- Length: 300–400 words
- Avoid technical jargon

OUTPUT FORMAT:
Markdown with headings and bullet points.
```

## 🔧 Installation & Usage

### Using as a Custom GPT

1. Create a new Custom GPT
2. Paste the provided **System Prompt** into the Instructions section
3. Upload all files from `/knowledge_base` as Knowledge
4. Save and test

### Using as a Knowledge Base (RAG)

- Ingest Markdown files into a vector database
- Use them as retrieval context for any LLM-based system

## 🧠 Extending the Knowledge Base

### What to Add

- New prompt engineering techniques
- Model-specific behaviors
- New prompt templates
- Prompt anti-patterns discovered in practice

### What NOT to Add

- Raw articles or blog posts
- Prompt “hacks” without generalization
- Marketing content
- Unstructured notes

**Contribution rule:**

> Store distilled expertise, not documentation dumps.

## 🤝 Contributing

Contributions are welcome.

You can:
- Improve existing documentation
- Add new techniques or templates
- Add support for new models
- Improve evaluation workflows

### Contribution Guidelines

- One concept per file or section
- Clear, neutral, technical language
- Actionable guidance only
- No model hype or speculation

## 🧪 Testing Philosophy

Prompt quality is evaluated based on:
- Clarity
- Determinism
- Constraint compliance
- Reusability
- Automation readiness

Testing is done through:
- Prompt rewrites
- Cross-model comparisons
- Failure analysis

## 🛡️ Design Principles

- Explicit over implicit
- Structure over improvisation
- Reliability over cleverness
- Automation over manual tweaking

## 📜 License

This project is released under the **MIT License**.

You are free to:
- Use
- Modify
- Distribute
- Embed in commercial systems

Attribution is appreciated but not required.

## 🚀 Roadmap

- Add support for new LLMs
- Add prompt linting rules
- Add benchmark prompt datasets
- Add automated evaluation scripts

## 📬 Contact / Maintainers

This project is community-driven.  
Open an issue or pull request to contribute.

### ⭐ If this project helps you, consider starring the repository
