# Vocabulary Implementation Requirements {#vocabulary-implementation-requirements}

The following vocabulary requirements complement those in the core xAPI specification and have been expanded to reflect the new responsibilities of creating and publishing xAPI vocabularies as linked datasets.

| **Requirement Number** | **Description** | **Conformance Level** |
| --- | --- | --- |
| 1 | Anyone establishing new vocabulary datasets or vocabulary terms **SHOULD** first check xAPI community resources (e.g., registries, repositories) to see if existing terms already exist to avoid duplication. | **SHOULD** |
| 2 | Anyone establishing new vocabularies and new vocabulary terms for xAPI **MUST** use HTTP IRIs so that they can be resolved/dereferenced. | **MUST** |
| 3 | Anyone establishing new vocabularies **SHOULD** use persistent and well-designed IRIs so that they can be stable for long term reliability. See the [IRI Design and Persistence Section](vocabulary_development_and_publishing/iri_design_and_persistence.md) of this document for guidelines. | **SHOULD** |
| 4 | Anyone creating new vocabulary terms **MUST** provide descriptive metadata by minimally using the recommended classes and properties in this specification, and associate the terms with a vocabulary (concept scheme). | **MUST** |
| 5 | Vocabulary datasets **SHOULD** contain additional provenance metadata about the authors, version, date created, and date last modified. | **SHOULD** |
| 6 | Authors **MAY** also express relationships between terms using SKOS. | **MAY** |
| 7 | Anyone establishing a new vocabulary **MUST** publish a human-readable representation of the vocabulary dataset as HTML accessible at the IRI. | **MUST** |
| 8 | Anyone establishing a new vocabulary **MUST** publish at least one additional machine-readable representations of the vocabulary dataset in RDF (e.g., RDFa,JSON-LD,Turtle). | **MUST** |
| 9 | If multiple representations exist, vocabulary authors **SHOULD** provide a means of discovering each of the available dataset representations through content negotiation. | **SHOULD** |
| 10 | Anyone publishing a vocabulary dataset **SHOULD** announce the availability of the vocabulary and submit it to xAPI community resources (e.g., registries, repositories). | **SHOULD** |
| 11 | Repositories, registries, or any other systems that publish xAPI vocabulary datasets expressed as RDF **SHOULD** provide a public SPARQL endpoint for querying that data. | **SHOULD** |
| 12 | Since vocabularies can change, a system aggregating vocabularies **SHOULD** have a process to keep their versions up to date. | **SHOULD** |

Figure 9\. Table of xAPI vocabulary requirements.