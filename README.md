# Large-Language Model Bias Ontology

This repository maintains the Large-Language Model Bias Ontology (LLaMBO) artifact extended from and is conformant to the Basic Formal Ontology (BFO) as specified in [ISO/IEC 21838‑1](https://www.iso.org/standard/71954.html) for top-level ontologies. Because BFO is used as a top-level architecture by numerous ontologies in the Open Biomedical and Biomedical Ontologies (OBO) Foundry, the Industrial Ontologies Foundry (IOF), and the Common Core Ontologies (CCO) suite, ontologies conformant to BFO promote interoperability, standardization, and reuse among domain-level ontologies. 

In addition to extending BFO, LLaMBO extends directly from modules in [CCO](https://github.com/CommonCoreOntology/CommonCoreOntologies), in particular those pertaining to information and measurement. 

The most current version is the "llambo.owl" file located in the root directory of this repo. 

## Development Team
* [John Beverley](https://www.buffalo.edu/cas/philosophy/faculty/faculty_directory/john-beverley.html)
* [Mark Jensen](https://github.com/mark-jensen)
* [Cameron More](https://github.com/cameronmore)

## Large-Language Model Bias Ontology Hierarchy
```mermaid
graph LR
    A(Entity):::BFO --> B(Continuant)
    B(Continuant):::BFO --> D(Specifically Dependent<br> Continuant)
    B(Continuant) --> E(Generically Dependent<br> Continuant):::BFO
    B(Continuant) --> F(Independent<br> Continuant)
    F(Independent<br> Continuant):::BFO --> G(Material Entity):::BFO
    D(Specifically Dependent<br> Continuant):::BFO --> J(Realizable<br> Entity):::BFO
    J(Realizable<br> Entity):::BFO --> L(Role):::BFO
    J(Realizable<br> Entity):::BFO --> M(Disposition):::BFO
    M(Disposition):::BFO  --> N(Function):::BFO
    A(Entity):::BFO --> C(Occurrent):::BFO
    C(Occurrent):::BFO --> AA(Process):::BFO

    classDef BFO fill:#F5AD27,color:#060606

  ```
