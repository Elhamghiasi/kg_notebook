# Knowledge Graphs — Basic Definition

## What is a Knowledge Graph?

A **Knowledge Graph (KG)** is a way to represent knowledge in a **structured, connected, and machine-readable** form.

At its core, it is a **graph**:
- **Nodes** represent entities (things)
- **Edges** represent relationships between entities

A knowledge graph stores facts explicitly rather than implicitly in text.

---

## Core Building Blocks

### 1. Entities (Nodes)
Entities are real or conceptual things in the domain.

Examples:
- Publication  
- Author  
- Agent  
- Department  
- University  

Each entity belongs to a **class/type**.

---

### 2. Relationships (Edges)
Relationships describe how entities are connected.

Examples:
- `submittedBy`
- `performedRole`
- `worksInDepartment`
- `partOfUniversity`

Relationships are **directed** and meaningful.

---

### 3. Attributes (Data Properties)
Attributes store literal values associated with entities.

Examples:
- `hasTitle → "A Study on Knowledge Graphs"`
- `hasEmail → "user@university.edu"`
- `dateOfSubmission → 2024-10-01`

---

## RDF Triples

Knowledge in a KG is represented as **triples**:
(subject) — (predicate) — (object)

Publication123 — submittedBy — Author456


This states a factual relationship between two entities.

---

## Ontology vs Knowledge Graph

### Ontology
- Defines the **schema** or structure
- Specifies:
  - Classes (e.g., Publication, Author, Agent)
  - Relationships (e.g., submittedBy, worksIn)
  - Constraints on valid connections

Ontology represents the **rules**.

---

### Knowledge Graph
- Contains the **instance data**
- Includes concrete entities and relationships
- Must conform to the ontology

Knowledge graph represents the **facts**.

---

## Why Knowledge Graphs Matter

Knowledge graphs:
- Make knowledge **explicit**
- Support **explainable reasoning**
- Reduce ambiguity and hallucination
- Enable precise querying using **SPARQL**
- Integrate well with **LLMs for grounded question answering**

---

## Summary

A knowledge graph is a structured network of entities and relationships, defined by an ontology, stored as triples, and designed to make knowledge explicit, queryable, and explainable.




