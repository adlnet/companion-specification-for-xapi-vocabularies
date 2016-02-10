## Namespace {#namespace}

The term “namespace” is used here to imply the IRI where the elements in a named ontology or schema are defined and resolved. The namespace IRI reserved for xAPI is ***```https://w3id.org/xapi/ontology#```***. This reserved namespace IRI initially addresses xAPI vocabularies, but may be further expanded in the future to define a more complete ontological data model representation of other xAPI objects and properties as well.

Both namespaces and prefixes are practices carried over from XML schema design principles. Namespace prefixes provide a shorthand way of abbreviating long namespace IRIs, making the classes and properties that belong to a schema or ontology more readable and compact. For example, Verb defined as a Class in the xAPI Vocabulary Dataset Schema is identified by the IRI, ***```https://w3id.org/xapi/ontology#Verb```*** and may also be represented as **xapi:Verb**, if the prefix **xapi** has been declared to stand for the namespace (***```https://w3id.org/xapi/ontology#```***)".

The namespace prefixes and their corresponding namespace IRIs currently used in this version of the xAPI Vocabulary Dataset Schema are provided below.

| **Schema/Ontology Name** | **Prefix** | **Namespace IRI** | **Purpose for xAPI Vocabularies** |
| --- | --- | --- | --- |
| Dublin Core | dcterms | http://purl.org/dc/terms/ | for time/date versioning |
| Friend Of A Friend (FOAF) | foaf | http://xmlns.com/foaf/0.1/ | for identifying the names of people or groups |
| Web Ontology Language (OWL) | owl | http://www.w3.org/2002/07/owl# | for ontology structure & modeling |
| Provenance Ontology (PROV-O) | prov | http://www.w3.org/ns/prov# | for vocabulary and term versioning and other maintenance metadata |
| Resource Description Framework (RDF) | rdf | http://www.w3.org/1999/02/22-rdf-syntax-ns# | for describing resources and their data types |
| RDF Schema | rdfs | http://www.w3.org/2000/01/rdf-schema# | for modeling resources with OWL classes & properties |
| Simple Knowledge Organization System (SKOS) | skos | http://www.w3.org/2004/02/skos/core# | for expressing relationships between concepts (e.g., verbs) and concept schemes (vocabularies) |
| Wordnet | wordnet | http://wordnet-rdf.princeton.edu/ontology# | for linking to synsets that can aid in word sense disambiguation and multilingual translations |
| Experience API (xAPI) | xapi | https://w3id.org/xapi/ontology# | to define xapi-specific classes and properties |
| XML Schema | xsd | http://www.w3.org/2001/XMLSchema# | for when using xsd data types such as date strings and language values |

Figure 4\. Table of select namespaces used for xAPI Vocabulary datasets.