---
title: Diagrams drawing
summary: Description of draw.io and mermaid
slug: an-slug
project-tags: 
  - self education
thematic-tags:
  - documentation
  - drawing
  - diagrams
---

# Diagrams drawing

*Description of draw.io and mermaid*

---
**Diagramming** => placing a number of diagram elements, connect them together, add descriptive text, and style the elements to convey more complex information visually

## Draw.io

Open source project for creating diagrams and ilustrations

- [Project page](https://www.drawio.com/)
- [Online editor](https://app.diagrams.net/)

Enable to create variety of diagrams:
- flow charts
- mind maps
- org charts
- Venn diagrams
- infographics
- network and architecture diagrams
- floor plans
- electrical and rack diagrams, UML diagrams

Software development related drawings:
- [UML diagrams](https://www.drawio.com/blog/uml-2-5.html)
- [entity relationship tables for database modelling](https://www.drawio.com/blog/entity-relationship-tables.html)
- [Mermaid diagrams](https://www.drawio.com/blog/mermaid-diagrams.html)
- [Gitflow diagrams](https://www.drawio.com/blog/gitflow-diagram)

All drawn images can be exported to multiple formats and stored in git repository

Example drawn by draw.io:

<div style="background-color: lightblue; display: inline-block;">
  <img src="../assets/draw.io-diagram.svg" alt="Diagram" />
</div>


## Mermaid diagrams
**Mermaid lets you create diagrams and visualizations using text and code.**
- they can be utilized in markdown documents
- they can be stored in git repositories
- they are rendered by gitlab/github
- there are addons for IDEs, that can display mermaid images

### Resources:
- [Mermaid live editor](https://mermaid.js.org/intro/syntax-reference.html#mermaid-live-editor)
- [Mermaid documentation](https://mermaid.js.org/)

### Examples
```mermaid
mindmap
Root ))import((
    A[named import] 
    B[default import]
    C[namespace import]
    D[side effect import]
```
```mermaid
---
title: Mermaid example generated by AI
---
erDiagram
    MEMBER {
        int MemberID PK
        string Name
        string Email
        date JoinDate
    }
    BOOK {
        int BookID PK
        string Title
        string Author
        int PublishedYear
    }
    LOAN {
        int LoanID PK
        int BookID FK
        int MemberID FK
        date LoanDate
        date ReturnDate
    }
    MEMBER ||--o{ LOAN : borrows
    BOOK ||--o{ LOAN : "is borrowed by"
```