# Smart Academic Task and Management System

A frontend-only academic workspace written in HTML, CSS and JavaScript. Open `dist/index.html` directly, or serve `dist/` with a static web server. No installation or backend is required. Inter is loaded from Google Fonts with a system-font fallback.

## Use

Start on the guest splash page. Create an account for an empty workspace, or choose **Explore the demo** for editable sample records. Add subjects before creating related tasks or examinations. Quick create supports tasks, events and study sessions.

All local accounts and per-account records use browser localStorage. Passwords use salted SHA-256 for this frontend demonstration; client-side checks are not a server security boundary. Data is not synced, emailed, or backed up remotely. A session expires after 24 hours. Password change requires the current password; email recovery is explicitly unavailable.

Focus mode has a live timer with start, pause, resume, break and end controls. End and save to preserve the session. An unsaved session is lost on page reload. Users explicitly set related task progress when saving. In-app reminders work while the app is open; there are no operating-system push notifications.

Analytics supports real CSV downloads and the browser print dialog. Feedback saves locally and is not sent anywhere. AI functionality is outside this build.

## Structure

- `dist/index.html`: entry point
- `dist/style.css`: responsive layouts, tokens and themes
- `dist/app.js`: routes, forms, local data and workflows
- `dist/IMPLEMENTATION.md`: implementation and verification tracker
- `tests/workflows.cjs`: dependency-free runtime tests (`node tests/workflows.cjs`)

The application is built from the supplied written requirements, not inspected Figma content. Figma access was denied. The earlier complete 15-module feature list was not available in full in this session; coverage is mapped to the requirements visible in the current conversation.
