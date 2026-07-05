# Shop Attendance Tracker

A single-file web app to track employee attendance for a small shop (< 10 employees).

## Features

- Employees clock in/out by tapping their name; a photo is captured via the device camera as proof.
- Daily hours are calculated automatically (supports overnight shifts and fixing missed punches).
- Records view per day with in/out photos, editable times.
- Monthly report: hours per day per employee, days worked, total hours — downloadable as Excel (.xlsx).

## Usage

Open the hosted page (GitHub Pages) on the tablet/phone at the shop entry and allow camera access. Add employees in the **Employees** tab, then use the main screen to clock in/out.

## Data storage

All data (records in localStorage, photos in IndexedDB) is stored **locally in the browser of the device** — there is no server database. Use the same device and browser consistently, and don't clear site data. Export the monthly Excel regularly as a backup.

## Tech

Plain HTML/CSS/JS, no build step. [SheetJS](https://sheetjs.com/) via CDN for Excel export (falls back to CSV when offline).
