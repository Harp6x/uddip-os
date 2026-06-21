# Hobie — Project Summary

**Repo:** `Harp6x/hobie` | **Local:** `~/Documents/code/hobie`
**Live:** hobie-deploy.vercel.app

---

## Mission
Gamified hobby tracker that makes pursuing hobbies feel like a game — quests, XP, levels, timers, streaks. Mobile-first PWA.

## Audience
Anyone who wants to build hobby habits with gamification. Primarily mobile users.

## Business Model
Free. No monetization yet. Future potential for premium features (cloud sync, social, advanced analytics).

## Technology
Vite 8 · React 19 · TypeScript · Supabase (Google OAuth + Magic Link) · react-router 7 · Tailwind CSS v4 · vite-plugin-pwa · Vercel

## Roadmap
1. User feedback collection
2. Feature iteration (based on feedback)
3. v2.0 — social features, sharing
4. Premium tier exploration

## Dependencies
- **Supabase** — Auth and cloud sync
- **Vercel** — Hosting
- Standalone — no dependency on other projects

## Relationship to Other Projects
- Independent app — no content, CMS, or code shared with other projects
- Same founder, same GitHub org, same deployment platform
- Could cross-promote with Before Maps (adventure hobbies) but currently separate

## Key Technical Notes
- **Timer pattern:** Wall-clock `Date.now()` — NEVER tick-based `setInterval(s+1)`. Browsers throttle intervals in background tabs.
- **State:** localStorage-first (`hobie_progress_v4`) with optional Supabase cloud sync
- **Known TS errors:** Unused Radix UI imports in `ui/` components — safe to ignore
- **Version:** Always bump `APP_VERSION` in `SettingsPage.tsx` AND `version` in `package.json` together

## Documentation
| Doc | Purpose |
|---|---|
| `CLAUDE.md` | AI standalone context |
| `AGENTS.md` | Quick reference |
| `docs/AGENTS.md` | Full AI context |
| `docs/lessons/` | Hard-learned rules (timers, git remotes) |
