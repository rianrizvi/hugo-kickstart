---
title: "{{ replace .Name "-" " " | title }}"
slug: "{{ .Name }}"
type: "section"
date: {{ .Date }}
weight: 999
---
This is the <kbd>content/{{ .Name }}.md</kdb> file
