# Pujo 2026 Scroll

A scroll-driven piece about one Durga Pujo, from Mahalaya to Doshomi, told through the author's own steps, phone unlocks, sleep and street recordings. Made for portfolio submission. Best on desktop, with headphones.

## How to read it

| Mark on screen | What it stands for |
| --- | --- |
| Footprints | One footprint for every 100 steps walked that day |
| Ribbon | Wider with more steps; finer teeth with more phone unlocks |
| Dark stretches | As long as the sleep before the day |
| No record | A day with no data is left empty, and says so |
| Sound | Recorded on my phone; Shosthi's far-off dhak is a filtered copy |
| Colour | Chosen, not measured; the liquid moves faster on days with more steps |

The same legend appears on the entry screen. Bengali terms in the text carry a dictionary-style gloss (headword, pronunciation, meaning) on hover, keyboard focus or tap.

## Run locally

It is a static site with no build step. Browsers block audio and fonts from `file://`, so serve the folder:

```
python3 -m http.server 8000
```

then open http://localhost:8000. A day can be opened directly with a hash, for example `#ashtami` (ids: mahalaya, chaturthi, panchami, shashthi, saptami1, saptami2, ashtami, navami, dashami).

## Deploy

Import the repository into Vercel as a project with the framework preset "Other". There is no build command and no output directory. `vercel.json` only sets long cache headers for audio and fonts.

## Files

- `index.html`: the whole piece (HTML, CSS, JavaScript, WebGL shader, Web Audio cue sheet).
- `audio/`: 17 AAC files in .mp4 containers (field recordings, unlock tick, Mahalaya excerpt, closing track).
- `fonts/`: Baloo Da 2 (variable), self-hosted, SIL Open Font License 1.1 (`fonts/LICENSE-OFL.txt`).

## Credits

- Concept, data, text, field recordings and the closing track "Asche Bochor Abar Hobe": the author.
- Mahalaya excerpt: from the original radio broadcast of Mahishasuramardini, recited by Birendra Krishna Bhadra.
- Code written with Claude (Anthropic) under the author's direction.
- Typeface: Baloo Da 2, SIL Open Font License 1.1.

The piece includes a short tribute to the 19 people who lost their lives at the Chorbagan pandal in Kolkata on 17 October 2026, with links to reporting by [The Quint](https://www.thequint.com/amp/story/news/breaking-news/kolkata-durga-puja-pandal-stampede-investigation-updates) and [The Telegraph](https://www.telegraphindia.com/west-bengal/my-mother-died-before-my-eyes-sons-heartbreaking-account-of-kolkata-chorbagan-stampede/cid/2185273).

## Licence

Copyright (c) 2026 Aritra Banerjee. All rights reserved; see `LICENSE`. The Baloo Da 2 typeface is separately licensed under the SIL Open Font License 1.1 (`fonts/LICENSE-OFL.txt`). The Mahalaya excerpt belongs to its original broadcaster and is not covered by this licence.
