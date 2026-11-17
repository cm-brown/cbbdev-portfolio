---
title: "merry_xmas.exe"
summary: "Retro Christmas card in a single HTML file: a Windows 95-style window with low-poly dancing elves and a chiptune Jingle Bells."
tags: ["JavaScript", "Canvas", "3D", "Web Audio"]
demo: "https://merry.cbbdev.com"
category: "web"
weight: 7
---
A Christmas card that opens like an old desktop program. It's one HTML file with no libraries or build step.

**What's inside**

- A small 3D renderer I wrote on a 2D canvas: box and cone meshes, matrix transforms, perspective projection, flat shading, and painter's-algorithm sorting, drawn at low resolution so it stays pixelated.
- Elves built from those shapes, each running one of several dance moves. You can add up to 15 or cycle moves with the buttons, a click, or the `E` and `M` keys.
- A typewriter-style dialogue box with the card's message.
- Jingle Bells played as chiptune with the Web Audio API, using square-wave melody and bass tones scheduled ahead of time.
