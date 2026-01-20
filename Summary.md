# Knowledge Graph & LLM–SPARQL Summary

## Core Concepts

- **Knowledge Graph (KG)** = entities such as `Publication`, `Author`, `Agent`, `Department`, `College`, `University`, `Role`.
- **Triples** = small factual statements in the form:


Example:
- **Attributes (datatype properties)** = literal values such as:
- `hasTitle`
- `hasAbstract`
- `dateOfSubmission`

- **Roles** connect people to what they do:


- **LLM requirement**:
- Must strictly follow the ontology.
- Must generate correct SPARQL queries using only defined relations.
- **Never invent new properties or classes.**

- **Prompting rule**:
> “Use only these relations; never invent new ones.”

---

## Writing NEN Triples (Node–Edge–Node)

### Conceptual View

- One **Publication node**
- Many **small facts** attached to it via:
- edges to literal values, or
- edges to other entities

### Step-by-step

---

## Publication Properties

```text
Publication → hasVolumeNumber → xsd:int
Publication → hasIssueNumber → xsd:int
Publication → hasArticleNumber → xsd:int
Publication → hasDOI → xsd:string
Publication → associatedFieldOfStudy → xsd:string
Publication → dateOfSubmission → xsd:date
Publication → dateOfPost → xsd:date
Publication → dateOfPublication → xsd:date
Publication → publicationState → xsd:string
Publication → dateOfPublicationStateChange → xsd:date
Publication → hasPublicationType → xsd:string
Publication → dateOfPublicationsStateChange → xsd:date
Publication → hasTitle → xsd:string
Publication → hasAbstract → xsd:string
Publication → contributionBy → xsd:string
Publication → hasAdvisor → xsd:string
Publication → submittedBy → Author

```
##  Author Properties

```text
Author → advisedBy → xsd:string
Author → isSubclassOf → Role
```
## Agent Properties

```text
Agent → performsRole → Role
Agent → worksInDepartment → Department
Agent → hasPhoneNumber → xsd:string
Agent → hasEmailAddress → xsd:string
Agent → hasFirstName → xsd:string
Agent → hasFamilyName → xsd:string

```
## Organizational Structure

```text
Department → departmentOf → College
College → collegeOf → University
University → atState → xsd:string
University → atCity → xsd:string

```


