# Good Girl Hydration Protocol

> Stay thirsty. Stay good.

A completely unnecessary, deeply spicy hydration tracker for people who apparently cannot drink water unless rewarded with praise, badges, voice lines, and escalating approval. Log your water. Earn your "good girl." Restore privileges. Because basic self-care clearly needed a reward system with psychological consequences.

Built for the **AiDHD Hackathon 2026 - "Build A Thing Nobody Asked For."**

## How it works

Drink water, hit milestones, unlock escalating rewards from a possessive AI persona. Skip water and log coffee instead, and your privileges go under review.

**Reward ladder** (unlocks as you fill 8 glasses):

- Glass 1-2: text praise
- Glass 3-4: a badge
- Glass 5-6: a voice line
- Glass 7-8: a visual reward (tap to open fullscreen)

**Daily set.** Each day serves one matched set - the text, voice, badge, and visual all share the same number. Day 1 is set #1, day 2 is set #2, and so on through 14.

**Coffee debt.** Logging coffee costs you a glass and files a violation. Each glass of water you log afterward pays the debt back down.

## Features

- 8-glass tracker with a progress ring and animated feedback
- Four escalating reward tiers: text / badge / voice / visual
- 14 sequential daily sets, each fully matched across all four reward types
- Coffee-debt mechanic with a "violation" panel
- localStorage persistence with real date-based day rollover
- "Walk of shame" recap when yesterday came up short
- Animated splash screen and a progressive mood that warms as you hydrate
- Fullscreen viewer for the visual reward

## Tech

Single static `index.html`. No build step, no backend, no accounts, no live API calls.

- React 18 + Tailwind + Babel-standalone, loaded from CDN
- All rewards pre-generated and served from `assets/`
- State lives entirely in the browser (localStorage)

## Run it

Open `index.html` in a browser, or serve the folder and open the local URL (recommended - `file://` can be fussy with localStorage). To share it, host the folder as a static site (e.g. GitHub Pages) and that URL is your demo link.

## Project structure

```
index.html        the whole app
assets/audio/     voice_1..14.mp3
assets/badges/    badge-1..14.png
assets/visuals/   t3_1..14.png
```

## A note on content

Playfully NSFW - suggestive praise, suggestive art, 18+, and unapologetic about it. There is no safe mode. If that is not your thing, this is not your app.

## Credits

Concept, copy, and chaos by a small constellation of AI collaborators. Voice lines via ElevenLabs. Tagline: "Stay thirsty. Stay good."
