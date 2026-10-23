<p align="center">
  <img src="logo.svg" alt="Arabic Alphabet logo" width="140">
</p>

# Arabic Alphabet الأبجدية

A single-page site for learning the Arabic alphabet and your first phrases, with audio for every letter and phrase.

No build step, no dependencies, no backend. Just one `index.html`.

## Features

- **All 28 letters + hamza**
  - Every letter shows its start, middle and end forms, its name, and its Latin spelling and IPA.
  - Each letter has a **Name** button and a **Sound** button that plays it with a, i and u.
- **How to say it**
  - Every letter is compared to sounds you already know in English, German, Japanese and Russian.
  - The 10 letters with no real equivalent are tagged *new sound* and come with a tip on how to make them.
- **50 starter phrases**
  - Greetings, polite words, small talk, help while learning, and everyday expressions.
  - Each phrase is written in Modern Standard Arabic with full vowel marks, and has a play button.
  - Where a phrase changes when you talk to a woman, a note shows that form.
- **Voice picker**
  - Choose from every Arabic voice installed on your device, for example Saudi or Egyptian.
  - The page remembers your choice.
- **Slow mode** plays the audio at reduced speed for careful listening.
- **Mobile / PC switch**
  - Mobile shows letters and phrases as cards, and PC shows them as a full table.
  - On first visit the layout is picked from your screen width, and after that the page remembers your choice.
- **Light and dark mode** follow your system setting.

## Usage

Open `index.html` in any modern browser. That's it.

To host it, enable **GitHub Pages** in the repo settings (Settings → Pages → deploy from branch `main`, folder `/`).

## Audio

Audio uses the browser's built-in [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis) with your device's Arabic text-to-speech voices. No audio files are shipped.

Quality depends on the voices installed on your device. Mac and iPhone usually sound best. If the voice list is short or empty, add Arabic voices:

| System  | Where |
|---------|-------|
| macOS   | System Settings → Accessibility → Spoken Content → System voice → Manage Voices → Arabic |
| iOS     | Settings → Accessibility → Spoken Content → Voices → Arabic |
| Windows | Settings → Time & language → Speech → Add voices → Arabic |
| Android | Settings → Text-to-speech → Speech Services by Google → Install voice data → Arabic |

Reload the page after installing.

## Tech

- Plain HTML, CSS and vanilla JavaScript in one file
- Fonts: [Amiri](https://fonts.google.com/specimen/Amiri) for Arabic, IBM Plex Sans / Mono for everything else (Google Fonts)
- `localStorage` stores only your layout and voice choice

## Logo

`logo.svg` is an eight-pointed star (khatam), a classic motif in Islamic geometric art. In its centre is the letter ع (ʿayn), the most typical sound of Arabic. The letter is drawn from the Amiri font (SIL Open Font License).

## Roadmap ideas

- Quiz mode for letters and phrases
- Recorded native-speaker audio
- Dialect versions of the phrases (Egyptian, Levantine)
