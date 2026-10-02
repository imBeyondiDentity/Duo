# Trio

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A hub page for three small audio tools. It doesn't process anything
itself — just link cards pointing to three separate browser apps, tied
together by one entry point and one shared design.

Runs entirely client-side. Nothing gets uploaded anywhere — each of the
three tools is its own HTML/JS file, working everything out right in the
browser. Deploys to GitHub Pages as static files, no build step, no
dependencies.

## Tools

| Tool | What it does |
|---|---|
| [Peel](peel.html) | pulls the sound out of a video, saves it as MP3 or WAV |
| [Monologue](monologue.html) | turns singing into speech, same voice |
| [Cover](cover.html) | embeds cover art into MP3 or WAV |

Each one is a standalone file and can be opened and used on its own,
away from the hub; `index.html` just gives them a shared front door and
a language toggle (RU/EN, defaulting off `navigator.language` with a
manual override).

## Other projects

The hub also carries a row of short links out to tools that live
outside this repository — currently [Airband](https://imbeyondidentity.github.io/airband/)
(restores the top end cut from Suno tracks) and [Music DNA](https://imbeyondidentity.github.io/identity-prompt-engine/)
(the Suno prompt engine). They open in a new tab, so Trio doesn't get
lost in the background.


## Structure

```
index.html       the hub: heading, three cards, "other projects" row, RU/EN
peel.html        Peel in full, a standalone self-contained file
monologue.html   Monologue in full, a standalone self-contained file
cover.html       Cover in full, a standalone self-contained file
```

Each HTML file is self-contained — styles and logic are inlined, no
external links out to a `.css`/`.js` file. Opened on its own (through a
chat preview, say), any one of them works by itself; following a link
from one file to another only resolves once they're all sitting
together on real hosting.

## Licence

MIT — see [`LICENCE`](LICENSE). Use it, fork it, change it, commercial
use included. The only condition is keeping the copyright notice and
licence text in copies.
