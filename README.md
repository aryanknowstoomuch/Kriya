# To-Do List (Vanilla JS)

A simple, responsive to-do list web app built with plain HTML, CSS, and JavaScript. Tasks can be added, checked off, removed, and are automatically saved to your browser's localStorage.

## Features
- Add new tasks
- Toggle completion state (checked/unchecked)
- Remove tasks
- Persistent storage using localStorage
- Responsive UI with clean styling

## Project Structure
```
project/
  html/
    index.html
  css/
    style.css
  js/
    scrpit.js
  To-Do-Img/
    images/
      checked.png
      unchecked.png
      icon.png
```

Note: The JavaScript file is intentionally named `scrpit.js` to match the reference in `index.html`.

## Getting Started
1. Clone or download this repository.
2. Open `html/index.html` directly in your browser.

No build step or server is required.

## How It Works
- The UI is rendered by `html/index.html` and styled with `css/style.css`.
- Core logic in `js/scrpit.js`:
  - `AddTask()` creates list items and a delete `×` button
  - Click on a list item toggles `checked` state
  - Click on `×` removes the item
  - `saveData()` serializes the list into `localStorage`
  - `showTask()` restores the list from `localStorage` on load

## Assets
Icons are loaded from `To-Do-Img/images/` and referenced in CSS for checked/unchecked states and in HTML for the header icon.

## Browser Support
Works on modern browsers. localStorage is required for persistence.

## License
MIT
