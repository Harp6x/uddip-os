# Project Portfolio

> Detailed breakdown of every project in the Uddip ecosystem.

---

## 1. Before Maps

**Mission:** Exploration-led travel company discovering meaningful experiences across India — iconic, emerging, and overlooked places experienced through a different lens.

**Audience:** Independent travelers (25–40) who want curated, scouted journeys — not package tours.

**Business Model:**
- Application-based group journeys (8–12 people, transparent pricing)
- Digital travel products (guides, toolkits on Gumroad)
- Future: retreats, custom journeys

**Technology:**
| Layer | Stack |
|---|---|
| Framework | Next.js 16.2.9 (App Router), TypeScript, React 19 |
| CMS | Sanity v5 (embedded `/studio`, 15 document types) |
| Styling | Tailwind CSS v4, shadcn/ui components |
| Hosting | Vercel (auto-deploy from GitHub) |
| Analytics | Vercel Analytics |

**Status:** Active. Content seeding in progress, scouting routes, building CMS content.
**Live URL:** beforemaps.com (or staging)
**Sanity Project:** c4zc1cd4 / production

**Key Docs:** `CLAUDE.md`, `docs/AGENTS.md`, `docs/ARCHITECTURE.md`, `docs/CONTENT-STRATEGY.md`

---

## 2. Hobie

**Mission:** Gamified hobby tracker that makes pursuing hobbies feel like a game — quests, XP, levels, timers, streaks.

**Audience:** Anyone who wants to build hobby habits with gamification. Mobile-first PWA.

**Business Model:** Free. Future potential for premium features.

**Technology:**
| Layer | Stack |
|---|---|
| Framework | Vite 8, React 19, TypeScript |
| Auth | Supabase (Google OAuth + Magic Link) |
| State | localStorage-first + Supabase cloud sync |
| Styling | Tailwind CSS v4 |
| PWA | vite-plugin-pwa |
| Hosting | Vercel |

**Status:** Active. v1.1 live at hobie-deploy.vercel.app.

**Key Docs:** `CLAUDE.md`, `docs/AGENTS.md`, `docs/lessons/`

---

## 3. Ms Paul Therapies

**Mission:** Professional online therapy practice for Aishani Paul (RCI-licensed clinical psychologist). Lead generation + educational content platform.

**Audience:** Indian adults (25–45) seeking mental health support — professionals, couples, parents, students. Also NRIs.

**Business Model:** Client therapy sessions booked via Cal.com/Google Forms. Digital products (workbooks, guides). Newsletter (Kit/ConvertKit).

**Technology:**
| Layer | Stack |
|---|---|
| Framework | Next.js 16.2.6 (App Router), TypeScript, React 19 |
| CMS | Sanity v5 (12 document types) |
| Styling | Tailwind CSS v4 (sage/cream/terracotta palette) |
| Forms | Google Forms + Cal.com |
| Newsletter | Kit (ConvertKit) |
| SEO | 10+ JSON-LD builders, sitemap, robots, llms.txt |
| Hosting | Vercel |

**Status:** Active. Live at mspaultherapies.in.
**Sanity Project:** k0r3y2my / production

**Key Docs:** `CLAUDE.md`, `AGENTS.md`, `MASTER-RCA.md`, `docs/ARCHITECTURE.md`

---

## 4. Uddip Content

**Mission:** Complete content library powering three brands: HARP6X (systems lab), ThereGoesUddip (field journal), and Before Maps (travel company).

**Audience:** Internal — used by Uddip to publish across platforms.

**Business Model:** Supports content marketing and digital product creation for all brands.

**Technology:** Pure markdown repository. 2,100+ files organized by brand and content type.

**Structure:**
- `harp6x/` — AI, cybersecurity, creator systems, productivity
- `theregoesuddip/` — Solo travel, Himalayan treks, slow travel, emotional essays
- `before-maps/` — Journey content, scouting reports, field notes (1,250+ pieces)
- `_os/` — Operating system docs, calendars, strategy
- `digital products empire/` — Product blueprints, launch plans
- `automation/` — Workflow automation scripts and templates

**Status:** Active. Continuously growing.

**Key Docs:** `README.md`, `SITEMAP.md`, `_os/`

---

## 5. Aishani Content

**Mission:** Complete content engine for Ms Paul Therapies — everything Aishani needs to run Instagram, YouTube, blog, email, client work, and digital products.

**Audience:** Internal — used by Aishani Paul for her therapy practice content.

**Business Model:** Supports content marketing and digital products for Ms Paul Therapies.

**Technology:** Pure markdown repository. 700+ files + 10 branded PDFs.

**Structure:**
- `content/` — Blog articles, reel scripts, carousel scripts, series outlines
- `digital-products/` — Workbooks, worksheets, guides for clients
- `checklists/` — Clinical and business checklists
- `questionnaires/` — Assessment tools
- `growth-playbook/` — Marketing strategy and growth plans
- `mspaultherapies/` — Website-specific content
- `pdfs/` — Branded downloadable PDFs

**Status:** Active. Continuously growing.

**Key Docs:** `README.md`, `SITEMAP.md`
