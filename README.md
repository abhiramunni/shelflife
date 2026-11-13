# ShelfLife — Your Reading Life, Shelved Beautifully

A single-file reading tracker that looks like a real bookshelf. Track what you're reading, log pages in seconds, keep a reading streak alive, set a yearly goal, save quotes you love — all on your device, no account, no server.

Live: **https://abhiramunni.github.io/shelflife/**

## What it does

- **The shelf** — every book is a wooden book spine. Tap any spine to open that book: update pages with a slider, give it a star rating, mark it finished, or remove it.
- **Now reading** — your current book with a progress bar and one-tap page logging. Logging pages updates your streak, your week chart and the book's progress at once.
- **Reading streak & stats** — books finished, pages logged, current day-streak, average rating.
- **2026 reading goal** — a progress ring (default 12 books, editable) that fills as you finish books.
- **Your week in pages** — a 7-day bar chart of pages logged each day.
- **Reading timer** — a quiet 25-minute session timer; when it ends, it points you at the page log.
- **Booker Prize 2026 shelf** — the 2026 winner *The End of Everything* by M. John Harrison (announced this week, the oldest winner in the prize's history) plus four past winners worth reading. One tap adds any of them to your shelf.
- **Quote shelf** — save lines you love, with the author, and delete any you outgrow.
- **Add a book** — title, author, total pages, genre and status; everything persists in `localStorage`.
- **Copy summary, remove samples, erase everything** — your data stays in your browser.

## Seeded with

Six starter books (Atomic Habits, The Alchemist, Sapiens, Ikigai, The End of Everything, Wings of Fire), a week of sample page sessions, and three classic reading quotes. Use "Remove sample books" to start from a clean shelf.

## Design

Warm editorial palette (ivory paper, espresso ink, bronze/amber/gold/terracotta), Fraunces + Inter, cinematic intro animation with tap-to-skip (quick on return visits), slow Ken Burns drift on two AI-generated warm editorial photos, and a 3-step onboarding coach.

## Tech

- One self-contained `index.html` — no backend, no build step, `localStorage` only.
- Two AI-generated photos embedded as base64 JPEGs.
- QA: 54/54 headless jsdom assertions pass, `node --check` clean, zero uncaught JS errors, no pictographic emoji.
