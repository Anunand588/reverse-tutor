# Reverse Tutor for B.Tech

A single-file web app for B.Tech students: teach a topic to the app (reverse tutoring), solve scenarios, take chapter quizzes, track progress, and compete in daily and monthly challenges.

## Features
- **Teach (reverse tutoring):** explain a topic by typing, speaking or uploading a file/PDF; the app asks doubts and scores each answer. Get revision notes from your explanation.
- **Scenarios:** four difficulty levels (Easy, Medium, Hard, Expert) with points.
- **Performance tracker:** total time, time per question, points, scenarios solved by difficulty, progress charts.
- **Chapter quiz:** multiple-choice quiz per chapter with saved marks.
- **Syllabus:** tick covered chapters and see reminders for uncovered ones.
- **Daily logic question:** a new question every day (midnight IST), ranked by time.
- **Discussion, leaderboards and monthly hackathon:** shared boards with AI evaluation.
- Curriculum: Year 1 (common) plus CSE, ECE, EEE, Mechanical and Civil for years 2-4.

## Running it
Open `index.html` in a browser, or host it with GitHub Pages (Settings > Pages > Deploy from branch > `main` / root).

## Important: features that need a backend
The AI-powered and shared features were built for the claude.ai artifact runtime (`window.claude`). Outside it (for example on GitHub Pages):

| Works on GitHub Pages | Needs your own backend |
|---|---|
| Syllabus tracking and reminders, tracker and charts, daily question (local), voice input, file/PDF upload, basic offline doubts and scoring | AI doubts and scoring quality, notes generation, chapter quiz, discussion board, leaderboards, hackathon, file sharing |

To enable the second column, connect your own database (for example Firebase) and an AI API behind a server (never put an API key in the page).

## Data
Progress is stored in the browser (`localStorage`) under the key `rt`.
