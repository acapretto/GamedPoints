# PRD — Gamified Points System

## Overview
A grading & motivation platform that lets students accumulate points through diverse activities (tests, projects, videos, tutoring, real-world applications) toward a mastery threshold (10,000 points = A). Replaces rigid percentage-based grading with flexible, student-centered pathways.

## Problem Statement
Traditional grading:
- 90% = A (fixed path: tests only)
- Students who excel at projects, creativity, or application have no path to "A"
- **Result:** Demotivation, disengagement, loss of students who learn differently

## User Stories

### Story 1: Teacher Defines Activity Types
- Teacher creates activity type: "Quiz" (100 pts per quiz)
- Teacher creates: "Project" (500 pts per project)
- Teacher creates: "YouTube Explanation" (200 pts)
- Teacher sets mastery threshold (default: 10,000 pts)
- **Outcome:** Custom points for diverse learning modalities

### Story 2: Student Earns Points Multiple Ways
- Student A takes 10 quizzes (1,000 pts) + 1 project (500 pts) + 2 videos (400 pts) = 1,900 pts
- Student B takes 5 quizzes (500 pts) + 3 projects (1,500 pts) + 1 real-world application (200 pts) = 2,200 pts
- **Outcome:** Multiple paths, same "currency"

### Story 3: Student Monitors Progress
- Student dashboard shows point total, progress bar to 10K
- Breakdown by activity type (visually appealing)
- Celebration when threshold reached
- **Outcome:** Transparent progress, autonomy, motivation

### Story 4: Teacher Tracks Class-Wide Progress
- Dashboard shows: students by points (leaderboard-optional), % of class at each threshold
- Teacher can adjust point values mid-year if needed
- Can override points if student challenges
- **Outcome:** Data-driven, responsive grading

## MVP Features (V0.1)

| Feature | Scope |
|---|---|
| Teacher admin panel (create activities, set point values) | ✅ |
| Student point entry (manual, for now) | ✅ |
| Student dashboard (total points, progress bar, breakdown by type) | ✅ |
| Mastery threshold (configurable, default 10K) | ✅ |
| Activity history view (student sees all logged activities) | ✅ |
| Teacher class dashboard (student list, points, progress) | ✅ |
| Local data storage (export CSV) | ✅ |

## Out of Scope (V0.1)
- Canvas integration (manual entry only)
- Automated point logging from assessments
- Student-facing point challenges/disputes
- Mobile-responsive design
- Leaderboard/competitive features
- Parent portal

## Success Metrics
- **Adoption:** 3+ teachers using with real classes
- **Student Engagement:** Self-reported motivation increase (survey)
- **Teacher Feedback:** "System is easier to use than Excel gradebook"
- **Completion Rate:** 5+ students hit 10K threshold in pilot

## Assumptions & Risks

| Assumption | Risk | Mitigation |
|---|---|---|
| Teachers will use multiple activity types | Teachers default to tests only (old habits) | Provide templates + examples + guide |
| Points feel motivating, not arbitrary | Students optimize for easy points, not learning | Build "activity quality" meta-rules (no max points from any one type) |
| 10K is the right threshold | Some classes finish too fast / too slow | Make threshold configurable, provide guidance |

## Success Criteria for V0.1
- Supports 30+ students in 1 class without slowdown
- Teacher can enter 100 point records in < 5 min (batch import)
- 80% of students report understanding their progress
