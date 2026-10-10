<p align="center">
  <a href="https://www.higginsd.com"><img src="assets/hero.gif" width="100%" alt="Higgins Digital — websites that push businesses forward. Decorative animated cover: the Higgins Digital H logo on black beside electric-blue circuit lines with occasional gold pulses." /></a>
</p>

<h1 align="center">Higgins Digital</h1>

<p align="center">
  <strong>The website for Higgins Digital, my software development company: studio, work, services, and a direct path to start a project.</strong><br />
  <a href="https://www.higginsd.com"><strong>Visit higginsd.com ↗</strong></a> · <a href="https://www.higginsd.com/work">Work</a> · <a href="https://www.higginsd.com/services">Services</a> · <a href="https://davishiggins.com">Davis Higgins</a>
</p>

<p align="center"><sub>Live · Founded, designed, and built by Davis Higgins · Charlotte, NC</sub></p>

---

## See it in motion

<p align="center">
  <img src="assets/demo.gif" width="800" alt="Screen recording of higginsd.com: opening the full-screen menu, hovering rows that turn into blue marquee bands, choosing Work, and scrolling the project grid." />
</p>

<p align="center"><sub>Real capture of the live site: menu, Work route transition, and project grid. <a href="assets/demo.png">Static frame</a></sub></p>

## What it does

- **Shows the work first.** A full-bleed project grid leads to a case study for each build. Every study covers the problem, the direction, what was built, and checkable specifics, with client and in-house work labeled honestly.
- **Explains what the company does.** Services, pricing, and a growth offering each get a focused page, plus location pages for the Charlotte market.
- **Makes starting a project easy.** Contact paths, email, and social links are reachable from the menu and the footer on every page.

## Why I built it

Higgins Digital builds websites, platforms, and AI-powered systems for businesses. A company that sells high-end web work has to prove it on its own site first, so this one is held to the same bar as client builds: deliberate typography, motion with a purpose, and accessibility that survives the animation.

It's also the public record of my work. Every case study comes from one typed source, so a project can't be described two different ways on two different pages.

## What I built

I founded Higgins Digital and designed and built its site:

- Information architecture across home, work, case studies, services, pricing, about, contact, blog, and location pages
- A single typed content source that feeds the work grid, every case study, related links, and metadata
- Motion: route transitions, a full-screen menu with marquee hover bands, and scroll scenes, all with reduced-motion paths
- SEO foundations: generated sitemap and robots, structured data, per-page metadata, and an MDX blog
- A private sign-in area that isn't part of this showcase

## How it's put together

```mermaid
flowchart TB
    C[Typed content sources<br/>projects · services · pricing] --> P[Next.js App Router pages]
    M[MDX articles] --> P
    P --> S[Static, SEO-ready routes<br/>sitemap · structured data]
    P --> X[Client motion layer<br/>GSAP · ScrollTrigger · Lenis]
    S --> V[Vercel]
    X --> V
```

### Engineering decisions

| Decision | Why |
|---|---|
| **One source of truth for the work** | Every project lives once in a typed data file that feeds the grid, case studies, related links, and metadata. A test fails the build if a project's images are missing. Outcomes can only appear with a cited source, so there are no invented performance numbers. |
| **Motion is scoped and reversible** | Animations are built with component-scoped GSAP contexts and explicit ScrollTrigger cleanup, so route changes never leave stale listeners behind. Every animated section has a `prefers-reduced-motion` equivalent. |
| **Accessible structure under the effects** | Clickable areas are real links and buttons. The menu traps and restores focus and works from the keyboard. Low-contrast brand colors were adjusted until filled controls cleared WCAG AA. |

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

| Layer | Technology | Responsibility |
|---|---|---|
| Framework | Next.js 15 (App Router), React 19, TypeScript, Tailwind CSS | Pages, routing, metadata |
| Content | Typed data modules, MDX (next-mdx-remote) | Case studies, services, articles |
| Motion | GSAP with ScrollTrigger, Lenis, Three.js | Transitions, menu, scroll scenes |
| Data | Supabase | Private client area and website-audit request intake |
| Quality | Playwright | End-to-end and data-integrity checks |
| Hosting | Vercel | Deployment |

## Credits and notes

- **Design lineage.** Parts of the presentation layer (page composition, GSAP timing values, and navigation and transition structure) derive from the open-source [K72 recreation](https://github.com/AyushAwasthi26/K72) by Ayush Awasthi, under the MIT License. I ported it from Vite and React Router to the Next.js App Router and substantially rewrote it, including reduced-motion handling, semantic controls, and focus management that the original lacked.
- **Typography in this repository.** The live site is set in a commercial typeface. The cover graphic above uses Inter Tight as a free stand-in and doesn't redistribute any font.
- **No invented metrics.** The site and this showcase report scope, not traffic or conversion numbers.

## About this repository

This is a documentation-only showcase. The site's source, client data, and private areas aren't included here.

**[Visit higginsd.com ↗](https://www.higginsd.com)** · Built by [Davis Higgins](https://davishiggins.com) · [More of my work](https://github.com/DavisHiggins)

<sub>© 2026 Davis Higgins. Text and images in this repository are shared for portfolio viewing. The Higgins Digital name and logo belong to Davis Higgins. Project imagery shown in screenshots belongs to the respective projects and clients.</sub>
