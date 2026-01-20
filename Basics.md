# My Learning Guide  
## Concepts I Am Working On

---

## Concept 1: What Is a Knowledge Graph?

A **Knowledge Graph (KG)** is a way to store knowledge as:
- **Things (nodes)**  
- **Connections between them (edges)**

### Core Terminology
- **Entities** → the “things” (nodes)
- **Relations** → the “connections” (edges)

---

## Structure of the Selected Knowledge Graph

The selected KG is a network of:

### 1. Entities (Classes)
Examples:
- `Publication`
- `Author`
- `Agent`
- `Department`
- `College`
- `University`
- `Role`

### 2. Relationships (Object Properties)
Examples:
- `submittedBy`
- `contributionBy`
- `performedRole`
- `worksInDepartment`
- `departmentOf`
- `collegeOf`

### 3. Attributes (Datatype Properties)
Values such as strings, dates, and integers:
- `hasTitle`
- `hasAbstract`
- `dateOfSubmission`
- `hasEmailAddress`

---

## RDF Triples

All knowledge is encoded as **triples**:


- `(entity) – (relationship) – (entity or value)`

---

## Examples Based on My Schema

### Example 1: A Publication Submitted by an Author

```ttl
:Publication123   :submittedBy   :Author456

:Publication123   :hasTitle         "A Review of Knowledge Graphs"
:Publication123   :hasAbstract      "This paper studies..."
:Publication123   :dateOfSubmission "2025-01-15"^^xsd:date
:Publication123   :hasDOI           "10.1000/xyz123"



