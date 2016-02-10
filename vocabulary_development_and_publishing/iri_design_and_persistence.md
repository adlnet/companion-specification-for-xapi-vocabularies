## IRI Design and Persistence {#iri-design-and-persistence}

The concept of IRI persistence for xAPI can be explained as the desirable outcome that any HTTP IRI used as an xAPI identifier should continue to constantly identify and stably refer that resource. Since xAPI is based on a web infrastructure that is dynamic and sometimes inherently unpredictable, the community requires a better continuity strategy for creating and maintaining identifiers based on stable IRIs. The rationale behind IRI persistence is simple: imagine that a developer or CoP is reusing the Verbs defined in an existing vocabulary, and the IRIs are no longer accessible. The person or CoP reusing the Verbs would no longer know the proper definitions or meaning, intended usage, date it was last updated, and other pertinent information.

A lack of an IRI design and persistence policy, coupled with a heavy dependency on an external vocabulary, has already resulted in many xAPI Verb and Activity Type IRIs that are not accessible. This was primarily the result of adopting IRIs for Verbs and Activity Types from the JSON Activity Streams 1.0 vocabulary. These IRIs were deprecated by that community and when accessed provide no semantic meaning to xAPI implementations. A persistence strategy and guidelines are critical for stable and predictable HTTP-based IRIs. The stability of IRIs not only depends on whether they are persistent, but how CoPs prepare, design, and manage them. The purpose of this part of the specification is to provide guidance for xAPI designers or developers responsible for creating identifiers. A list of recommended persistence and design practices are provided below.

### IRI Principles {#iri-principles}

This section provides a set of general design principles aimed at helping xAPI stakeholders make better decisions when creating and managing IRIs. Most of these principles were collected from IRI persistence research by the W3C’s Phil Archer (2013).

1.  IRIs should be stable and reliable in order to maximize the possibilities of reuse.
2.  IRIs should be well-formed by following a consistent pattern for naming constructs.
3.  IRIs should avoid using file extensions or technologies, and use careful naming conventions for the domain, any subdomains, and resources.
4.  IRIs should avoid using query strings (e.g., http://example.com/getId.aspx?id=1). 
5.  IRIs should be designed with governance and maintenance in mind.
6.  IRIs should use a dedicated and trusted service independent of the originator for provisioning and maintenance.
7.  IRIs should be designed and built to be able support multiple types of formats (both human and machine readable).

### Recommended IRI Design Practices {#recommended-iri-design-practices}

While keeping the aforementioned principles in mind, the following practices are recommended for designing all new xAPI IRIs:

1.  **Use a strong IRI pattern.** The following pattern for an IRI designed for persistence is based on research findings from Archer (2013). In the research findings and case studies examined, the most stable IRIs followed a consistent pattern for naming constructs. The recommended pattern below has been adapted specifically for the xAPI community.

https:// {**domain**} / {**resource** **type**} / {**vocabulary**} / {**term type**} / {**term**}

For example the cmi5 verb, **_https://w3id.org/xapi/adl/verbs/satisfied_ **follows this pattern where:

|  |
| --- |

*   **{domain}** is the host server where the resource .
*   **{resource type} **declares the core/base type of resource (i.e., xapi).
*   **{vocabulary}** specifies the vocabulary or profile that uses or maintains the vocabulary term(s) (i.e., adl).
*   **{term type}** is the type of vocabulary term (i.e., verbs).
*   **{term}** is the specific vocabulary term resource (i.e., satisfied).

1.  **Use a dedicated service when minting new xAPI IRIs.** According to Yakel (2007), curation has been deﬁned as “the active involvement of information professionals in the management, including the preservation, of digital data for future use.”  Services such as W3id.org allow for the curation of persistent HTTP IRIs on the web and provide a resolution service that allows the xAPI community to manage persistent IRI identifiers that can force a redirection to a target web resource. If the target IRI changes, the persistent IRI identifier pointing to it can be easily updated. Creating an IRI identifier that can be maintained openly by multiple members of a CoP is a recommended practice as it affords a minimal number of risks and dependencies. Alternatively, designers could mint new IRIs using their own domain on their own privately owned server, but that would inherently contradict many of the aforementioned best practices for persistence.