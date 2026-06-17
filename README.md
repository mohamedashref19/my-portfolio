<div align="center">

# Mohamed Ashraf — Developer Portfolio

<br>

![HTML5](https://img.shields.io/badge/HTML5-080b10?style=for-the-badge&logo=html5&logoColor=00e5a0)
![CSS3](https://img.shields.io/badge/CSS3-080b10?style=for-the-badge&logo=css3&logoColor=00e5a0)
![JavaScript](https://img.shields.io/badge/JavaScript-080b10?style=for-the-badge&logo=javascript&logoColor=00e5a0)
![Node.js](https://img.shields.io/badge/Node.js-080b10?style=for-the-badge&logo=node.js&logoColor=00e5a0)
![MongoDB](https://img.shields.io/badge/MongoDB-080b10?style=for-the-badge&logo=mongodb&logoColor=00e5a0)
![AWS](https://img.shields.io/badge/AWS_EC2-080b10?style=for-the-badge&logo=amazonec2&logoColor=00e5a0)

<br>

[![Live Site](https://img.shields.io/badge/→%20View%20Live%20Site-00e5a0?style=for-the-badge&labelColor=080b10&color=00e5a0&logoColor=080b10)](https://github.com/mohamedashref19)
[![Email](https://img.shields.io/badge/→%20Get%20In%20Touch-7c6bff?style=for-the-badge&labelColor=080b10&color=7c6bff)](mailto:mohamedashref2003195@gmail.com)

</div>

---

## 🧠 About The Project

This repository is the source code for my personal developer portfolio — the single page that answers the question _"what does this engineer actually build?"_

Most backend engineers are invisible on the web. The work is in the logic, the architecture, the things users never see but always feel. This portfolio flips that: it's designed to make backend thinking _visible_ — through a terminal-native aesthetic, structured data presentation, and a layout that mirrors how a developer actually thinks about systems.

Built with zero frameworks and zero dependencies. Just **HTML, CSS, and Vanilla JS** — because choosing the right tool for the job is itself a backend skill.

> The design uses a dual-accent system — `#00e5a0` mint for primary actions and `#7c6bff` violet for secondary effects — paired with `Space Grotesk` for display typography and `JetBrains Mono` for all code-adjacent UI elements.

---

## ✨ Key Features

- **`profile.json` Terminal Mockup** — The About section renders my profile as syntax-highlighted JSON with a blinking cursor, built entirely in CSS and semantic HTML. No canvas, no libraries.

- **CSS Glitch Effect** — A subtle typographic glitch on the hero section using `::before` / `::after` pseudo-elements with offset `clip-path` animations and staggered timing — no JavaScript involved.

- **Animated Mesh Gradient Hero** — Two radial gradient orbs (mint + violet) animate independently with `@keyframes`, creating a living depth effect without any canvas or WebGL overhead.

- **Perspective Grid Background** — SVG-based dot/line grid masked with a radial gradient, giving the hero a terminal-screen spatial feel.

- **Skill Ticker** — A seamless, infinitely looping horizontal marquee of the tech stack built with pure CSS `translate` animation — pausable on hover.

- **Scroll-triggered Entrance Animations** — `IntersectionObserver` drives `fade-up`, `fade-left`, and `fade-right` classes with staggered delays, keeping the page snappy with zero layout shift.

- **Active Nav Highlighting** — Scroll position is tracked and the correct nav link is highlighted dynamically without any router or third-party scroll library.

- **SVG Noise Grain Overlay** — A fixed, full-viewport `feTurbulence` SVG filter adds a subtle film-grain texture to the background, improving perceived depth on dark surfaces.

- **Fully Responsive** — CSS Grid and Flexbox with `clamp()` fluid type scaling. The layout restructures cleanly at `900px` and `600px` breakpoints with a hamburger nav drawer on mobile.

- **Accessible & Semantic** — `<article>`, `<header>`, `<nav>`, `<section>`, `<footer>` throughout. `aria-label`, `aria-expanded`, and `role` attributes on interactive elements. `prefers-reduced-motion` respected.

- **Custom Scrollbar** — 3px mint-colored scrollbar track via `::-webkit-scrollbar`, consistent with the accent palette.

---

## 🚀 Featured Work

The portfolio showcases four production-grade backend projects:

| Project                 | Description                                                                                                                                                                      | Stack                                |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| **Masar**               | AI freelancing platform (Graduation Project). An AI requirements builder converts rough client briefs into structured specs; Stripe escrow holds funds until milestone delivery. | Node.js · MongoDB · Stripe · AI      |
| **Aqra**                | Voice-recognition Quran companion, live on Google Play. Real-time recitation correction powered by voice AI, deployed on AWS EC2 with zero-downtime architecture.                | Node.js · Capacitor · Firebase · AWS |
| **Restaurant Platform** | End-to-end booking system with Stripe payments, admin dashboard, and dynamic transactional emails.                                                                               | Node.js · Express · MongoDB · Stripe |
| **Natours**             | Tour booking REST API with geospatial queries, JWT auth, role-based access control, and Stripe checkout.                                                                         | Node.js · MongoDB · Mapbox           |

---

## 🛠️ Local Setup

No build step. No package manager. No config files. Clone and open.

**1. Clone the repository**

```bash
git clone https://github.com/mohamedashref19/portfolio.git
```

**2. Navigate into the project**

```bash
cd portfolio
```

**3. Open in your browser**

```bash
# Option A — open directly (macOS / Linux)
open index.html

# Option B — open directly (Windows)
start index.html

# Option C — serve locally with Python (recommended, avoids CORS on any assets)
python3 -m http.server 8080
# then visit http://localhost:8080
```

> **Note:** If you have the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension in VS Code, right-click `index.html` → _Open with Live Server_ for hot-reload during development.

---

## 🎨 Design Tokens

For anyone forking or adapting this — the entire visual system lives in `:root` CSS variables at the top of `index.html`:

```css
:root {
  --bg: #080b10; /* page background       */
  --surface: #111620; /* card / panel surfaces  */
  --border: #1c2535; /* subtle dividers        */
  --mint: #00e5a0; /* primary accent         */
  --violet: #7c6bff; /* secondary accent       */
  --text: #dde4ef; /* primary text           */
  --text-2: #7e92a8; /* muted text             */
  --mono: "JetBrains Mono", monospace;
  --sans: "Space Grotesk", sans-serif;
}
```

Swap the two accent values to re-theme the entire site instantly.

---

## 📁 Project Structure

```
portfolio/
├── index.html        # Entire site — markup, styles, and scripts in one file
├── README.md         # You are here
└── images/           # Project thumbnails (optional, referenced in project cards)
    └── thumbs/
        ├── masar.jpg
        ├── aqra.jpg
        └── ...
```

> The site is intentionally a single-file build. For a portfolio of this scope, the maintenance overhead of a bundler outweighs the benefits.

---

## 📬 Contact

<div align="center">

I'm open to **backend freelance work**, **internship opportunities**, and **interesting problems**.

|                 |                                                                         |
| --------------- | ----------------------------------------------------------------------- |
| 📧 **Email**    | [mohamedashref2003195@gmail.com](mailto:mohamedashref2003195@gmail.com) |
| 🐙 **GitHub**   | [@mohamedashref19](https://github.com/mohamedashref19)                  |
| 📍 **Location** | Alexandria, Egypt                                                       |

<br>

_If you have a project that needs backend magic — reach out._

</div>

---

<div align="center">

<sub>Built with HTML · CSS · Vanilla JS &nbsp;·&nbsp; No frameworks were harmed in the making of this site.</sub>

<br>

<sub>© 2026 Mohamed Ashraf — Backend Engineer</sub>

</div>
