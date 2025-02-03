# MINIMAL HUGO SITE

A 'bare bones' instructional site using <a href="https://github.com/gohugoio/hugo">Hugo</a> and <a href="https://github.com/picocss/pico">PicoCSS</a> styling.

# PROJECT CONTENTS
```
hugo.toml

layouts/_default/baseof.html # wraps every request with site-wide html
layouts/_default/single.html # lays out content/* != _index.md
layouts/index.html # lays out the homepage

archetypes/default.md # template for all content files
content/_index.md
```

# INSTALLATION

Clone the site locally
```
git clone --depth 1 https://github.com/rianrizvi/kickstart.git 
cd kickstart
```

[Install Hugo](https://gohugo.io/installation/) then check version (I'm on `v0.143.0`)
```
hugo version 
```

# QUICKSTART

Launch the site in your browser
```
hugo server --openBrowser
```


# NEXT

- Update `hugo.toml`, by setting the site wide html 'title', and baseURL used to rewrite absolute URLs

- Add content sections to the Homepage, while the Hugo server is running if you want
```
kickstart> hugo new content new-section.md
```
It creates a new `content/new-section.md` file with default content based on `archetypes/default.md`.
The new section will live update in the browser, and the Navbar menu will update with it. Edit the markdown under the leading variables section, you can include inline html, because the site configuration in `hugo.toml` allows it with the `markup.goldmark.renderer.unsafe` setting

- Change the `favicon.ico` in `layouts/_default/baseof.html` to use local image files, for example
```
<link rel="shortcut icon" type="image/png" href="/img/icon-192x192.png">
<link rel="shortcut icon" sizes="192x192" href="/img/icon-192x192.png">
<link rel="apple-touch-icon" href="/img/icon-192x192.png">
```
Then source and place these files by creating a `static/img` folder.
Don't forget incognito mode in your browser if you think you have caching/update issues.

- Extra instructions to build out the site are on the Homepage

