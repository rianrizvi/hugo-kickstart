---
title: 'index'
weight: 10
redborders: false
---
A 'bare bones' instructional site using <a href="https://github.com/gohugoio/hugo">Hugo</a> and <a href="https://github.com/picocss/pico">PicoCSS</a> styling.

The benefit of Hugo is that it allows a solopreneur to reduce the overhead of managing a content
platform. You want to manage your site simply by editing mediawiki content files in Neovim or whatever. But you also need to keep doing styling/layout modifications so you cannot afford for that to become more complicated/cumbersome. Hugo breaks up the work of layout/styling in a way that makes sense for
the structure of your content. 

As your site/business expands, you want to add features, like site-wide color changes, UI libraries, back-end integration to perhaps Cloudflare Workers. This project will show that in stages, using different commits.

These initial paragraphs live in 
<kbd>content/_index.md</kbd>. Layout is determined by <kbd>layouts/index.html</kbd>.

Add variables at the top of the <kbd>content/_index.md</kbd> file, to parameterize how the front page is layed out. For example, I've added a 'redborders' variable to visually debug the homepage when necessary. This variable is used by <kbd>layouts/index.html</kbd>.
