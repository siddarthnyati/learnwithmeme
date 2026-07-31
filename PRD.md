# LearnWithMeMe — PRD

**Author:** Siddarth Nyati · **Status:** Working prototype, live at [siddarthnyati.github.io/learnwithmeme](https://siddarthnyati.github.io/learnwithmeme)

## One-line pitch

The meme you almost got — flip the card, and a bilingual friend explains why it's funny in the language you're learning.

## The insight

Duolingo's core product is world-class at skill acquisition — repetition, spacing, streaks, and a tone nobody else can copy made it the default way humans start a language. That machine works; nothing here touches it.

But there's a moment the machine doesn't reach: everyone in the group chat laughs at something in your target language — you got every word and still missed the joke. Vocabulary wasn't the problem; culture was. Jokes are the densest artifacts a language produces: register, history, and social norms compressed into one line.

Memes are the modern unit of that compression, and nobody is teaching them. The gap between "I can order coffee" and "I laughed before the translation loaded" is where a learner stops feeling like a visitor. That's the gap this product sits in.

## The user

Maya, 29, is four years into French. She's past every app's core content, watches French YouTube on 1x speed, and can hold a conversation — but in her French group chat she still googles jokes and laughs thirty seconds late. She doesn't need another lesson. She needs the shared references that mark someone as *in*. Not a beginner, not fluent: the intermediate learner whose remaining distance to the culture is no longer measured in vocabulary.

## Job-to-be-done

> When I have five minutes, I want to feel more culturally fluent in the language I'm learning, without another streak to maintain.

## The product

A grid of memes per language — four each, seven languages including English. Tap one and it opens big; tap again and it flips. Nothing else.

### The front

An authentic native-language meme, presented the way a native speaker would meet it: original script, no translation, no hand-holding — plus an illustrated character scene, because what makes a meme land is the picture, not just the caption. For non-Latin scripts, a small romanized reading sits underneath; on the browse grid, a one-line translation sits under every card so no script locks you out. The front is deliberately a little uncomfortable. That almost-got-it itch is the hook.

### The back

The dissection, in a fixed order: the translation, why it lands, a cultural note, word bites (the individual pieces worth keeping), and a grammar bite — or an alphabet bite for non-Latin scripts. The voice is a bilingual friend leaning over your shoulder, never a textbook and never a joke-explainer uncle. If the back reads like homework, it has failed.

### The base language

Dissections shouldn't assume English. An "I speak" picker sets the explanation language — English and Spanish are live in the prototype — and the deck list adapts: no Spanish-to-Spanish, and for a Spanish speaker, English itself becomes a learnable deck. That last detail is the DET in miniature: the world's largest population of learners is learning English, in their own language.

## Product principles

1. **Non-intrusive.** No nag mechanics of any kind. The product is confident enough to let you leave.
2. **Culturally respectful.** The joke punches at the language quirk or the shared human moment — never at the culture as a punchline.
3. **Warm, not preachy.** Explain the joke without embalming it. One cultural note, not a lecture.
4. **Delight-first, not completion-first.** Success is a laugh and one word remembered, not a finished unit.

## Design language

The visual system is built from a close read of Duolingo's published brand guidelines (design.duolingo.com), and it speaks them with an accent you'd have to squint to hear:

- **Their palette, fully.** Feather Green primary with full-bleed color blocks the way their marketing pages use them, Macaw, Bee, Fox and Cardinal accents, Eel text, their exact neutrals — the published hex values, not approximations.
- **Their type rules.** Headlines short, lowercase, in brand color, never neutral; body set in Nunito — the substitute font Duolingo's own guidelines bless.
- **Their illustration system.** Three rounded shapes, flat perspective, pill shadows, floating hands, no gray, fewest shapes possible — followed literally, and lightly animated, because memes are physical comedy.
- **Their controls.** Chunky buttons with a hard bottom edge that physically press down.
- **One deliberate line:** the characters are original. Memo — a Fox-orange speech-bubble creature — and his Macaw-blue friend are drawn to Duolingo's construction rules, but Duo, Lily and the cast stay theirs. Shipping someone else's trademarked characters on a public portfolio URL is the one flourish a hiring manager could only hold against me.

## Content strategy

Every meme is sourced by a native curator for that language — someone who lives in the meme culture, not someone who studied it. The pipeline: curator proposes → originality check (text-form only, no lifted image macros) → translation and dissection drafted by the curator, edited for voice consistency → safety review by a second native speaker for stereotype risk and audience readings the curator may not carry → publish. Dissections are written per base language by curators who share it — a Spanish speaker's explanation of an English meme is authored in Spanish, not machine-translated into it.

Authentic voice matters more than volume: better six great memes than sixty average ones — one phrasebook-energy meme costs more credibility than an empty slot. Decks refresh at a cadence curators can sustain honestly, not one a content calendar demands.

## Anti-features

Deliberate departures from the core app's mechanics, each with a reason:

- **No streaks.** The streak is the right tool for habit-building in skill acquisition. Cultural curiosity dies under obligation.
- **No XP or leaderboards.** There is no "winning" at getting a joke. Competition would bend content toward what's countable.
- **No notifications.** A product about belonging cannot nag. The meme is the retention mechanic or there isn't one.
- **No sign-in.** Nothing here needs an identity. Friction-free is the point of a five-minute surface.
- **No progress dashboard.** Measuring "memes learned" would turn a laugh into a chore log.

The bet: for this job, pull beats push. If that bet is wrong, the metrics below will say so quickly.

## Metrics that would matter

All numeric targets are illustrative, not commitments — this is a prototype, not an instrumented product.

- **Engagement per visit:** memes flipped per session (illustrative: ≥3) and time on the card back — did they read the dissection or bounce off it?
- **Share rate:** share-to-flip ratio (illustrative: ≥5%). A shared joke is performed membership — the product's promise, enacted.
- **Return rate:** 30-day return-visit rate *without any prompting* (illustrative: ≥25%). This is the honest test of the no-notifications bet, and the number I'd watch first.

## Rollout

- **Phase 1 — prove the surface.** Web. Seven languages including English, four memes each, dissections in English and Spanish (this prototype). Embed inside the Duolingo app as a "Culture" surface reached from the language home. Measure the three metrics above.
- **Phase 2 — prove the pipeline.** Twenty languages, three to five memes per language per week, each with a paid native curator — and base-language coverage expanding with the same curator network. The hard problem here is editorial operations, not engineering.
- **Phase 3 — open the door.** User-submitted memes with human moderation by the curator network. Community sourcing solves freshness; it also concentrates every risk below, which is why it's last.

## Risks

- **Cultural insensitivity** — the big one. A meme that reads as affectionate self-deprecation inside a culture can read as mockery from outside it. Mitigation is structural, not aspirational: native curators with real veto power, a second-native-speaker safety review distinct from the curator, an in-product "this reads wrong" feedback loop, and a standing rule that any single flag from a native speaker pauses the card pending review.
- **Meme staleness.** A dead meme is worse than no meme — it teaches yesterday's culture. Mitigation: curator-set expiry dates on trend-dependent cards; evergreen language-quirk memes (the majority of this seed set) age far more slowly.
- **Tone drift at scale.** Twenty languages and dozens of curators will pull the voice apart. Mitigation: a written voice bible with worked examples per language, and one editorial owner who reads everything.
- **Copyright.** Meme culture is soaked in copyrighted image macros. Mitigation: text-form memes only as a hard rule, originality check in the pipeline, and emoji-plus-typography for visual flavor.

## Why this fits Duolingo

Duolingo owns the emotional brand of language learning — the only company whose product people have feelings about. But the deepest thing a learner wants isn't a skill certificate; it's the moment a culture treats them as one of its own. This is the surface that serves that moment directly, and it extends the brand from "the app that taught me Spanish" to "the app that made me feel Mexican for a second."

It would also only work at Duolingo. The entire product is tone, sustained across languages at scale — precisely the muscle Duolingo spent a decade building and the one competitors can't copy. In most companies this product would die of committee-approved joke explanations. Here it wouldn't.

## Why me

- I've shipped consumer product experiences end-to-end at ResMed — subscription and bundling work where the job was making a considered purchase feel simple, which is mostly the craft of deciding what *not* to put on the screen. Same craft as this product's anti-feature list.
- I'm the user. I've been a lifelong learner across languages — including proving English proficiency in 2019 to get to Dartmouth — so I know firsthand that the distance between "certified proficient" and "gets the jokes" is real, and that closing it is what belonging feels like.
- Product taste, demonstrated rather than claimed: I built this prototype end-to-end — PRD, content, design, and working code — because a meme deck felt more true to Duolingo's DNA than any dashboard I could have mocked up instead.
