# Focus Sprint

A single-file mini web app for **MLH Global Hack Week — Challenge 1**: task tracking plus a 25-minute Pomodoro-style focus timer. No build step, no dependencies, no network calls.

## Open the app

1. Open this folder in Finder (or your file manager).
2. Double-click **`index.html`**, or drag it into Chrome, Firefox, Safari, or Edge.

Alternatively, from a terminal in this folder:

```bash
open index.html
```

## Features

- Add tasks, mark complete, delete individual tasks
- Completed / total count
- Tasks saved in `localStorage` (survives refresh)
- 25:00 focus timer with Start, Pause, and Reset
- Keyboard: **Alt+S** toggles Start/Pause, **Alt+R** resets the timer

## Files

- `index.html` — HTML, CSS, and JavaScript in one file
- `verification.json` — results and scope of the functional checks

## Built with Cursor

Cursor Desktop, using Composer 2.5 Fast, generated the initial single-file app and README from a prompt describing task management, local persistence, accessibility, and a 25-minute focus timer. Cursor helped turn the feature list into a working implementation without a build system or external services.

## Verification

Nine DOM behavior checks passed in jsdom, covering task validation, safe text rendering, completion counts, persistence, deletion, and timer start/pause/reset/completion. Timer checks used a fake clock; these results do not represent a rendered browser or visual test. See `verification.json` for the complete checklist.
