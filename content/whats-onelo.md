---
id: whats-onelo
---

# What's Onelo

Onelo is a __set of tools__ that given a __data source__, __find files__ and __inspect their content__ to __extract structures__ that can be __exported__ and later __displayed__.

## Data sources

In the early stages of development, we understand data sources as some directory on the local file system.

> Future versions could be able to use remote data sources like Dropbox, Github repositories, etc accessed via API

## Find files

Search all files in the data source including subdirectories.

> Should Onelo find all files or only files that it can be able to inspect?

## Inspect content

Read the content of a given file and store it. //TODO: _content_ and _store it_ needs an explanation

> Should Onelo inspect all kind of files or only files that it can understand?

## Extract structures

From all the files found and inspected, three types of structures can be extracted:

1. Explicit: The same file hierarchy we can find in the data source filesystem.
2. Implicit: The structure is created based on:
    * links between files written along content
    * some metadata specified at the beginning of the file and understandable by Onelo //TODO: _Metadata_ needs an explanation
3. Inferred: The structure is created based on some machine learning or natural language processing algorithms

Explicit structure is obvious, and it not have much added value, but could be useful in some scenarios.

Implicit and inferred are the most valuable structures. They represent the relationships between the files through their content.

## Export structures

Structures could be represented in several ways that fit the needs of each structure, for example, an implicit structure could be represented as a graph or an inferred structure could be represented as some non-linear stuff.

At the end those representation should be exported as some set of data that can be consumed or persisted as a file using the best approach, for example, use [mermaid](https://mermaid-js.github.io) or [dot](https://en.wikipedia.org/wiki/DOT_(graph_description_language)), etc.

## Display structures and content

An structure exported (as stream of data or as a file) could be displayed using the more useful representation depending on the nature of the structure (some kind of graph, a classic hierarchy, etc). Moreover, it can be navigated and should display the content inspected.

User could swap between the differents structures extracted (if there are more than one).

## Tools

We have saved the tools for last. Tools are the things we need to accomplish the things explained in the previous sections.
