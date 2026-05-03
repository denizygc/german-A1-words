# German A1 Vocab Quiz

A progressive web app for practicing German A1 vocabulary, articles, listening, and picture recognition.

## Features

- **1129 quiz entries** - 756 vocab + 373 artikel
- **Listening mode** - hear the German word and choose the English meaning
- **Picture to German mode** - see a picture and choose the German word
- **Automatic pronunciation** - answers are spoken with browser text-to-speech
- **Answer reveal** - correct picture answers show German; wrong picture answers show German + English
- **Artikel practice** - choose the correct article (der/die/das) for nouns
- **Speed control** - toggle between slow and normal playback
- **Question count** - choose 10, 25, or 50 questions
- **Word Pool** - browse words with picture thumbnails where available
- **Add words** - add your own vocab or artikel questions directly in the app
- **Persistent storage** - custom words are saved in localStorage
- **Works offline** - PWA with service worker caching
- **iPhone ready** - add to Home Screen for a native app experience

## Modes

### Listening

Hear the German word, choose the English meaning, then reveal the written German word.

### Picture

See only the picture, choose the German word. If the answer is wrong, the app pronounces and reveals the correct answer.

## Word Categories

Months, Numbers, Clothing & Colors, Common Adverbs, Verbs, Nouns, Adjectives, Prepositions, Pronouns, Conjunctions, Interjections, and more.

## Quick Start

```bash
python3 -m http.server 8080
```

Open http://localhost:8080 in your browser.

If an old version appears, hard refresh with Cmd + Shift + R or clear site data for localhost.

## Install on iPhone

1. Open the hosted URL in **Safari**
2. Tap **Share** (box with arrow)
3. Tap **Add to Home Screen**
4. It launches full-screen like a native app

## Deploy

Host the entire folder on any static hosting:

- **GitHub Pages** - push to a repo, enable Pages
- **Netlify** - drag and drop the folder
- **Vercel** - connect the repo

## Project Structure

```
├── index.html             # Single-page app
├── A1_Studied_Words.txt   # Source word list
├── a1-word-list.js        # Generated A1 word data
├── picture-map.js         # Generated SVG picture map
├── manifest.json          # PWA manifest
├── sw.js                  # Service worker for offline support
├── icon-192.png           # App icon 192x192
├── icon-512.png           # App icon 512x512
├── .gitignore
├── LICENSE
└── README.md
```

## Data Source

Vocabulary is compiled from the Goethe-Zertifikat A1 word list. Picture SVGs are extracted into `picture-map.js`; raw picture HTML exports are ignored by git.
