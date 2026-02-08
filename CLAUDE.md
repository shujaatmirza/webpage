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
- `assets/img/headshot.jpeg` — Profile photo (also used as favicon)
- `papers/` — PDF files for publications

## Design System

### Colors (CSS custom properties in `:root`)
- Background: `#f4f3ef` (warm off-white)
- Surface/content: `#ffffff`
- Sidebar: `#f9f8f6`
- Ink (headings): `#1c1917`
- Body text: `#3c3836`
- Secondary: `#706b65`
- Accent (links): `#3d5a80` (steel blue)
- Award gold: `#7d5e12` on `#faf4e6`

### Typography
- **EB Garamond 500** — sidebar name only
- **Inter 400/500/600** — everything else
- Type scale: 27px (name) / 16px (reserved) / 15px (body) / 13px (dates, venues) / 11px (labels, badges)

### Layout
- Fixed sidebar (280px) with profile image, name, tagline, social icons
- Content area with max-width 780px
- Sidebar has no border — separation via background color + subtle box-shadow on content
- Profile image: 140px circular with white border ring

### Responsive Breakpoints
- **960px**: Sidebar stacks on top, content below. Text bumped to 16px. Icons bigger (18px) with tighter gap.
- **380px**: Tighter padding for very small screens.

## Content Structure (index.md)
1. **Bio** — Two paragraphs. P1: current role at Microsoft AI Red Team, research focus on loss of control. P2: previous roles (MATS, Spotify).
2. **Interests & Education** — Two-column layout with icons. Interests: Autonomy and Loss of Control, Adversarial ML, Harmful Manipulation, Data Privacy. Education: PhD/MPhil/BS all from NYU institutions (no years shown).
3. **Recent Highlights** — Timeline with date + description. 9 items from Fall 2025 to May 2023.
4. **Research** — 5 selected publications with venue locations. Two have award badges (Distinguished Artifact Award, Best Paper Award).
5. **Scholar CTA** — Link to Google Scholar with arrow.
6. **Footer** — Copyright 2025.

## Social Links (in layout)
- Email: shujaat.mirza@nyu.edu
- Google Scholar: citations?user=6mJvLd4AAAAJ
- LinkedIn: /in/shujaatmirzaa/
- X/Twitter: @shujaatmirzaa

## Design Decisions & Rationale
- No GitHub link (intentional removal)
- Section headings are uppercase 11px labels with short 32px accent rule underneath
- No borders between news/pub items — spacing only
- Award badges are gold uppercase pills, used sparingly
- Social icons use `--color-muted` (not faint) for visibility
- Name links to https://www.shujaatmirza.com/
- Font loading is trimmed to only used weights to save bandwidth
