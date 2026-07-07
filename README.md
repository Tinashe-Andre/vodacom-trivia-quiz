# Vodacom Early Careers — 30-Sec Trivia Quiz

A single-page trivia game built with HTML, Bootstrap (CDN), and vanilla JS.
No build step, no dependencies to install — it's just one HTML file.

## Folder guide

- `index.html` — the whole app: markup, styles, and game logic in one file.
  It's named `index.html` and sits at the root on purpose, so Vercel (or
  any static host) serves it automatically with zero configuration.
- `01_Planning/trivia-questions-brief.pdf` — the original brief with the
  15 questions and answers this game is built from.

As the project grows, feel free to add the rest of the usual folders
(`03_Docs`, `04_Tests`, `06_Archive`, etc.) using the `new-coding-project.bat`
template script — just don't move `index.html` out of the root, or the
zero-config Vercel deploy will stop finding it.

## Running it locally

Just double-click `index.html` — it opens directly in your browser, no
server needed.

## What it does

- Login screen: quick guest sign-in (name + email) or a real
  username/password account (stored in the browser for now — see the
  `AuthAPI` comments in `index.html` for the swap-in point for a real
  backend later).
- 5 randomised questions per round, pulled from a bank of 15, with a
  30-second timer.
- Tracks which questions each logged-in user has already seen, so
  repeat plays cycle through fresh questions instead of repeating.
- Win screen / "Sorry, try again" screen, both with Share and Register
  buttons linking to the Vodacom Early Careers registration page.

## Deployment

This repo is set up to deploy on Vercel with zero configuration —
just import the repo at vercel.com and it will find `index.html`
automatically.
