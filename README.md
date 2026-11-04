# Pujo 2026 Scroll

A scroll-driven piece about the days of Durga Pujo, Mahalaya to Doshomi, made from one person's own data and recordings. Scroll is time: the page only moves forward when you do. Best on desktop, with sound.

## How to read it

| What you see or hear | What it comes from |
| --- | --- |
| One footprint appears for every 100 steps | Daily step count from the author's phone |
| The small number, bottom left | The same step count |
| The saree-border ribbon on both edges | Its width follows the day's steps; its sawtooth edge gets denser with more phone unlocks |
| "Unlocks" counter, top right, with a faint tick | Phone unlock count (one soft tick per nine unlocks, so it stays quiet) |
| The length of each dark gap between days | Hours slept the night before (6 screen heights per hour) |
| "No record" | Days with no data. Gaps are shown as gaps, not filled in |
| The colour of each day, and the liquid wipe between days | Chosen by the author for each day |
| Field recordings | Recorded on the author's phone during Pujo, level-matched and looped |
| Muffled dhak on Shosthi | A low-pass-filtered copy of the Ponchomi aarti recording, used because dhak was audible that day but not recorded. It is a treatment, not a recording |
| Closing music | *Asche Bochor Abar Hobe*, the author's own track |

Days with no phone data (Mahalaya, Choturthi) have no step or unlock readings. The piece ends on the phrase আসছে বছর আবার হবে.

## Run it locally

No build step. From this folder:

    python3 -m http.server 8000

then open http://localhost:8000. (Opening index.html directly from disk will not load the audio.)

## Deploy

It is a static site. Import the repository in Vercel as a plain static project (framework preset: Other, no build command, output directory: the repository root).

## Structure

    index.html        the whole piece: markup, styles and script
    audio/            edited recordings (AAC in .mp4) and the closing track
    fonts/            Baloo Da 2 (SIL Open Font License 1.1), self-hosted
    vercel.json       cache headers

## Credits

Concept, data, field recordings, text, music and art direction: Aritra Banerjee.
Implementation (code) written with AI assistance from Claude (Anthropic), under the author's direction.
Typeface: Baloo Da 2 by Ek Type, SIL Open Font License 1.1 (see fonts/LICENSE-OFL.txt).

## Before this goes public

- Confirm the source and permission for the Mahalaya broadcast excerpt (audio/mahalaya.mp4), and credit it correctly.
- Add sources for the Chorbagan tribute (the number, the venue, the date) to the write-up.
- Add a licence for the code and media (for example all rights reserved, or Creative Commons for the recordings).
