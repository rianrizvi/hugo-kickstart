---
title: "New Sections"
slug: "new-sections"
type: "section"
date: 2025-02-02T14:29:25-08:00
weight: 20
---
You add a section to this homepage with <kbd>$ hugo new content &lt;filename&gt;</kbd> and edit the new <kbd>content/filename.md</kbd> file to set order (i.e. 'weight'), content etc.

When you add content files, the Hugo server live updates in your browser, unlike with updates to <kbd>layouts/*.html</kbd> files which require a manual browser refresh.

Workflow-wise you might block out a bunch of sections for a new site for some project, and then hop into the <kbd>.md</kbd> files and style them each with unique local html, as shown here. 

The navbar will automatically update, because the homepage layout reads the content files and builds out the options based on it. Most Hugo themes need you to manage a separate list of navbar items in <kbd>hugo.toml</kbd> which adds to code coupling.

