# learnwithmeme

**The meme you almost got — in the language you're learning.**

**→ Live demo: [siddarthnyati.github.io/learnwithmeme](https://siddarthnyati.github.io/learnwithmeme)** · **The thinking: [PRD.md](PRD.md)**

A grid of authentic native-language memes — four per language across seven languages, including English, because that's the [Duolingo English Test](https://englishtest.duolingo.com/). Tap a card and it opens big; flip it for the dissection: the translation, why it lands, a cultural note, and the word and grammar bites worth keeping — explained in English or Spanish, whichever you actually speak. The main app builds the habit; this is what the habit is for.

## Why this exists

I'm applying for the Senior PM role on the Duolingo English Test, and I wanted to show up with something more honest than a slide deck. Duolingo is world-class at teaching you the language; this is a sketch of the surface that teaches you the people. The product reasoning — insight, principles, content strategy, anti-features, metrics, rollout, risks — is in the [PRD](PRD.md).

## How it's built

- **One file.** `index.html` — no build step, no framework install, no dependencies beyond two CDN tags (Tailwind, Google Fonts). Clone it, open it, it works.
- **To Duolingo's published design system** ([design.duolingo.com](https://design.duolingo.com)): their palette's exact hex values, their type rules (lowercase headlines in brand color, Nunito body — the substitute font their guidelines bless), their chunky press-down buttons, and their illustration shape language — three rounded shapes, flat perspective, pill shadows, no gray.
- **Original characters.** Every card's scene is hand-built inline SVG starring Memo (the Fox-orange speech-bubble creature) and friends, drawn to Duolingo's construction rules. Duo, Lily, and the real cast stay theirs — trademarked characters don't belong on someone else's portfolio.
- **Small touches:** deep-linkable decks and cards (`#ja-3`), base language and deck persist in `localStorage`, full keyboard support (arrows, space, esc), `prefers-reduced-motion` respected.

## Run it locally

Open `index.html` in a browser. That's the whole setup.

---

Made by **Siddarth Nyati** — applying for Senior PM, DET at Duolingo. Not affiliated with Duolingo (yet). The characters here are original; Duolingo's own cast stays theirs.
