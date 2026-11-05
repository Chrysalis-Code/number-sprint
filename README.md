# Class 2 Learning Quest

A level-based learning game for CBSE Class 2, made for tablets and phones: **Maths, English, Hindi, Tamil and World Around Us**. Maths, English and World Around Us are in English (screen and voice); Tamil lessons are fully in Tamil and Hindi lessons fully in Hindi. One self-contained `index.html`, no build step.

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
| Tamil (Samacheer Kalvi Class 2 topics) | உயிர் எழுத்து உலா (vowels, குறில்–நெடில்), மெய் எழுத்து மாலை (consonants, வல்லினம்/மெல்லினம்/இடையினம்), சொல் தோட்டம் (உயிர்மெய், words, எதிர்ச்சொல், ஒருமை–பன்மை), கதை வீடு (sentences, colours and days, ஆத்திசூடி, stories) |
| World Around Us | My Body and Health, Plants and Animals, Family and Community, Our Earth |

## Ways to answer (no typing)

Tap an answer, say it out loud, or do one of the hands-on activities. 6 of every level's 10 rounds are hands-on, and most levels use 5 or 6 different kinds:

- **Match the following**: tap or drag a line between pairs
- **Sort into boxes**: drag or tap cards into bins (wet or dry waste, odd or even, pet, farm or wild)
- **Put in order**: tap in sequence (days, months, counting, building a sentence)
- **Circle it**: draw a ring around the right picture with a finger
- **Trace it**: trace big letters and numbers (அ, क, b, 7)
- **Number line**: drag the frog to the right number
- **Tap to count**: tap the right number of pictures (or share them equally)
- **Build the word**: tap letter or syllable tiles in order (cat, गाय, மரம்), including a few tiles that don't belong; also number parts and shape patterns
- **Drag into the blank**: drag the right answer into the box in the sentence or sum
- **Find in the picture**: tap every matching thing in a scene (good habits, wild animals, every “க்”)
- **Thumbs up or down**: "Is it 9?" Yes or No
- **Pop the balloon**: tap the floating balloon with the right answer
- **Memory cards**: flip two cards at a time to find the pairs
- **Pay with coins**: tap or drag coins and notes into the purse to pay a price or give change

**Works in any orientation.** On a phone turned sideways, Kili sits on the left and the question on the right, so each question fits on one screen. Checked in Chrome on phone and tablet sizes, portrait and landscape.

**Listening questions** ("Listen. Which letter do you hear?") never show the letter or word on screen or in Kili's speech bubble. A big speaker button plays just that sound again.

## Talking with Kili

Every level is a conversation with Kili the parrot, in five steps that follow the Chrysalis lesson flow: engagement, concept-building, assessment, reflection.

1. **Wonder**: Kili tells the world's story and today's learning goal ("I can…"), then asks "Ready?"
2. **Think together**: Kili solves one example out loud, using the level's strategy.
3. **Play**: 10 questions, taking turns. Kili reads the question and the answers, then says "Your turn" and **waits, listening**, for as long as the child needs. After the answer Kili gives feedback, and only then moves to the next question. The child can say the answer, "repeat", "help" or "I don't know", or tap. Now and then Kili asks "How did you work that out?"
4. **Brain buster**: an optional harder bonus question.
5. **Teach Kili**: the child explains what they learned, then rates the level Easy, OK or Tricky.

**Language.** There is no language to choose. Maths, English and World Around Us are shown and spoken in English, in an Indian English (en-IN) voice at a calm speed. Inside a Tamil lesson everything is Tamil: questions, buttons, hints and Kili's voice. Inside a Hindi lesson everything is Hindi. The speaker button at the top right turns Kili's voice on or off.

**Natural Tamil and Hindi voices, built in.** Tamil and Hindi are spoken by a neural speech engine that runs inside the browser ([Piper](https://github.com/rhasspy/piper) voices *ta_IN-HemaLatha* and *hi_IN-priyamvada*, using onnxruntime-web). Every sentence is spoken whole, numbers included, and nothing is installed on the tablet. The first time a Tamil or Hindi lesson opens, the device downloads the engine and that voice: about 80 MB, with a progress screen. After that it works without internet. The engine runs in a background worker so the screen never freezes, and it makes the next sentence while the current one plays. If the download isn't possible, Kili uses the tablet's own voice.

**Animated Kili.** Kili is a drawn, animated parrot: she blinks, nods while talking, tilts her head while listening, and flaps her wings for right answers. Her beak moves with the loudness of the recorded voice (lip-sync), or with word timing for the tablet's voice.

**Microphone.** Listening works in Chrome on Android and in Safari on iPad when the game is opened from GitHub Pages. The Claude artifact viewer blocks the microphone, so there the child taps instead.

## Learning path and lessons

Inspired by Duolingo: each subject is a winding path of round level circles grouped into worlds. The next lesson pulses with a START label, finished levels show their stars, and a crown marks 3 stars. During a lesson a progress bar fills at the top, with a 🔥 counter for answers right in a row. After each answer a green or red panel slides up ("You got it!" or "Correct answer: 53") with a Continue button. Kili also moves on by herself when she finishes talking. A finished lesson shows coins, accuracy and time, and a day-streak celebration.

## Classwork (assign levels)

Inspired by Google Classroom: in the parent area, **Classwork** lets you pick a subject, a level and a due date, then tap **Assign**. The child sees it at the top of the map ("📋 From your parent", with a Start button), and the level is marked on the path. When the child finishes it, Classwork shows it as **Done** with the score and stars. Work not done by the due date shows as **Missing**.

## Parent dashboard

Tap **Parents** and answer a times-table question. Shows today's time, questions and accuracy, a 14-day chart, a practice calendar, skill status for every level, tricky questions, a daily log, and per-child settings, and a way to edit or delete a child's profile.

## Saving progress

- Opened as a Claude artifact, progress is saved to the owner's Claude account.
- Opened anywhere else (GitHub Pages, a local file), progress is saved in that browser only.

The password is a simple front door for children, not real security: anyone who reads the page source can see it.

## Versions

The version number shows at the top left. On GitHub Pages the game checks `version.json` and reloads itself to the newest version between levels, so no hard refresh is needed.
