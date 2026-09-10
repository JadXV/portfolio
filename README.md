<div align="center">

<img src="./icon.png" alt="JadXV" width="110" />

# JadXV | Portfolio

My interactive, terminal-style personal portfolio, built as a single HTML file.

[![Live at jadxv.com](https://img.shields.io/badge/Live-jadxv.com-5b93ff?style=for-the-badge&logo=vercel&logoColor=white)](https://jadxv.com)
&nbsp;
[![HTML5](https://img.shields.io/badge/HTML5-e34f26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS-1572b6?style=for-the-badge&logo=css&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)
&nbsp;
[![Vercel](https://img.shields.io/badge/Deployed_on_Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

</div>

---

## Overview

I'm Jad (JadXV), a full-stack developer from Toronto. This is my portfolio.

Instead of a normal scrolling page, it opens as a draggable, resizable macOS-style
terminal window. You explore it by typing commands like `whoami`, `skills`, and
`achievements`, while live widgets in the sidebar show my local time, my recent
GitHub activity, and my socials.

The whole thing lives in one file, [index.html](./index.html), with no build step
and no framework.

## Features

### Terminal experience
- Type-to-navigate command interface with a realistic zsh prompt
- Animated boot sequence with a per-character fade-in reveal (respects `prefers-reduced-motion`)
- Command history with the up and down arrow keys
- Tab completion with longest-common-prefix matching and suggestion listing
- Fuzzy "did you mean" hints powered by Levenshtein distance
- `clear` / `cls` to reset the screen

### macOS-style window
- Working traffic-light buttons for close, minimize, and maximize
- Drag the title bar to move the window, double-click to recenter
- Eight resize handles on the edges and corners
- Zoom with Cmd or Ctrl plus the `+`, `-`, and `0` keys, or Ctrl and scroll
- The window stays clamped inside the viewport

### Live sidebar widgets
- Dual analog clocks comparing my Toronto time with your local time, including the hour offset
- A GitHub widget that pulls my repo counts, follower counts, and recent public activity from the GitHub REST API, with local caching and rate-limit handling
- A "last update" line sourced from my latest commit to this repo
- A socials card linking my GitHub, Devpost, Discord, Twitter / X, and YouTube

### Built for discovery
- Full Open Graph and Twitter Card metadata
- Three JSON-LD blocks (Person, WebSite, ProfilePage)
- Screen-reader-only semantic content mirroring every terminal command
- Responsive layout with a dedicated mobile notice

## Terminal commands

| Command | What it shows |
| :--- | :--- |
| `help` | Every available command |
| `whoami` | A short intro |
| `skills` | The languages and tools I work in |
| `avgeek` | My aviation and flight-sim interests |
| `achievements` | My hackathon wins, participation, and hosting |
| `projects` | What I'm currently building |
| `github` | A link to my GitHub profile |
| `socials` | My social media and contact info |
| `clear` or `cls` | Clears the terminal screen |

## Tech stack

| Layer | Choice |
| :--- | :--- |
| Markup and styling | Handwritten HTML and CSS, no preprocessor |
| Behavior | Vanilla JavaScript, no framework or bundler |
| Data | [GitHub REST API](https://docs.github.com/en/rest) for activity and commit info |
| Hosting | [Vercel](https://vercel.com/), served at [jadxv.com](https://jadxv.com) |

## Running it locally

There's no build tooling. Clone the repo and open the file, or serve it with any
static server for the full API behavior.

```bash
git clone https://github.com/JadXV/portfolio.git
cd portfolio

# option 1: open it directly
open index.html

# option 2: serve it (recommended, avoids file:// quirks)
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Project structure

```text
portfolio/
├── index.html        all markup, styles, and scripts
├── background.jpeg    full-bleed blurred backdrop
├── icon.png           favicon, avatar, and window icon
└── .gitignore
```

## License

Please provide credit if you reuse any part of this project. All rights reserved.

---

<div align="center">

Made by Jad (JadXV)
&nbsp;·&nbsp;
[GitHub](https://github.com/JadXV)
&nbsp;·&nbsp;
[Devpost](https://devpost.com/JadXV)
&nbsp;·&nbsp;
[Twitter / X](https://x.com/JadXvX)
&nbsp;·&nbsp;
[YouTube](https://youtube.com/@jadxvx)

</div>
