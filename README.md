# Companion Specification for xAPI Vocabularies {#companion-specification-for-xapi-vocabularies}

Companion Specification for Experience API (xAPI) Vocabularies

![logo](assets/logo.png)

December 2015

DRAFT v.1.0 PROPOSAL

(send questions or feedback to: xapi-vocabulary@adlnet.gov)

Table of Contents

1.  [Status of this Document](export/status_of_this_document.md)
2.  [License](export/license.md)
3.  [Introduction](export/introduction.md)
4.  [Background and Motivation](export/background_and_motivation.md)
5.  [How to Read this Document](export/how_to_read_this_document/README.md)
    1.  [Scope & Audience](export/how_to_read_this_document/scope_&_audience.md)
    2.  [Conformance](export/how_to_read_this_document/conformance.md)
6.  [Semantic Web Technology, Linked Data, and RDF](export/semantic_web_technology,_linked_data,_and_rdf/README.md)
    1.  [RDF Data Structure](export/semantic_web_technology,_linked_data,_and_rdf/rdf_data_structure.md)
7.  [xAPI Vocabularies as Linked Datasets](export/xapi_vocabularies_as_linked_datasets.md)
8.  [Relationship Between Vocabularies, Profiles, and Recipes](export/relationship_between_vocabularies,_profiles,_and_r.md)
9.  [Vocabulary Dataset Schema](export/vocabulary_dataset_schema/README.md)
    1.  [Namespace](export/vocabulary_dataset_schema/namespace.md)
    2.  [Classes and Properties](export/vocabulary_dataset_schema/classes_and_properties.md)
    3.  [Recommended Classes](export/vocabulary_dataset_schema/recommended_classes.md)
    4.  [Optional Classes](export/vocabulary_dataset_schema/optional_classes.md)
    5.  [Recommended Properties](export/vocabulary_dataset_schema/recommended_properties.md)
    6.  [Optional Properties](export/vocabulary_dataset_schema/optional_properties.md)
10.  [Dataset Schema Design](export/dataset_schema_design/README.md)
    1.  [Alignment with SKOS](export/dataset_schema_design/alignment_with_skos.md)
    2.  [xAPI Verbs and Activity Types as Concepts](export/dataset_schema_design/alignment_with_skos.md#xapi-verbs-and-activity-types-as-concepts)
    3.  [xAPI Vocabularies as Concept Schemes](export/dataset_schema_design/alignment_with_skos.md#xapi-vocabularies-as-concept-schemes)
    4.  [Provenance Metadata](export/dataset_schema_design/provenance_metadata.md)
11.  [Vocabulary Development and Publishing](export/vocabulary_development_and_publishing/README.md)
    1.  [IRI Design and Persistence](export/vocabulary_development_and_publishing/iri_design_and_persistence.md)
    2.  [IRI Principles](export/vocabulary_development_and_publishing/iri_design_and_persistence.md#iri-principles)
    3.  [Recommended IRI Design Practices](export/vocabulary_development_and_publishing/iri_design_and_persistence.md#recommended-iri-design-practices)
    4.  [Generating and Maintaining Vocabulary IRIs](export/vocabulary_development_and_publishing/generating_and_maintaining_vocabulary_iris.md)
    5.  [Resolving IRIs and Content Negotiation](export/vocabulary_development_and_publishing/resolving_iris_and_content_negotiation.md)
    6.  [Publishing Vocabulary Datasets as HTML/RDFa](export/vocabulary_development_and_publishing/publishing_vocabulary_datasets_as_htmlrdfa.md)
    7.  [Publishing Vocabulary Datasets as JSON-LD](export/vocabulary_development_and_publishing/publishing_vocabulary_datasets_as_json-ld.md)
12.  [Vocabulary Search and Reuse](export/vocabulary_search_and_reuse.md)
    1.  [SPARQL](export/vocabulary_search_and_reuse.md#sparql)
    2.  Federated Search

13.  [Vocabulary Implementation Requirements](export/vocabulary_implementation_requirements.md)
14.  [References](export/references.md)
15.  [Additional Resources](export/additional_resources.md)
16.  [Acknowledgements](export/acknowledgements.md)
17.  [Appendices](export/appendices/README.md)
    1.  [Appendix A: HTML/RDFa Vocabulary Dataset Example](export/appendices/appendix_a_htmlrdfa_vocabulary_dataset_example.md)
    2.  [Appendix B: Content Negotiation .HTACCESS (Apache) Example](export/appendices/appendix_b_content_negotiation_htaccess_apache_exa.md)