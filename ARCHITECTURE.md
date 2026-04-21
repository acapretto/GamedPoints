# ARCHITECTURE.md — Gamified Points System

No code written yet. This file will be updated as decisions are made during build.

## Planned Stack
- Frontend: React + TypeScript (Vite)
- Backend: Node.js + Express (or Supabase Edge Functions)
- Database: Supabase (Postgres)
- Auth: Supabase Auth (teacher only; students use class code)
- Deployment: Netlify (frontend) + Supabase (backend/db)

## Planned Architecture

### Data Model (draft)
- `teachers` — teacher accounts
- `classes` — one per class section (has a join code)
- `activity_types` — customizable per class (Quiz, Project, Video, etc.) with point values
- `students` — linked to class via join code, no auth
- `point_records` — one row per earned activity (student, activity_type, points, date, note)

### Key Screens
- Teacher: Activity type manager, point entry (bulk/single), class dashboard
- Student: Personal dashboard (total points, progress bar, activity breakdown)

### Decisions to Lock During Build
- Whether students need accounts or just a name + class code
- Point entry flow: teacher-only vs. student self-report with teacher approval
- Leaderboard: opt-in per class (some teachers will not want it)
