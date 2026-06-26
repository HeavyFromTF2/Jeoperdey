# Advanced Jeopardy Clone

A fully interactive, client-side Jeopardy quiz game designed for pub trivia, classrooms, or team-building events. It supports dynamic grid layouts, real-time score tracking, responsive modals, and complete local customization without requiring a database.

---

## Features

* **7-Category Grid Layout:** Features a full-screen board layout (`7 columns × 5 rows`) engineered for rich styling and high-contrast text.
* **Dual Operating Modes:** 
  * **Play Mode:** Click cells to trigger fullscreen question animations and handle team scoring.
  * **Edit Mode:** Click headers or cells directly on the board to customize category names, values, questions, or answers on the fly.
* **Media Support:** Handles standard image/video URLs, YouTube videos (and Shorts), or direct **local file uploads** parsed as Base64.
* **Dynamic Scoreboard:** Add, remove, or rename unlimited teams. Adjust scores manually via inputs or utilize quick-click `+/-` buttons inside the question view.
* **Zero-Server Persistence:** Keeps your entire game configurations and current scores intact using browser `localStorage`.
* **Portability:** Export your entire board configuration into a single `.json` file or import a saved backup seamlessly.

---

## Keyboard Shortcuts

When a question modal is active, you can use these shortcuts to speed up gameplay:

| Key | Action |
| :--- | :--- |
| **`SPACEBAR`** | Reveals the hidden answer / Closes modal if already revealed |
| **`ESCAPE (ESC)`** | Closes/exits the active question or settings modal |

---

## Quick Start & Clear State

### Running the App
Since the application runs entirely in the browser, simply double-click the `index.html` file to play. 

### Resetting Cache
Because the app relies heavily on `localStorage` to save your changes, old cached versions might sometimes conflict. If you need to wipe out previous settings and revert to default templates, open your browser's Developer Tools (**F12**), navigate to the **Console** tab, run:

```javascript
localStorage.clear();
