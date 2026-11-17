# Notebook Explainer: Debi Pomerantz edition

The reel structure from `../../STYLE.md`, re-skinned with the Debi Pomerantz design
system (`tokens.json`, copied from the brand zip). See `preview.jpg` for ten mock frames.
`frames.html` is the source (it expects `photo.jpg` + `headshot.jpg` from the brand Photography folder beside it).

**Rule of thumb:** keep the *structure* of the reference (one-word captions, receipt
zone, chapter cards, quote cards, notepad, climbing meter). Take every colour, font,
shape and annotation from the brand.

---

## 1. Token mapping

| Reference element | Reference value | Debi edition |
|---|---|---|
| Accent (keywords, counters, highlights) | yellow `#F4E17F` | **sunshine `#FFC22E`** (text on it is plum `#2A1824`, never white) |
| Chapter card | yellow fill | **butter `#FFE9A8`** with `ink` text |
| "Before" card that floods | cream `#FAF7EE` | **ground `#FFFCF7`** → floods to **sunshine** |
| Card text / ink | `#191919` | **ink (plum) `#2A1824`**, which replaces black everywhere |
| Caption text over footage | white + soft shadow | **`#FBEFE6` cream + hard 3px plum offset shadow** (sticker style, no blur) |
| Soft dark scrim behind top overlays | black ellipse, feathered | **removed** (no gradients or soft shadows). Overlays sit on **ground cards**: 2px ink border, `radius-lg`, `sticker` 4px 4px 0 plum |
| Blur-card darkening | black ~35% | flat **plum tint `rgba(42,24,36,.55)`** over the blur |
| Strikethrough line | white/grey | **berry `#B8255E`** (berry = "here's the real issue"), and the correct word goes in a **sunshine pill** |
| Grayscale punchline | B&W footage | **berry margin note**: a hand-drawn circle draws round the punchline number (~1 s), with a Caveat note: "the real issue", "not this", "start here" |
| Handwritten sub-labels | marker font, white | **Caveat 600**: `ink-soft` on cards, `blush` on the plum quote card |
| Page dots `●○○○` | white dots | **Stepper**: 8px pill segments, done = `ink`, current = `tangerine`, rest = faint, plus "Step 1 of 4" in words |
| Progress motif (day grid / battery) | yellow | **pill track** on `surface` with an ink outline, filling in **tangerine**; label "day 44 of 100" in Young Serif |
| CTA pill | yellow pill | ground card with a Young Serif keyword ("comment *clarity*") |
| Follow button | blue | **tangerine primary button**, ink border, plum text. It's the one tangerine action on screen |
| Icons (bookmark etc.) | filled emoji-like | **2px ink strokes, round caps** |

## 2. Type mapping

| Job | Reference | Debi edition |
|---|---|---|
| Captions, headlines, labels | Poppins Bold | **Figtree 700** |
| Emotional keyword / payoff | italic serif (Instrument-like) | **Young Serif** (one weight, upright, never fake bold or italic) |
| Annotations, notepad | casual marker | **Caveat 600** (≥24px equivalent) |

Load: `Young+Serif`, `Figtree:wght@400;500;600;700`, `Caveat:wght@600`.

## 3. Where the brand overrides the reference (decisions made)

1. **"No single highlighted word inside a headline."** On cards the payoff gets **its own
   line** in Young Serif ("the first 2 weeks:" / "empty your brain."), never one coloured
   word in the middle of a sans line. The caption keyword swap still happens, because a
   caption is one word on its own, not a word inside a headline.
2. **No gradients, no soft shadows.** The smoky top scrim becomes solid ground cards with
   the sticker shadow. Captions use a hard plum offset instead of a blur shadow.
3. **No filters on Debi's images.** Grayscale is out; the margin note does the job.
   The blur on quote cards is kept, since it's a transition behind type rather than a look
   on her photograph. Drop it too if you'd rather be strict.
4. **Margin note limits:** max one per screen, never on a sunshine or tangerine fill (so
   not on the flood card), and only pointing at the diagnosis.
5. **One tangerine per screen:** the stepper's current segment, the meter fill and the
   Follow button never share a frame.
6. **Sentence case, no emoji, no all caps.** Applies to every overlay.
7. **Motion:** the web rule ("two movements only") is for the site UI. In video, keep the
   reference's fast 3–4 frame, no-bounce moves. The brand's own motions still show up:
   the margin-note circle **draws in over ~1 s**, and cards land with a **2px up-left sticker
   lift**.

## 4. Footage

Match the brand photography: natural, warm light (autumn tones carry tangerine and
sunshine for free), plain dark or neutral clothing, looking at camera. No grading, no
studio flash. A warm indoor corner works too if the light is soft.

## 5. Voice check for on-screen text

Name the thing → one next step. "Here's the real issue." not "7 steps to…".
No hustle language, no overnight-results promises, laugh *with* her, never at.
