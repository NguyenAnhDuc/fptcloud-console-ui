# AGENTS.md — fptcloud-console-ui

> Single source of truth. CLAUDE.md symlinks here.
> `ln -s AGENTS.md CLAUDE.md`

FPT Cloud Console UI — React + MUI frontend for Vietnam's public cloud platform (comparable to AWS/GCP console).
This repo is the frontend SPA for console.fptcloud.com. New features are added as modules under src/pages/ + src/components/.
Stack: React 18 · MUI v5 · REST /api/v1/ (backend: fptcloud-portal-api) · FPT ID OAuth (JWT)

## Commands
- `npm start` — run dev server
- `npm test` — run tests (React Testing Library)
- `npm run lint` — ESLint
- `npm run build` — production build

## Zone map
FROZEN (hotfix only — AI MUST NOT touch):
- `src/auth/` — FPT ID OAuth integration
- `src/core/` — shared layout, routing, theme

GROWTH (new features OK):
- `src/components/FeedbackWidget/`
- `src/pages/AdminReport/`

## Gold standard
See `src/components/_gold-standard/` — reference component pattern.
Read before generating any new component.

## Cross-repo
API contract: see CONSTITUTION.md (synced from fptcloud-portal-api)
Backend must deploy to staging BEFORE FE integration starts.

## Skill Activation
| Task | Skill |
|------|-------|
| Create new component/page | .claude/skills/gold-standard/SKILL.md |
| Review code | .claude/skills/code-review/SKILL.md |
