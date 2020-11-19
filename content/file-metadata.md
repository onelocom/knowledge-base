# File metadata

Onelo uses metadata to extract some structure between files, we knows that structure as __implicit structure__.

Each type of file will have their own metadata. In the early stages of development, only markdown files are supported.

## Markdown

The metadata must be a [toml](https://toml.io) set of data added to the beginning (front matter) of a markdown file.
Insert metadata between `+++` (like [hugo](https://gohugo.io/content-management/front-matter/) do).

```
+++
Insert here metadata
+++
```

### Metadata specification

* id

### Example

```
+++
id: file-metadata
+++
