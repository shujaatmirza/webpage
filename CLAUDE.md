# Shujaat Mirza — Personal Academic Website

## Overview
Jekyll-based academic portfolio hosted on GitHub Pages at **shujaatmirza.com**.
Repo: `git@github.com:shujaatmirza/webpage.git` on `master` branch.

## Tech Stack
- **Jekyll** with `jekyll-theme-minimal` (heavily customized)
- **SCSS** design system with CSS custom properties
- **GitHub Pages** deployment (auto-builds on push to master)
- **Google Analytics** GA4: `G-N7CS1PGEX1`

## Key Files
- `_config.yml` — Site title, description, theme config
- `_layouts/default.html` — Full custom layout (sidebar + content), fonts, GA4, favicon
- `assets/css/style.scss` — Complete design system (colors, typography, layout, responsive)
- `index.md` — All page content (bio, interests, education, news, publications)
- `assets/img/headshot-opt.jpeg` — Optimized profile photo (400x400, ~33KB)
- `assets/img/favicon-64.png` — 64x64 favicon
- `assets/img/headshot.jpeg` — Original high-res profile photo (archived)
- `papers/` — PDF files for publications

## Design System

### Colors (CSS custom properties in `:root`)
- Background: `#f4f3ef` (warm off-white)
- Surface/content: `#ffffff`
- Sidebar: `#f9f8f6`
- Ink (headings): `#1c1917`
- Body text: `#3c3836`
- Secondary: `#706b65`
- Muted: `#857f78` (WCAG AA compliant)
- Faint: `#9e9890` (footer text, WCAG AA compliant)
- Rule decorative: `#d1ccc5` (non-text borders/underlines only)
- Accent (links, section rules): `#3d5a80` (steel blue)
- Award gold: `#7d5e12` on `#faf4e6`

### Typography
- **EB Garamond 500 (regular + italic)** — sidebar name, publication titles, news emphasis
- **Inter 400/500/600** — everything else
- Type scale: 27px (name) / 16.5px (pub titles) / 15.5px (news emphasis) / 15px (body) / 13px (dates, venues) / 11px (labels, badges)

### Layout
- Fixed sidebar (280px) with 3px accent bar at top, profile image, name, tagline, social icons
- Content area with max-width 780px
- Sidebar has no border — separation via background color + subtle box-shadow on content
- Profile image: 140px circular with white border ring + rule-color outline (double ring)
- Publications have left accent border (2px) that turns steel blue on hover
- Skip-to-content link for keyboard accessibility

### Responsive Breakpoints
- **960px**: Sidebar stacks on top (soft shadow separation), content below. Text bumped to 16px. Icons bigger (18px) with 44px circular touch targets. News items get bottom borders for scannability.
- **380px**: Tighter padding for very small screens.

## Content Structure (index.md)
1. **Bio** — Two paragraphs. P1: current role at Microsoft AI Red Team, research focus on loss of control. P2: previous roles (MATS, Spotify).
2. **Interests & Education** — Two-column layout with icons. Interests: Autonomy and Loss of Control, Adversarial ML, Harmful Manipulation, Privacy-Enhancing Technologies. Education: PhD/MPhil/BS all from NYU institutions (no years shown).
3. **Recent Highlights** — Timeline with date + description. 9 items from Fall 2025 to May 2023.
4. **Research** — 5 selected publications with venue locations. Two have award badges (Distinguished Artifact Award, Best Paper Award).
5. **Scholar CTA** — Link to Google Scholar with arrow.
6. **Footer** — Copyright 2026.

## Social Links (in layout)
- Email: shujaat.mirza@nyu.edu
- Google Scholar: scholar.google.com/citations?user=6mJvLd4AAAAJ
- LinkedIn: /in/shujaatmirzaa/
- X: x.com/shujaatmirzaa

## Design Decisions & Rationale
- No GitHub link (intentional removal)
- Section headings are uppercase 11px labels with short 36px steel-blue accent rule underneath
- Publications have left-border accents; no borders between news items on desktop (spacing only)
- Award badges are gold uppercase pills, used sparingly
- Social icons use `--color-muted` with tinted background hover (6px rounded rect on desktop, 44px circle on mobile)
- Profile image has double-ring treatment (white border + rule outline) with subtle hover scale
- Name links to https://www.shujaatmirza.com/
- Font loading includes EB Garamond regular + italic (used for pub titles and emphasis)
- All text colors meet WCAG AA contrast requirements
- Skip-to-content link and focus-visible outlines for keyboard navigation
