# KG + LLM + Prompt Engineering

This project explores how **Large Language Models (LLMs)** can answer natural language questions over a **Knowledge Graph (KG)** by understanding an ontology and generating correct **SPARQL queries**.

---

## Example Natural Language Questions

The LLM is given questions such as:

- Who submitted this publication?
- When was Publication `xxx` posted?
- Which department does the author work in?
- Which college is the Computer Science department part of?

---

## What the LLM Must Do

To answer these questions correctly, the LLM must:

1. **Understand the ontology structure**
   - For example:
     - `Author` is **not** the person
     - `Author → performedBy → Agent`

2. **Convert the natural language question into a SPARQL query**

3. **Execute the query over the Knowledge Graph**

4. **Retrieve the correct answer from the KG**

---

## Example Walkthrough

### Question

> What is the title of Publication `xxx`?

### Expected Behavior

- Identify `Publication` as an entity in the ontology
- Recognize `hasTitle` as the relevant datatype property
- Generate the appropriate SPARQL query
- Retrieve the title value from the Knowledge Graph

---

## Key Concepts

- **Knowledge Graph (KG)**  
  Structured knowledge represented as entities and relationships

- **Ontology-Aware Reasoning**  
  The LLM must reason over ontology constraints and paths, not surface text

- **Prompt Engineering**  
  Prompts are designed to guide the LLM to:
  - Interpret ontology structure
  - Generate valid SPARQL queries
  - Avoid incorrect entity assumptions

---

## Goal

Evaluate how effectively an LLM can:
- Understand an ontology
- Translate natural language questions into SPARQL
- Retrieve accurate answers from a Knowledge Graph
