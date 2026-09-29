---
title: "Static Site Generator"
summary: "Markdown-to-HTML static site generator written from scratch in Python, with its own block and inline parser."
tags: ["Python", "Parsing", "Testing"]
repo: "https://github.com/cm-brown/static_site_generator"
demo: "https://cm-brown.github.io/static_site_generator/"
weight: 3
---
A static site generator built without any Markdown libraries. It parses Markdown into blocks and inline nodes, converts them into an HTML node tree, and renders every page in `content/` through a template, with unit tests along the way.

It's the same idea as Hugo, which runs this site. Building one myself is how I learned what a tool like that does.
