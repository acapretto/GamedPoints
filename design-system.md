# design-system.md — Gamified Points System

## Principles
- Motivating and game-like for students without being childish
- Clean and data-dense for the teacher dashboard
- Mobile-first for student view (students use phones)

## Color Palette (draft)
| Token | Value | Use |
|---|---|---|
| Primary | `#1d4ed8` | Buttons, headings, progress fill |
| Success | `#15803d` | Milestones reached, positive feedback |
| Accent | `#7c3aed` | Point badges, game-like elements |
| Warning | `#c2410c` | Streak risk, approaching deadline |
| Background | `#f1f5f9` | Page background |
| Card | `#ffffff` | Content cards |

## Components (to define during build)
- Point badge — circular, shows numeric points earned
- Progress bar — toward 10K threshold, color shifts as student gets closer
- Activity chip — small colored tag per activity type
- Leaderboard row — rank, name, points, progress bar (compact)

## Stack
- React + TypeScript
- Tailwind CSS
- No external UI component library (build from primitives)

## Conventions
- Student view: large numbers, celebration states, minimal chrome
- Teacher view: dense tables, sortable columns, inline edit
