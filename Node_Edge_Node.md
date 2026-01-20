# Node–Edge–Node

In the context of a knowledge graph, the terms **node**, **edge**, and the relationship **node–edge–node** are fundamental concepts.

## Node (Entity)

- Nodes represent real-world entities or concepts.
- These can be:
  - Concrete objects (e.g., "Lionel Messi", "Eiffel Tower")
  - Abstract concepts (e.g., "Football", "Democracy")
  - Events (e.g., "World War II")
- Each node represents a unique entity.
- Nodes can have associated properties (attributes) that describe them, such as:
  - Name
  - Age
  - Occupation

## Edge (Relationship)

- Edges represent the relationships or connections between nodes.
- They describe how different entities are related to each other.
- Edges are typically directed, indicating the nature and direction of the relationship.
- Examples of relationships:
  - "is a captain of"
  - "is located in"
  - "wrote"
- Edges can also have properties, such as:
  - Start date
  - End date of a relationship

## Node–Edge–Node (Triple)

- This structure forms the basic building block of a knowledge graph.
- It describes a specific relationship between two entities.
- A common representation is:
  - **subject–predicate–object**
  - **head entity–relationship–tail entity**

### Components

- **Subject / Head Entity**: The node from which the relationship originates.
- **Predicate / Relationship**: The edge defining the type of relationship.
- **Object / Tail Entity**: The node to which the relationship points.

## Example

Consider the statement:

> "Lionel Messi is a captain of Argentina Football Team."

| Component | Value |
|---------|-------|
| Node 1 (Subject) | Lionel Messi |
| Edge (Predicate) | is a captain of |
| Node 2 (Object) | Argentina Football Team |

This node–edge–node structure allows for the representation of complex, interconnected information in a structured and machine-readable format, enabling tasks like querying, inferring new relationships, and building intelligent applications.

## Reference

https://docs.stardog.com/tutorials/rdf-graph-data-model

## RDF Graphs

- A directed graph is a set of objects, usually called **nodes**, connected together by lines, usually called **edges**.
- The edges are **directed** from one node to another.
- Edges are directional and can be thought of as arrows (`→`).
- An edge points from one node to another node.



# RDF Graphs

A **directed graph** is a set of objects, usually called **nodes**, connected by lines, usually called **edges**, that are **directed** from one node to another.

- Edges are directional and can be thought of as arrows (`→`)
- Each edge points from one node to another node

---

# RDF Terminology

In RDF, graph components are defined as follows:

- **Edge** → *Triple*
- **Source node** → *Subject*
- **Edge name** → *Predicate*
- **Target node** → *Object*

A node can appear:
- As a **subject** in one triple
- As an **object** in another triple

---

# RDF Graph Definition

An **RDF graph** is defined as a **set of RDF triples**.

Key characteristics:

- Nodes are **not declared separately**
- Nodes are **implicitly defined by the edges (triples)**
- An RDF node **cannot exist without participating in at least one triple**

This definition closely matches the informal notion of a directed graph, with the key constraint that nodes only exist through their relationships.
