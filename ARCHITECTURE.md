# ARCHITECTURE.md

## App Overview

This project is a browser-based **Mood Tracker** hosted on GitHub Pages. It is a static web app built with HTML, CSS, and JavaScript. The app does not use a backend server, external database, login system, or paid API. All user mood entries are stored locally in the browser using `localStorage`.

## Primary User Flow

1. The user opens the app.
2. The user selects a mood from a small set of mood options.
3. The user may add an optional short note.
4. The user saves the entry.
5. The entry appears in the mood history list.
6. The chart updates to show the new mood trend.
7. The user can delete an entry if needed.

## File Structure

```text
/
├── index.html
├── styles.css
├── script.js
└── README.md
```

## `index.html`

The HTML file defines the page structure. It should include:

- App title and short description.
- Privacy note explaining that entries stay in the browser.
- Mood entry form.
- Mood option buttons or radio inputs.
- Optional note field.
- Save button.
- Mood trend chart area.
- Mood history section.

## `styles.css`

The CSS file controls the visual design. It should include:

- A calm color palette.
- Responsive layout for mobile and desktop.
- Clear spacing and readable typography.
- Accessible contrast for text and buttons.
- Visual distinction for selected mood options.

## `script.js`

The JavaScript file controls app behavior. It should include:

- Mood option data.
- Save entry function.
- Load entries from `localStorage`.
- Render mood history.
- Delete entry function.
- Update mood trend chart.
- Basic form validation.

## Data Model

Each mood entry should be stored as an object:

```json
{
  "id": "unique-id",
  "date": "YYYY-MM-DD",
  "mood": "Good",
  "score": 4,
  "note": "Optional user note"
}
```

Mood scores can be used for charting:

```json
{
  "Great": 5,
  "Good": 4,
  "Okay": 3,
  "Tired": 2,
  "Sad": 1,
  "Stressed": 1
}
```

## Storage

Use `localStorage` with a key such as:

```text
moodTrackerEntries
```

The app should:

- Save entries as a JSON string.
- Parse entries when the page loads.
- Handle missing or corrupted data safely.
- Never send entries to an external service.

## Chart Approach

Use a simple chart that can work without external dependencies. A basic SVG, canvas, or styled HTML bar chart is acceptable. The chart should show recent entries in chronological order and make mood changes easy to understand.

## Privacy and Safety

The app is for personal reflection only. It should not claim to diagnose, treat, or provide medical advice. The app should include a visible privacy statement explaining that data is stored only in the current browser. Users should understand that clearing browser data may delete their entries.

## Accessibility

The app should support:

- Keyboard navigation.
- Clear labels for form fields.
- Sufficient color contrast.
- Text descriptions in addition to icons.
- Responsive design for smaller screens.

## Future Improvements

Possible future features include:

- Export entries as a JSON or CSV file.
- Filter entries by date range.
- Add custom moods.
- Add reminders without requiring a user account.
- Add an optional reflection prompt after saving a mood.
