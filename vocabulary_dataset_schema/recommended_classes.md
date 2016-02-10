## Recommended Classes {#recommended-classes}

| **Class Name** | **Description** | **rdf:type** | **rdfs:subClassOf** | **owl:disjointWith** |
| --- | --- | --- | --- | --- |
| xapi: ActivityType | The Activity Type corresponds to the type identifier of the Activity Definition Object in an xAPI statement. When the IRI is dereferenced it can provide specific information (metadata) about the type of activity. Activity Types are concepts and should be associated with a specific activity vocabulary. | [owl:Class](http://www.w3.org/2002/07/owl#Class) | [skos:Concept](http://www.w3.org/2004/02/skos/core#Concept) | [xapi:Verb](https://w3id.org/xapi/ontology#Verb) |
| skos:ConceptScheme | A SKOS concept scheme is an aggregation of one or more SKOS concepts. xAPI vocabularies are represented as concept schemes. For example, a verb vocabulary is a concept scheme. | [owl:Class](http://www.w3.org/2002/07/owl#Class) |  | [skos:Concept](http://www.w3.org/2004/02/skos/core#Concept),[skos:Collection](http://www.w3.org/2004/02/skos/core#Collection) |
| xapi:Verb | Verbs correspond to the id / identifier of the Verb Object in an xAPI statement. When the IRI is dereferenced it can provide more meaning about the Verb term. Verbs are concepts and should be associated with a specific verb dataset and may be referenced by other vocabularies. | [owl:Class](http://www.w3.org/2002/07/owl#Class) | [skos:Concept](http://www.w3.org/2004/02/skos/core#Concept) |  |

Figure 5\. Table of recommended classes for xAPI Vocabulary datasets.