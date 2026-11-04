# Class 2 Math Quest

A level-based maths game for CBSE Class 2, made for tablets. One self-contained `index.html`, no build step.

## How it works

1. **Log in** with the password (default `1234`, set by `APP_PASSWORD` in `index.html`).
2. **Pick your player**, or tap **New player** to make one (name + animal).
3. **Play**: 8 worlds × 5 levels, 10 untimed questions each. Earn 1–3 stars (7, 9 or 10 right on the first try); one star unlocks the next level. Coins buy stickers.

## Worlds

| # | World | Topics |
|---|---|---|
| 1 | Number Garden | Counting, before/after, number names, comparing, skip counting |
| 2 | Place Value Fort | Tens and ones, expanded form, value of a digit |
| 3 | Addition Beach | Within 10 and 20, two-digit addition with and without carrying |
| 4 | Subtraction Cave | Within 10 and 20, two-digit subtraction with and without borrowing |
| 5 | Rupee Market | Coins and notes, counting money, shopping, change |
| 6 | Clock Tower | O'clock, half past, days of the week, months |
| 7 | Shape Park | Shapes, sides and corners, patterns, measuring in cm, odd and even |
| 8 | Times Table Jungle | Equal groups, tables of 2–5 and 10, sharing, word problems |

## Voice

- **Read aloud**: questions, answer choices, hints and praise are spoken (Web Speech API).
- **Say your answer**: tap the microphone and say the answer ("forty-seven", "half past four", "greater than"). Works in Chrome and Safari when the page is served over HTTPS, for example GitHub Pages.

## Parent dashboard

Tap **Parents** and answer a times-table question. Shows today's time, questions and accuracy, a 14-day chart, a practice calendar, skill status for every level, tricky questions, a daily log, and per-child settings.

## Saving progress

- Opened as a Claude artifact, progress is saved to the owner's Claude account.
- Opened anywhere else (GitHub Pages, a local file), progress is saved in that browser only.

The password is a simple front door for children, not real security: anyone who reads the page source can see it.
