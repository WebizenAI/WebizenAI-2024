# Parsers

There are several parsers that are sought to be produced, to create RDF data and support for use by ML / LLM related tools, alongside other functionality.  This in-turn also relates to the library functionality.

## WebMarks: Semantic Bookmarks

The parser processes a WebPage and stores the information about it in RDF.


## Other Content Types

There's a list, and this is an initial, non-exhaustive high-level outline / placeholder.

### PDFs (& text)

The Parser should process the PDF file, then both store the content (text in particular) in a HTML related format, that incorporates also a comprehensive graph, incorporating entity analysis and other context information; as to make the file more easily consumable by LLM software and discoverable via Webizen Systems. 

By extension, the process should also be able to process images and decern content types in documents, as to distinguish tables, code and other content types to text. 

### Image Processing

The Image Processing system should produce metadata (in RDF) about the contents of the image and any discernible entities represented in the image.  The method should also support the ability for users to manually define 'assertions', that are then stored seperately in the file to other intepretations that may be generated via LLMs, etc.

There are various other functions, that'll be illustrated in documentation at some stage in the future.

### Audio Processing

Phonetic analysis, transcriptions and entity analysis; alongside the many other opportunities.


### Video Processing

Similar to Audio, but different. 

### Logs

The ability to process logs and other inputs that require schemas and processes.

