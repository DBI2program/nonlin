# NONLIN website

Starter website for the ERC project **NONLIN — Large-scale interactions mediating cognitive processes: Non-linear and nonseparable**.

## GitHub Pages

This site uses Jekyll and is designed to be hosted with GitHub Pages.

### Update a publication
Create a new Markdown file in `_publications/`, for example:

```yaml
---
title: "Paper title"
authors: "Author A., Author B."
journal: "Journal Name"
date: 2027-03-12
doi: "10.xxxx/xxxxx"
---
```

The publications page and homepage will update automatically.

### Add news
Create a Markdown file in `_news/`:

```yaml
---
title: "News headline"
date: 2027-03-12
category: Publication
---
Write the news text here in Markdown.
```

### Update team members
Edit or add Markdown files in `_people/`. The `order` field controls display order.

### Update collaborators
Edit or add files in `_collaborators/`.

## Local preview
With Ruby and Bundler installed:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.
