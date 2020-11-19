+++
id: onelo-core
+++

# Onelo Core

## Phases

TODO: Add here some link between following phases and What's Onelo

    Prelude: Set up contextual information such as the version of Onelo.
    Sourcing: Gather all relevant information given a source (e.g. a directory).
    Extraction: Parse all source entries, extract and generate the directed graph.
    Transformation: Apply tranformation rules to generate the desired output.

## Cache

TODO: Put here the content from docs/architecture/readme.md


TODO: Use this features to improve this documentation

* Read a directory recursively (all subdirectories included) and get the filename of all files inside
* Read a file and get all the contents
* Store file content in the cache
* Get file content from cache
* Get all files from cache according to its location in the filesystem
* Get a graph according to the relationships between them:
  * Links in their content
  * Connections created in their metadata
  * Inferred by its content
* Create and write files according content stored in the cache