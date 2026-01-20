# Large Language Models (LLMs) — Learning Notebook

## What Are Large Language Models?

Large Language Models (LLMs) are AI systems trained to understand and generate human-like text.

They work by:
- Predicting the next token in a sequence
- Using the context of previous tokens
- Learning patterns from massive text datasets

### Examples
- GPT-4
- Gemini
- Claude
- LLaMA
- Mistral

---

## Core Concepts

| Concept | Meaning |
|------|------|
| Token | The smallest text unit the model reads (word, subword, or character). |
| Embedding | Numerical representation of tokens that capture semantic meaning. |
| Parameters | Model’s internal weights (LLMs have billions). |
| Context Window | How many tokens the model can see at once. |
| Fine-tuning | Additional training to specialize a model on new data or tasks. |
| Prompt | Input text given to guide the model’s response. |

---

## What LLMs Can Do

### Text Generation
- Writing
- Summarizing
- Translating
- Explaining

### Reasoning (Limited)
- Logic problems
- Basic math

### Coding
- Writing code
- Explaining code

### Knowledge Retrieval
- Answering questions based on learned patterns
- Using external data via RAG (Retrieval-Augmented Generation)

---

## Limitations

- LLMs do not truly understand facts; they predict text patterns.
- They can hallucinate incorrect but confident information.
- Outputs are highly sensitive to prompt wording.
- Training and inference are compute-intensive (GPUs/TPUs).

---

## Interacting with LLMs via APIs

When designing and testing prompts, interaction with LLMs typically happens through APIs.

APIs allow control over:
- Model behavior
- Randomness
- Output style and length

Tuning often requires trial and error.

---

## Key Generation Setting: Temperature

### Temperature

Temperature controls how predictable or creative the model’s output is.

- **Low temperature**
  - More deterministic
  - Best for factual or precise tasks

- **High temperature**
  - More random and creative
  - Best for storytelling or brainstorming

**Rule of thumb:**
- Low temperature → accuracy
- High temperature → creativity

---

## Summary

- LLMs generate text token by token using context.
- Core concepts include tokens, embeddings, parameters, and prompts.
- API settings strongly influence outputs.
- Careful prompt and parameter design is essential.
