# CLAUDE.md — Gamified Points System

## Project Vision
Replace traditional percentage-based grading (90% = A) with open-ended point accumulation. Students earn points through diverse activities: assessments, projects, videos, real-world applications, peer tutoring. Master level = 10,000 points by any path. Flexibility + motivation.

## Context
- **Category:** Gamification & Alternative Assessment
- **User:** Math teacher (Andrew) wanting to move beyond rigid grading
- **Pain Point:** Students who don't test well have no other path to "A"
- **Target Model:** Classroom tool (free or TpT bundle); later Canvas integration

## Tech Stack
- **Frontend:** React + TypeScript (Vite)
- **Backend:** Node.js + Express or Firebase
- **Database:** Supabase or Firebase Firestore
- **Auth:** Teacher admin panel + Canvas SSO (later)
- **Reporting:** Student dashboard, teacher analytics
- **Deployment:** Netlify

## Conventions & Standards
- **Point Value Design:** Configurable per activity type; teacher can adjust on the fly
- **Activities:** Tests, projects, videos, real-world applications, peer tutoring (extensible)
- **Testing:** Unit tests for point calculation logic, E2E for workflows
- **Naming:** camelCase functions, PascalCase components

## Status & Milestones
- **V0.1 (March 2026):** Activity creation, point entry, student dashboard, 10K threshold
- **V0.2:** Multi-class support, activity templates
- **V1.0:** Canvas integration, detailed reporting, parent access
