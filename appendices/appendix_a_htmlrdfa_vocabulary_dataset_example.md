## Appendix A: HTML/RDFa Vocabulary Dataset Example {#appendix-a-html-rdfa-vocabulary-dataset-example}

**Vocabulary Dataset as RDFa. _This example is not complete and is provided for documentation purposes only._**
**_The cmi5 verbs are actually part of the ADL vocabulary dataset._**

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<title>Experience API (xAPI) - cmi5 Vocabulary Dataset</title>
</head>
<body>
<div xmlns="http://www.w3.org/1999/xhtml" prefix="
    dcterms: http://purl.org/dc/terms/
    foaf: http://xmlns.com/foaf/0.1/
    owl: http://www.w3.org/2002/07/owl#
    prov: http://www.w3.org/ns/prov#
    rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
    rdfs: http://www.w3.org/2000/01/rdf-schema#
    skos: http://www.w3.org/2004/02/skos/core#
    xapi: https://w3id.org/xapi/ontology#
    xsd: http://www.w3.org/2001/XMLSchema#"> 
  
  <!-- Vocabulary -->
  <div typeof="skos:ConceptScheme" about="https://w3id.org/xapi/cmi5">
    <div property="skos:prefLabel" lang="en" xml:lang="en" content="cmi5 Vocabulary">
      <h2 class="page-header">cmi5 Vocabulary</h2>
    </div>
  </div>

  <table class="table table-hover">
    <thead>
      <tr class="info">
        <th>Label</th>
        <th>Description</th>
        <th>Closely Related Term</th>
        <th>Vocabulary</th>
      </tr>
    </thead>

    <!-- Newly Minted Verb -->
    <tbody typeof="xapi:Verb" about="https://w3id.org/xapi/adl/verbs/abandoned" id="abandoned">
      <tr>
        <td property="skos:prefLabel" lang="en" xml:lang="en" content="abandoned">abandoned</td>
        <td property="skos:definition" lang="en" xml:lang="en" content="Indicates the activity provider has determined that the session was abnormally terminated either by an actor or due to a system failure.">Indicates the activity provider has determined that the session was abnormally terminated either by an actor or due to a system failure.</td>
        <td rel="xapi:closelyRelatedNaturalLanguageTerm" resource="http://wordnet-rdf.princeton.edu/wn31/202080923-v"><a href="http://wordnet-rdf.princeton.edu/wn31/202080923-v" target="_blank">http://wordnet-rdf.princeton.edu/wn31/202080923-v</a></td>
        <td rel="skos:inScheme" resource="https://w3id.org/xapi/cmi5"><a href="https://w3id.org/xapi/cmi5">https://w3id.org/xapi/cmi5</a></td>
      </tr>
    </tbody>
    
    <!-- Newly Minted Verb -->
    <tbody typeof="xapi:Verb" about="https://w3id.org/xapi/adl/verbs/satisfied" id="satisfied">
      <tr>
        <td property="skos:prefLabel" lang="en" xml:lang="en" content="satisfied">satisfied</td>
        <td property="skos:definition" lang="en" xml:lang="en" content="Indicates that the authority or activity provider determined the actor has fulfilled the criteria of the object or activity.">Indicates that the authority or activity provider determined the actor has fulfilled the criteria of the object or activity.</td>
        <td rel="xapi:closelyRelatedNaturalLanguageTerm" resource="http://wordnet-rdf.princeton.edu/wn31/202677669-v"><a href="http://wordnet-rdf.princeton.edu/wn31/202677669-v" target="_blank">http://wordnet-rdf.princeton.edu/wn31/202677669-v</a></td>
        <td rel="skos:inScheme" resource="https://w3id.org/xapi/cmi5"><a href="https://w3id.org/xapi/cmi5">https://w3id.org/xapi/cmi5</a></td>
      </tr>
    </tbody>
    
    <!-- Newly Minted Verb -->
    <tbody typeof="xapi:Verb" about="https://w3id.org/xapi/adl/verbs/waived" id="waived">
      <tr>
        <td property="skos:prefLabel" lang="en" xml:lang="en" content="waived">waived</td>
        <td property="skos:definition" lang="en" xml:lang="en" content="Indicates that the learning activity requirements were met by means other than completing the activity. A waived statement is used to indicate that the activity may be skipped by the actor.">Indicates that the learning activity requirements were met by means other than completing the activity. A waived statement is used to indicate that the activity may be skipped by the actor.</td>
        <td rel="xapi:closelyRelatedNaturalLanguageTerm" resource="http://wordnet-rdf.princeton.edu/wn31/202539728-v"><a href="http://wordnet-rdf.princeton.edu/wn31/202539728-v" target="_blank">http://wordnet-rdf.princeton.edu/wn31/202539728-v</a></td>
        <td rel="skos:inScheme" resource="https://w3id.org/xapi/cmi5"><a href="https://w3id.org/xapi/cmi5">https://w3id.org/xapi/cmi5</a></td>
      </tr>
    </tbody>
  </table>
</div>
</body>
</html>```

Figure 10\. Example of vocabulary as RDFa/HTML (index.html hosted at ```http://example.com/datasets/cmi5```)