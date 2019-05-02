# International HPC Summer School Wiki

This wiki is in support of the [International HPC Summer School](http://www.ihpcss.org), but is *not* the official location of event details.
Instead, this wiki hosts public resources mostly from the mentoring committee.

## Adding a Page

Creating a page is easy.
Either point your browser at "ihpcss.github.io/wiki/new-page-name" or create a new markdown (`.md`) file within the `wiki` directory.

On each page, please include the following yaml front-matter at the top:

``` yaml
---
layout: page
title: "New Page Name Here"
---
```

To have a page appear in the sidebar navigation, include this in the front-matter:

``` yaml
tag: [sidebar]
```

Once you've created the new page, manually update the site map listing on the `index.md` page.

## Editing

The sidebar on each page has links to "Edit this page" and "Edit with Prose.io".
These links will take you to GitHub and Prose.io respectively to edit the page.

## Styling

The title from the yaml front-matter is automatically converted to an H1 (`#`) heading.
All headings within a page should be H2 (`##`) or lower.
