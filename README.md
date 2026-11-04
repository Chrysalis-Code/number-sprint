# Class 2 Learning Quest

A level-based learning game for CBSE Class 2, made for tablets: **Maths, English, Hindi and World Around Us**. Screens are in English, and the voice speaks Tamil. One self-contained `index.html`, no build step.

Every level is mapped to a learning outcome, success criteria and the NCF for Foundational Stage 2022. See [CURRICULUM.md](CURRICULUM.md).

## How it works

1. **Log in** with the password (default `2026`, set by `APP_PASSWORD` in `index.html`).
2. **Pick your player**, or tap **New player** to make one (name + animal).
3. **Choose a subject**, then play: Maths has 8 worlds and each other subject has 4, with 5 levels per world (100 levels in all). Each level is 10 untimed questions. Earn 1–3 stars (7, 9 or 10 right on the first try); one star unlocks the next level. Coins buy stickers.

## Maths worlds

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

## Other subjects

| Subject | Worlds |
|---|---|
| English | Sound Safari (phonics), Word Workshop (words and spelling), Grammar Garden (naming, action and describing words), Story Corner (reading) |
| Hindi | Akshar Mela (letters), Matra Magic (vowel signs), Shabd Bagicha (words), Vakya Ghar (sentences) |
| World Around Us | My Body and Health, Plants and Animals, Family and Community, Our Earth |

## Talking with Kili

Every level is a conversation with Kili the parrot, in five steps that follow the Chrysalis lesson flow: engagement, concept-building, assessment, reflection.

1. **Wonder**: Kili tells the world's story and today's learning goal ("I can…"), then asks "Ready?"
2. **Think together**: Kili solves one example out loud, using the level's strategy.
3. **Play**: 10 questions. Kili reads each one, then **listens automatically**. The child can say the answer, "repeat", "help" or "I don't know", or tap. Now and then Kili asks "How did you work that out?"
4. **Brain buster**: an optional harder bonus question.
5. **Teach Kili**: the child explains what they learned, then rates the level Easy, OK or Tricky.

**Voice language.** Each child chooses Tamil, Hindi or English, and can change it in the parent settings. English and Hindi words inside a sentence are spoken in their own voices. The child-like style raises the pitch of the tablet's Indian voice. The quality depends on the voices installed. On Android, install the Tamil and Hindi voices under Settings › Text-to-speech › Google › Install voice data.

**Microphone.** Listening works in Chrome on Android and in Safari on iPad when the game is opened from GitHub Pages. The Claude artifact viewer blocks the microphone, so there the child taps instead.

## Parent dashboard

Tap **Parents** and answer a times-table question. Shows today's time, questions and accuracy, a 14-day chart, a practice calendar, skill status for every level, tricky questions, a daily log, and per-child settings, and a way to delete a child's profile.

## Saving progress

- Opened as a Claude artifact, progress is saved to the owner's Claude account.
- Opened anywhere else (GitHub Pages, a local file), progress is saved in that browser only.

The password is a simple front door for children, not real security: anyone who reads the page source can see it.
