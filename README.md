<p align="center">
  <a href="https://www.higginsd.com"><img src="assets/hero.svg" width="100%" alt="Higgins Digital: websites that push businesses forward. Animated cover with the Higgins Digital logo on a black starfield beside circuit traces carrying blue and gold pulses and crossing blue and gold marquee bands of services." /></a>
</p>

<h1 align="center">Higgins Digital</h1>

<p align="center"><strong>The website for Higgins Digital, my software development company: studio, work, services, and a direct path to start a project.</strong></p>

<p align="center">
  <a href="https://www.higginsd.com"><img src="assets/btn-open.svg" height="44" alt="Visit higginsd.com" /></a>&nbsp;
  <a href="https://www.higginsd.com/work"><img src="assets/btn-work.svg" height="44" alt="Work" /></a>&nbsp;
  <a href="https://www.higginsd.com/services"><img src="assets/btn-services.svg" height="44" alt="Services" /></a>&nbsp;
  <a href="https://davishiggins.com"><img src="assets/btn-dh.svg" height="44" alt="Davis Higgins" /></a>
</p>

<p align="center"><sub>Live · Founded, designed, and built by Davis Higgins · Charlotte, NC</sub></p>

---

## See it in motion

<p align="center">
  <img src="assets/demo.gif" width="800" alt="Screen recording of higginsd.com: opening the full-screen menu, hovering rows that turn into blue marquee bands, choosing Work, and scrolling the project grid." />
</p>

<p align="center"><sub>Real capture of the live site: menu, Work route transition, and project grid. <a href="assets/demo.png">Static frame</a></sub></p>

## What it does

- **Shows the work first.** A full-bleed project grid leads to a case study for every build, covering the problem, the direction, what was built, and the specifics.
- **Explains what the company does.** Services, pricing, and a growth offering each get a focused page, plus location pages for the Charlotte market.
- **Makes starting a project easy.** Contact paths, email, and social links are reachable from the menu and the footer on every page.

## Why I built it

Higgins Digital builds websites, platforms, and AI-powered systems for businesses. A company that sells high-end web work has to prove it on its own site first, so this one is held to the same bar as client builds: deliberate typography, motion with a purpose, and accessibility that survives the animation.

It's also the public record of my work, with every case study told one consistent way across the site.

## What I built

I founded Higgins Digital and designed and built its site:

- Information architecture across home, work, case studies, services, pricing, about, contact, blog, and location pages
- A single content source that powers the work grid, every case study, and related links
- Motion: route transitions, a full-screen menu with marquee hover bands, and scroll scenes, all with reduced-motion paths
- Search foundations: sitemap, structured data, per-page metadata, and a blog
- A private client area

<details>
<summary><strong>How it's put together</strong></summary>

<br />

```mermaid
flowchart TB
    C[One content source<br/>work · services · pricing] --> P[Site pages]
    A[Articles] --> P
    P --> S[Search-ready routes]
    P --> M[Motion layer]
    S --> V[Live site]
    M --> V
```

| Decision | Why |
|---|---|
| **One source of truth for the work** | Every project is described once and appears consistently everywhere it's referenced, so case studies can't drift out of sync. |
| **Motion that cleans up after itself** | Animations are scoped to the page they belong to, so moving around the site never leaves anything stuck or sluggish, and every scene has a reduced-motion version. |
| **Accessible under the effects** | Interactive elements are real links and buttons, the menu works fully from the keyboard, and brand colors were tuned until controls met contrast standards. |

</details>

## Screens

<table>
  <tr>
    <td width="62%"><img src="assets/screenshot-home.png" alt="Higgins Digital homepage: 'Websites that push businesses forward' over a black starfield with Work and About buttons." /></td>
    <td rowspan="2" width="38%" align="center"><img src="assets/screenshot-mobile.png" width="300" alt="Higgins Digital homepage on a phone." /></td>
  </tr>
  <tr>
    <td><img src="assets/screenshot-services.png" alt="Higgins Digital services page: 'Websites, platforms, and systems built around your business' with a list of services." /></td>
  </tr>
</table>

<sub>Homepage · Services · Homepage on mobile</sub>

## Technology

| Layer | Technology |
|---|---|
| Framework | Next.js, React, TypeScript, Tailwind CSS |
| Motion | GSAP, Lenis, Three.js |
| Hosting | Vercel |

---

<p align="center">
  <a href="https://www.higginsd.com"><img src="assets/btn-open.svg" height="44" alt="Visit higginsd.com" /></a>&nbsp;
  <a href="https://github.com/DavisHiggins"><img src="assets/btn-more.svg" height="44" alt="More of my work" /></a>
</p>

<p align="center"><sub>© 2026 Davis Higgins. All rights reserved. The Higgins Digital name and logo belong to Davis Higgins. Project imagery belongs to the respective projects and clients.</sub></p>
