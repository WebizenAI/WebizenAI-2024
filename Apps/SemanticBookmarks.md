# Semantic Bookmarks

This notion of a 'semantic bookmark' is about the construction of an RDF file that contains a volume of structured data about a URL.  

If this name needs to be changed, that's fine.  A possible name is WebMarks, but, not much thought has gone into it yet.

## Description

When a Semantic Bookmark is created, it acquires the available structured data from the site location and compiles it into an RDF based record.  This may be used with LLM technology to add additional information, such as categorisation, that may be absent from that page.  The design structure should also support the means to define a location where a temporal snapshot of the webpage may be stored for preservation, whether via an archive services such as archive.org or via IPFS.  

The structure should also support the means to create logs about the access history, time spent and any changes associated to the bookmarked reference / page.  

Social Information and permissions interfaces are also expected to be appended to these records.

## Key Ontologies

The Key ontologies expected to be most prevelant are;

- SchemaOrg: due to its use for SEO
- OGP: due to its use for Social Media Sites.

Other ontologies that are expected to be used; include but are not limited to,

- DublinCore
- WikiData
- FOAF
- SOIC
- PROV
- RDFS
- OWL

## Creation Tools

Semantic Social-Web tooling, integrated into browsers, is expected to be used to create Semantic Bookmarks, that are then stored in the users systems.  

## Retrival Tools

The primary storage method is intended be a database that provides a SPARQL interface.

