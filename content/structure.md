---
title: "Structure"
slug: "structure"
type: "section"
date: 2025-02-02T14:44:52-08:00
weight: 30
---

```
hugo.toml

layouts/_default/baseof.html # wraps every request with site-wide html
layouts/_default/single.html # lays out content/* != _index.md
layouts/index.html # lays out the homepage

archetypes/default.md # template for all content files
content/_index.md
```

**HUGO.TOML EXAMPLE**
```
baseURL = "https://kickstartplatforms.com/"
title = 'Kickstart'

[taxonomies] # empty so explicitly undefined
```
- baseURL replaces absolute links
- title is a parameter used in layout files
- taxonomies is helpful for bigger sites, not necessary right now

**CONTENT/ vs LAYOUTS/**

Each content file matches a web resource path, eg `https://website.com/` retrieves `content/index.md`. So that file must exist, and so must a matching layout file, `layouts/index.html`. 

The matching rules are explained in depth later, but here's another example: `https://website.com/<anything>.html` =&gt; `content/<anything>.md` =&gt; `layous/_default/single.html`

`_default/baseof.html` provides site wide html, and wraps every `layouts/` file retreived.


