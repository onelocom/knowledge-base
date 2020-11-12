---
id: onelo-api
---

# Onelo API

Rust

## Features

- Read a directory recursively (all subdirectories included) and get the filename of all files inside
- Read a file and get all the contents
- Store file content in the cache
- Get file content from cache
- Get all files from cache according to its location in the filesystem
- Get a graph according to the relationships between them:
    - Links in their content
    - Connections created in their metadata
    - Inferred by its content
- Create and write files according content stored in the cache