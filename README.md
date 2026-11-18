# Шаг · Mobile Path

Installable, offline-first personal learning planner for English and mobile development, with an interview target of August 2027.

## Run

Serve this folder over HTTP, for example `python3 -m http.server 8765`. Open localhost. PWA installation and service workers require HTTPS or localhost. All paths are relative, so the app supports GitHub Pages project subdirectories.

## Deploy to GitHub Pages

Publish this folder at the root of a public repository. In Settings → Pages, select Deploy from a branch → main → /(root). Wait for the Pages deployment. Open its HTTPS URL in Safari, then Share → Add to Home Screen.

## Features

Two tasks per learning session, a 20-minute option, completion tracking, notes, JSON export/import, mentor report, roadmap and three portfolio project briefs. The first seven sessions are curated. Later sessions use recurring practice themes and need mentor review based on actual progress. Task completion is self-reported.

Data lives in localStorage on one browser/device. Clearing browser data loses it unless exported. The app does not send progress to the mentor chat or sync devices. No authentication, analytics or student data is embedded in the public source.

## Reminders

Settings exports an iCalendar daily reminder in Europe/Minsk. Import into Calendar and verify alerts are enabled. Its recurrence is independent of app completion. Re-importing can duplicate events. Notification permission and a test notification are available in supported installed PWAs. Background Web Push is not connected. A service worker push handler is included for a future sender integration, but no subscription service or background scheduler exists.

## Checks

JavaScript syntax and simulated completion/import/render logic checked. Desktop browser preview checked. iPhone installation, calendar import and actual notification delivery require verification on a phone.
