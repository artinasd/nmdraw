# NurMedia Lottery

A dependency-free Persian/RTL lottery page for NurMedia.

## Design

- All **207 unique usernames** are rendered simultaneously.
- The supplied source list contained 208 rows because `samira202935` appeared twice; the exact duplicate is removed so each attendee has one entry.
- The draw uses the browser's **Web Crypto API** (`crypto.getRandomValues`) and an unbiased Fisher–Yates shuffle.
- The animation only visualizes the already randomized elimination order; it does not use CSS animation randomness to choose the winner.
- No network request or server is needed after the page loads.

## Run

Open `index.html` directly, or serve the folder with any static HTTP server.

## Files

- `index.html` — RTL Persian/Kurdish UI
- `style.css` — responsive visual design
- `script.js` — participant data, secure shuffle and draw animation
