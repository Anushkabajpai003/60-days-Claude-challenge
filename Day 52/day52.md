# Day 52 — AB Talks 60-Day Claude AI Challenge

**Capstone Progress: Day 2 of 10 — System Design**

## What I Did Today

Continued my 10-day capstone project — **AI Habit Coach**, a habit tracker with a real Claude-powered AI coach that sends personalized motivation, detects behavioral patterns, and holds short coaching conversations.

Today's focus was pure system design — no production code yet. The goal: turn yesterday's product plan into a complete technical blueprint so implementation can start immediately tomorrow with zero ambiguity.

## Key Work Completed

- **Repository setup:** Created the GitHub repo (`ai-habit-coach`), cloned it locally, and scaffolded the initial project structure.
- **Tech stack finalized:** Python + Flask, SQLite (dev) → PostgreSQL (prod), Anthropic Claude API, Render.com hosting — all free-tier, chosen specifically to fit a 1–2 hr/day build pace.
- **System architecture designed:** Component diagram, request lifecycle, and AI interaction flow, all documented with Mermaid diagrams.
- **Database schema designed:** Two tables (`habit`, `check_in`), validated against every user story in the PRD. Added a unique constraint on `(habit_id, date)` as an improvement over the original plan, to enforce duplicate-check-in prevention at the database level.
- **API contract designed:** All 7 endpoints needed for v1.0 — habit CRUD, check-ins, and coach chat — fully specified with request/response/validation/error handling, before writing any implementation.
- **UI/UX designed:** A 2-screen user flow (Homepage + Coach Chat), with low-fidelity wireframes and navigation mapped out.
- **Project structure finalized:** Clear one-responsibility-per-file layout so every future day knows exactly where new code belongs.

## What I Learned

Design discipline up front massively de-risks the days ahead. By validating the database schema against every single user story — and mapping every planned feature to a specific API endpoint — I caught and fixed a small gap (duplicate check-in prevention) before it could become a bug later in the build.

## Commit Reference

Full Day 2 system design work committed and pushed to the capstone repository:
[`d646316` — "Day 2: System design - architecture, schema, API, UI wireframes, project structure"](https://github.com/Anushkabajpai003/ai-habit-coach/commit/d646316582baf2041d32236bccb885045f0e9ddc)

## Next Up

Day 3 of the capstone (Day 53 of the challenge): implementing the database models and habit CRUD functionality — the first real, working code.