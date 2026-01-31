# Interview Practice Reps App

A lightweight web app to help you get many realistic interview practice reps, so you never walk into a job interview under‑prepared again.

Instead of waiting for mock interviews with friends, you can quickly run timed, on‑camera practice sessions on your own schedule.

---

## Problem

Most candidates do not get enough meaningful practice before interviews:

- Scheduling mock interviews with friends or peers is hard.
- Even when they happen, they may not feel realistic or structured.
- Practising alone with pen and paper does not create time pressure or accountability.

The result: people enter interviews rusty, anxious, and under‑rehearsed.

---

## What this app does

This app lets you:

- Define the questions or themes you want to practise (e.g. “Tell me about yourself”, “Product sense”, “Behavioural: conflict with a colleague”).
- Run short practice sessions where:
  - The app shows questions one by one, randomly or from your set.
  - You have a fixed time (default 2 minutes) to answer each question out loud.
  - Your device camera records your answer for each question.
- Review your past sessions:
  - Rewatch individual clips.
  - Add quick reflection notes on what went well and what to improve.

The focus is on **reps**: doing many realistic runs, not over‑analyzing each one.

---

## Key features (MVP)

- Create and manage question sets.
- Configure session length (number of questions) and time per question.
- Timed practice sessions with camera recording and visible countdown.
- Automatic saving of short video clips per question.
- Session history with per‑question playback and simple notes.

---

## Product artefacts

This repository captures the full product development process:

- [`PRD.md`](./PRD.md) – problem, target users, goals, scope, and flows.
- `designs/` – exported mocks from Google Stitch (user flows, key screens).
- App source code – implementation for the web app (built with cto.new and manual edits).

If you are reviewing this as part of my portfolio, start with `PRD.md`, then skim the designs, and finally look at how the implementation maps back to the product goals.

---

## Tech stack (planned)

- Frontend: (to confirm) React / Next.js web app.
- Video: in‑browser camera capture using the MediaRecorder API or similar.
- Backend / storage: (TBD – depends on hosting choice), used to store sessions, metadata, and video clips.
- Development workflow: GitHub repository connected to cto.new for structured branches and pull requests.

This section will be updated as the implementation firms up.

---

## Development workflow

For this project I aim to:

- Use GitHub Issues to track product tasks (PRD, designs, core flows).
- Use branches and pull requests (including from cto.new) for each meaningful feature.
- Keep documentation and code in sync, updating `PRD.md` and this `README.md` as the product evolves.

This repo is intentionally structured to show both *how* I think about the product and *how* I build it.

---

## Status

Early MVP – currently working on:

- Finalising PRD and initial user flows.
- Designing key screens in Google Stitch.
- Wiring the first version of the web app via cto.new.

Follow the commit history and open pull requests to see progress over time.
