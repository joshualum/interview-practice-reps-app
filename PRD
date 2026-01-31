# Interview Practice Reps App – PRD

## 1. Problem Overview

### 1.1 Who has this problem

- Job seekers preparing for upcoming interviews (students, early‑career, mid‑career switchers).
- Busy professionals interviewing infrequently who feel “rusty” and under‑practised.
- Candidates without easy access to experienced interview partners or mentors.

### 1.2 Core problem

Getting enough *meaningful* interview practice reps is hard:

- To simulate a real interview today, people rely on mock interviews with friends or peers, which are difficult to schedule and coordinate.
- Even when mock interviews happen, they often do not feel realistic and provide limited structured reflection or feedback.
- Practising alone (e.g. thinking through answers in your head or on paper) does not create the pressure, time‑boxing, or accountability of a real interview.

As a result, many candidates walk into interviews under‑prepared, with too few real practice reps and low confidence.

---

## 2. Existing solutions and gaps

### 2.1 Current behaviours

- Mock interviews with friends, colleagues, or community groups.
- Solo practice with pen and paper (writing answers, brainstorming stories).
- Ad hoc use of YouTube videos, blog question lists, or note apps to rehearse.

### 2.2 Gaps

- Scheduling friction: coordinating times with partners is hard, so practice reps are infrequent.
- Low realism: mock interviews rarely simulate being “on the spot” with a camera and a strict time limit.
- Weak feedback loops: candidates often do not review their performance in a structured way, so it is hard to notice patterns and improve across reps.
- High activation energy: starting a practice session feels heavy, so people procrastinate and enter interviews under‑rehearsed.

---

## 3. Product concept

### 3.1 Product vision

A lightweight web app that makes it easy to get many realistic interview practice reps, on your own schedule, with minimal friction and just enough self‑reflection to improve.

### 3.2 Core idea

- The user tells the app what questions or themes they want to practise (e.g. “Tell me about yourself”, “Product sense questions”, “Behavioural: conflict with a colleague”).
- The app simulates an interviewer by presenting questions one by one, randomly or from a configured set.
- For each question, the user has a fixed time box (e.g. 2 minutes) to answer out loud while their device camera records them.
- Each answer is saved as a short video clip that the user can later review to evaluate their performance.
- The emphasis is on getting *many* reps done quickly, not spending a lot of time scoring every single answer.

---

## 4. Target users and personas

### 4.1 Primary persona

- **Name:** Alex, 29, product manager candidate  
- **Context:** Working full‑time, interviewing occasionally, struggles to find consistent time and partners to practise.  
- **Needs:** 
  - A way to practise common product and behavioural questions in a realistic setting.
  - Low‑friction sessions that can fit into 15–30 minute breaks.
  - A way to look back at how they actually communicated, not just what they intended to say.

### 4.2 Secondary personas

- Final‑year students preparing for internship/graduate role interviews.
- Career switchers doing multiple interviews across different companies and roles.

---

## 5. Goals and non‑goals

### 5.1 Goals (MVP)

- Allow a user to define a set of questions or select from simple presets.
- Run timed practice sessions where:
  - A question is shown on screen.
  - A countdown (e.g. 2 minutes) runs.
  - The user’s camera records their response.
- Save each answer as a separate video clip tied to the question and timestamp.
- Provide a simple history view where users can:
  - See past sessions.
  - Click into a session to replay clips and jot down quick reflections.

### 5.2 Non‑goals (for MVP)

- Automated AI scoring or detailed coaching on performance.
- Complex scheduling with other humans, marketplaces for interviewers, or live mock sessions.
- Detailed analytics dashboards or advanced tagging of every clip.
- Native mobile apps (initial focus is a responsive web app).

---

## 6. User experience flow (MVP)

### 6.1 Onboarding

1. User lands on home page, sees a short explanation of the app and a “Start practising” CTA.
2. User signs in or continues as a simple account (email / magic link or similar).
3. User is prompted to set up their first question set.

### 6.2 Creating a question set

1. User creates a “Question set” (e.g. “PM behavioural”, “Thermo Fisher onsite prep”).
2. User enters questions manually or selects from a small list of starter templates.
3. User chooses:
   - Time limit per question (default 2 minutes).
   - Number of questions per session (e.g. 5, 10).

### 6.3 Running a practice session

1. User clicks “Start session”.
2. App:
   - Randomly picks the first question from the active set.
   - Shows the question full screen with a short buffer countdown (e.g. 3 seconds).
3. Recording starts:
   - Camera preview + timer visible.
   - At 2 minutes, recording auto‑stops and the app transitions to the next question.
4. Repeat until all questions for that session are answered.
5. At the end, user sees a “Session complete” screen with a list of questions and their corresponding video clips.

### 6.4 Review and reflection

1. From the session summary, user can:
   - Tap on any question to replay the associated video.
   - Add a quick note (e.g. “Too long intro”, “Good example here”, “Need better structure”).
2. Later, the user can go to a “History” page to:
   - Filter by question set.
   - Rewatch clips from recent sessions.

---

## 7. Scope and requirements (MVP)

### 7.1 Functional requirements

- Question management:
  - Create, edit, delete question sets.
  - Add, edit, delete individual questions.
- Practice engine:
  - Start session for a given question set.
  - Randomise question order within a session.
  - Time‑boxed answering with a visible countdown.
  - Automatic transition to the next question after time expires.
- Video capture:
  - Request camera and microphone access from browser.
  - Record and save each response as a separate clip.
  - Store metadata: question ID, timestamp, session ID, duration.
- Session history:
  - List of recent sessions, each with date/time and number of questions.
  - Detail view with list of questions, associated clips, and quick notes.
- Basic auth:
  - Simple account system to keep sessions and clips private to each user.

### 7.2 Non‑functional requirements

- Runs well in modern desktop and mobile browsers.
- Makes it clear when camera/mic are in use, with explicit permissions and an easy way to stop.
- Data stored securely; users can delete sessions and associated videos.

---

## 8. Success metrics (early)

- Activation:
  - % of new users who complete at least 1 full practice session within 24 hours.
- Engagement:
  - Median number of questions answered per session.
  - % of users who complete 3+ sessions in a week.
- Perceived value (qualitative):
  - “I feel more prepared for interviews after using this” (self‑reported).
  - “This made it easier to get real practice reps compared to my old approach” (self‑reported).

---

## 9. Open questions / future ideas

- AI‑assisted feedback on body language, filler words, and structure.
- Recommended question sets per role (PM, SWE, consulting, etc.).
- Sharing selected clips with mentors or friends for comments.
- Calendar‑based streaks and goals (e.g. “10 questions per day for 7 days”).
