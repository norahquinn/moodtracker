# AGENTS.md

## Project

Build a **Mood Tracker** web app for GitHub Pages. The app should run entirely in the browser and save user data locally using `localStorage`.

## Goal

Create a simple, calm, and easy-to-use app that lets a user record their mood each day, view past entries, and see mood trends in a small chart.

## Target User

The user is someone who wants a low-pressure way to notice mood patterns over time. The app should feel supportive and private, not clinical or judgmental.

## Hosting Constraints

- The app will be hosted on **GitHub Pages**.
- Use only static front-end files: HTML, CSS, and JavaScript.
- Do not require a backend server, database, login, or paid API.
- All data must be stored in the browser using `localStorage`.

## Core Features

The app must include:

1. A daily mood entry form.
2. Mood choices represented by icons or emoji-style labels.
3. Optional short notes for each mood entry.
4. A list or calendar-style view of previous entries.
5. A simple chart showing mood trends over time.
6. The ability to delete an entry.
7. A clear message explaining that data is stored only in the browser.

## Mood Options

Use a small set of readable mood options, such as:

- Great
- Good
- Okay
- Tired
- Sad
- Stressed

Each mood should have a visual icon and a numeric score for charting.

## Design Requirements

- Use a soft, calming visual style.
- Make the layout responsive for mobile and desktop.
- Keep the interface simple and not overwhelming.
- Use accessible color contrast.
- Do not use harsh language, guilt-based messages, or medical claims.

## Privacy and Safety Rules

- Do not send user data anywhere.
- Do not ask for sensitive medical information.
- Do not present the app as therapy or mental health treatment.
- Include a short privacy note: “Your entries are saved only in this browser.”
- If adding sample text, keep it supportive but neutral.

## Technical Preferences

- Use vanilla HTML, CSS, and JavaScript unless a framework is absolutely necessary.
- Keep files simple and easy to edit.
- Preferred file structure:
  - `index.html`
  - `styles.css`
  - `script.js`
  - `README.md`

## Definition of Done

The app is done when a user can:

- Open the GitHub Pages site.
- Select a mood.
- Add an optional note.
- Save the entry.
- See previous entries.
- View a simple mood trend chart.
- Delete entries.
- Refresh the page and still see saved data.
