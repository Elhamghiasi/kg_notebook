## What is SPARQL Query Generation?

**SPARQL query generation** is the process of **automatically creating SPARQL queries** from more human-friendly inputs, such as:

- Natural language questions
- Structured templates
- Prompts given to large language models (LLMs)

The goal is to translate *what a user wants to know* into a **valid SPARQL query** that can be executed over a **knowledge graph (RDF data)**.

---

## Why SPARQL Query Generation Is Needed

Humans typically ask questions in **natural language**, while knowledge graphs are queried using **SPARQL**.  
SPARQL query generation acts as a **bridge** between these two representations.

---
### Natural Language Question → SPARQL Query → Knowledge Graph → Answer


---

## Example

**Natural language question:**
> Which universities are located in Ohio?

**Generated SPARQL query:**
```sparql
SELECT ?university
WHERE {
  ?university rdf:type ex:University .
  ?university ex:locatedIn ex:Ohio .
}
