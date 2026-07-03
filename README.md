# JavaScript HW-12 — Image Search Gallery

> Course project — [GoIT Full Stack Web Development](https://goit.global/) program.

🔗 **Live demo:** [tatyanatychynska.github.io/goit-js-hw-12](https://tatyanatychynska.github.io/goit-js-hw-12/)

A simple image search app built with vanilla JavaScript and Vite. Users search for images via the [Pixabay API](https://pixabay.com/api/docs/), view results in a responsive gallery with a lightbox, and load more results in pages.

## Features

- Search images by keyword using the Pixabay API
- Responsive image gallery with lazy-loaded images
- Lightbox preview on click ([SimpleLightbox](https://simplelightbox.com/))
- "Load more" pagination with smooth scroll to the next batch
- Toast notifications for empty queries, no results, errors, and end of results ([iziToast](https://izitoast.marcelodolce.com/))
- Loader indicator while fetching data

## Tech Stack

- [Vite](https://vitejs.dev/) — dev server and bundler
- [Axios](https://axios-http.com/) — HTTP requests to the Pixabay API
- [iziToast](https://izitoast.marcelodolce.com/) — notifications
- [SimpleLightbox](https://simplelightbox.com/) — image lightbox

## Getting Started

Install dependencies:

```bash
npm install
```

Run the dev server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Project Structure

```
src/
├── css/                 # Styles (reset, base, main)
├── img/                 # Static images/icons
├── js/
│   ├── pixabay-api.js   # Pixabay API request logic
│   └── render-functions.js # DOM rendering, loader & button helpers
├── index.html
└── main.js              # App entry point, form & pagination logic
```

## Deployment

Pushes to `main` are automatically built and deployed to GitHub Pages via the workflow in [.github/workflows](.github/workflows).
