<div align="center">

# 🍒 Sharif Ruzaimi — Portfolio & Blog

A single-page personal portfolio and blog built from scratch with vanilla HTML, CSS and React (via Babel Standalone — no build step). Made for **CSD 34203 — Special Topics in Software Development, CLO3**.

[![Made with HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Made with CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-fc563c?style=for-the-badge)](#-license)

[**🌐 Live demo**](https://carlossain55.github.io/portfolio/) · [**🐙 Source**](https://github.com/CarlosSain55/portfolio) · [**👤 Author**](https://github.com/CarlosSain55)

</div>

---

## 📖 About this project

This is my personal portfolio and developer blog — built as the individual assignment for **CSD 34203** at UniSZA (CLO3, 20%). The brief was simple: build a personal blog page, push it to GitHub, demonstrate the full software-development workflow. I took the chance to go further and shipped a full editorial portfolio with a 3D CSS keycap skill board, a slideshow About section, an experience timeline, a 3-post blog with a modal reader, persistent dark-mode, and a clean handwritten design system in cream / navy / vermillion.

No build step. No npm. Open `index.html` and it runs.

---

## ✨ Features

| Section | What it does |
| --- | --- |
| **Home** | Editorial hero — giant `SR` monogram, vermillion disc, animated cutout portrait, scrambling subhead, parallax orbs, LIVE/SANDAKAN chip |
| **About** | Bio + auto-advancing 4-photo slideshow (hover to pause, prev/next, frame counter) + animated stats grid |
| **Experience** | 3-card timeline — Matcha Cloud · UniSZA · Multimedia Exco — with hover-tilt photo cards |
| **Skills** | **Real 3D CSS keycap board** of 25 caps. Hover lifts a cap, click presses it, and the actual physical key on your keyboard presses the matching cap. Real brand logos via the Simple Icons CDN |
| **Projects** | Animated reveal of the four featured projects from my CV |
| **Notes (Blog)** | 4 sample posts in a card grid + full-screen modal reader (`Esc` to close) |
| **Contact** | Big editorial layout, social cards with logos, click-to-copy email, available-status pill |
| **Dark mode** | Floating toggle bottom-right, persisted to `localStorage` |
| **Navigation** | Floating center pill with scroll-spy + sliding active indicator + top progress bar |
| **Responsive** | Grids collapse at 920px and 620px, nav labels hide on small screens |

---

## 🧰 Tech stack

- **Markup** — semantic HTML5
- **Styling** — hand-written CSS, custom properties (theming), CSS Grid + Flex, 3D transforms, masks
- **Behaviour** — React 18 + JSX, transpiled in-browser by Babel Standalone (zero toolchain)
- **Typography** — Space Grotesk · JetBrains Mono · Instrument Serif (Google Fonts)
- **Icons** — Simple Icons (CDN, CC0)
- **Persistence** — `localStorage` for theme
- **Workflow** — Git + GitHub

---

## 📁 Project structure

```
portfolio/
├── index.html              # entry — fonts, CSS variables, boot splash, script tags
├── app.jsx                 # <App>, <ThemeToggle>, section orchestration
├── sections.jsx            # Nav · Hero · About · Experience · Projects · Contact · Marquee
├── keyboard.jsx            # 3D keycap board · brand-logo loader · skills data
├── blog.jsx                # Blog grid · post cards · modal reader · cover art
├── README.md               # this file
└── assets/
    ├── sharif-cutout.png       # transparent hero portrait
    ├── sharif-polaroid.jpg     # polaroid for About slideshow
    ├── sharif-diner.jpg
    ├── sharif-garden.jpg
    ├── matcha-cloud.jpg        # Experience card
    ├── exp-unisza.jpg          # Experience card — Anugerah Cemerlang
    └── exp-exco.jpg            # Experience card — Pertahanan Awam
```

---

## 📰 Sample posts

The Notes section ships with four field-note style posts:

1. **TutorGo: matching students with tutors** — building a role-based booking platform in CodeIgniter 4.
2. **Teaching a model to see thread** — what I learned building a YOLO defect detector for fabric.
3. **A thousand sales rows and a star** — designing a warehouse that survives its first OLAP query.
4. **Notes from behind a matcha bar** — why I think pulling shots makes me a better engineer.

Each post has a custom inline-SVG cover, an author byline, a tag list, and renders inside a click-to-open reader modal.

---

## ▶️ Running it locally

### Option A — open the file directly

```bash
git clone https://github.com/CarlosSain55/portfolio.git
cd portfolio
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

### Option B — serve it (recommended)

A static server avoids any quirks with CDN scripts. Pick whichever you have:

```bash
python3 -m http.server 5173
# → http://localhost:5173

# or
npx serve .
```

No dependencies to install, no build step to run.

---

## 🚀 Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Repository → **Settings → Pages**.
3. **Source:** Deploy from a branch · **Branch:** `main` · **Folder:** `/ (root)`.
4. Save. After a minute the site is live at
   `https://<your-username>.github.io/portfolio/`.

---

## 🖼️ Screenshots

> _Drop screenshots into a `/screenshots` folder, then link them here:_
>
> | Home | Skills | Blog reader |
> | --- | --- | --- |
> | ![](screenshots/01-home.png) | ![](screenshots/02-skills.png) | ![](screenshots/03-blog.png) |

---

## 🗒️ Commit history (highlights)

Following the rubric's "at least 3 meaningful commits" requirement, the actual history has many more — these are the highlights:

- `init: scaffold index.html, fonts, boot splash`
- `feat(hero): editorial composition with SR monogram + cutout portrait`
- `feat(skills): 3D CSS keycap board with brand logos`
- `feat(experience): timeline cards with large photo thumbnails`
- `feat(blog): card grid, modal reader, four sample posts`
- `feat(theme): persistent dark-mode toggle`
- `feat(contact): social cards with brand logos`
- `style(palette): editorial cream / navy / vermillion`
- `docs: write README with features, tech, run steps`

---

## 👤 Author

<table>
<tr>
<td valign="top" width="120">
  <img src="assets/sharif-cutout.png" alt="Sharif Ruzaimi" width="100" />
</td>
<td valign="top">

**Sharif Ruzaimi Syirazi**
BSc Computer Science (Software Development) · Universiti Sultan Zainal Abidin

📍 Sandakan, Sabah, Malaysia
✉️ [shruzaimi@gmail.com](mailto:shruzaimi@gmail.com)
🐙 [github.com/CarlosSain55](https://github.com/CarlosSain55)
💼 [linkedin.com/in/sharif-ruzaimi-syirazi](https://www.linkedin.com/in/sharif-ruzaimi-syirazi)
📱 +60 17-811 7668

</td>
</tr>
</table>

---

## 📄 License

The **code** in this repository is released under the [MIT License](https://opensource.org/licenses/MIT) — feel free to read, fork, and learn from it.

Personal **photos** and **written content** (blog posts, biography) remain © Sharif Ruzaimi Syirazi 2026 and are not licensed for reuse.

---

<div align="center">

_Built with HTML, CSS, a bit of React, and a lot of matcha._<br />
_CSD 34203 — Special Topics in Software Development · CLO3 · 20%_

⭐️ **If you like it, leave a star — it makes my day.**

</div>
