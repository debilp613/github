# Style: "Notebook Explainer"

A teardown of two reference reels (a creator-education talking head, ~1:50 and ~2:27,
576×1024 @ 30 fps, recorded off TikTok). Written so the look can be rebuilt on a new
talking-head clip. `reference/style-sheet.jpg` shows one still of each element below.

---

## 1. The formula in one paragraph

One locked-off selfie take of the speaker, chopped with jump cuts. **A single word of
caption sits on her chest the whole time.** The top ~15% of the frame is a "receipt
zone": small data graphics (counters, meters, chips, strikethroughs) that prove what
she's saying and swap every 2–6 s. Every chapter opens on a **full-screen yellow title
card** with a step number and page dots. Big thesis lines get a **blurred-background
quote card**. A **progress meter that climbs chapter by chapter** (day 1→100 of 100,
or a battery 4%→100%) is the motif that holds the video together. It ends on a CTA and
an animated "Follow" click.

---

## 2. Look: palette, type, layout

### Palette (sampled)
| Token | Hex | Used for |
|---|---|---|
| `yellow` | `#F4E17F` (cards `#F5E37E`) | headline accents, keyword captions, chapter cards, counters, pills |
| `ink` | `#191919` | text on yellow/cream cards, text inside pills |
| `cream` | `#FAF7EE` | alternate chapter card that floods to yellow |
| `white` | `#FFFFFF` | default caption + overlay text |
| `notepad` | `#F1E7A5` + blue rules, red margin | legal-pad scene |
| footage | warm beige wall, orange ring light glow behind her right shoulder | the set is part of the palette, so keep it warm |

There are only three colours plus the footage. Yellow is the only accent, and it marks the
word that matters.

### Typefaces (closest matches)
1. **Geometric bold sans**, which looks like **Poppins Bold/ExtraBold**: captions, headlines, card titles.
   Lowercase almost everywhere ("the first 2 weeks:").
2. **Condensed high-contrast italic serif**, close to **Instrument Serif Italic**
   (Playfair Display Italic is a fallback): *the emphasis word*. On cards it's set larger than the sans
   ("empty your **brain.**", "*full lives.*"). In captions it replaces the sans for keywords.
3. **Casual handwriting**, close to **Gochi Hand / Caveat**: small sub-labels under data
   ("+ a moment", "4 stops, 100 days", "real data, not guesses") and the notepad text.

Rule: **sans states it, serif feels it, handwriting annotates it.**

### Frame zones (9:16)
```
┌──────────────────────┐
│  RECEIPT ZONE        │  ~4–16% from top: title / data overlay, centred
│  (dark soft scrim)   │
│                      │
│        face          │
│                      │
│   ── CAPTION ──      │  ~58–65% from top: on the chest, below the mic
│   [logo strip/card]  │  ~66–72%: secondary inserts (logos, follow card)
│                      │
└──────────────────────┘  bottom ~20% left clear (platform UI)
```
- Captions never move. One fixed line, centred.
- **Top scrim:** every top overlay sits on a big, very soft dark ellipse (≈ black
  35–45%, huge feather) for legibility. It fades out **1–2 frames later than the text**,
  so between overlays you briefly see a smoky shadow. That's part of the look.

---

## 3. Captions (on the whole time)

- **One word at a time** (two only for tiny words: "I'm about", "to build", "in marketing").
- White Poppins Bold, ~9–10% of frame width in cap height, soft drop shadow (no box,
  no stroke).
- **Keyword swap:** roughly 1 word in 8–12 is set in the **yellow italic serif**, a touch
  larger: *wrong, mapped, perfect, 22, kids, formats, opinion, story, expect, tuesday,
  brand*. These are the emotional or surprising words, not the nouns.
- **Transition between words:** 1–2 frame cross-dissolve (you see both words ghosted
  on one frame). No pop, no bounce, no scale. It reads as calm, not "MrBeast".
- Captions are hidden on full-screen cards (they return the moment the footage does).

---

## 4. Top "receipt" overlays (the component kit)

Each lives in the receipt zone for ~2–6 s, enters with a **3–4 frame fade + slight
blur-to-sharp**, exits with a **3 frame fade-and-blur**. Lines inside build
**one at a time, synced to the words she says**.

| # | Component | Build | Example |
|---|---|---|---|
| A | **Hook title** | small white bold line over huge yellow bold line, there from frame 0 for ~4.5 s | "Build your brand / **in 100 days**" |
| B | **Rolling counter** | icon + label, number counts up 0→N over ~0.8 s ease-out, then a second line drops in | 🔖 saved: 0→96→…→**1,204** / **used: 0** |
| C | **Day grid** | 10×10 dot grid fills cell by cell + "day **44** of 100", handwriting subline changes per chapter | "+ 12 posts of proof" |
| D | **Battery meter** | battery icon fills + "**25%** interesting", rolls up when a new step lands | 4% → 22% → 25% → 38% → 50% → 71% → 75% → 83% → 100% |
| E | **Strikethrough rewrite** | word appears → line draws through it L→R (~4 frames) + dims → "→" + yellow replacement fades in | ~~perfect~~ → **posted**, ~~4-hour edits~~ → **30 minutes** |
| F | **Chip/pill row** | rounded pills appear left→right, one per beat; filled = done, outlined grey = upcoming | `2 weeks` `month 1` `month 2` `month 3` / numbered `1` `2` `3` boxes that get filled with labels |
| G | **Checklist pills** | white pills with yellow ✓, stack downward one per beat | ✓ 36 posts ✓ 1 clear message ✓ the people who want it |
| H | **Fill-in-the-blank** | white rounded box with black text and `___` | "I'm the person who ___" |
| I | **Fake UI** | search bar + big yellow "No Results"; "Recently Deleted"; Albums widget filling with thumbnails | sells the problem visually |
| J | **Speech-bubble label** | white rounded-rect, black bold text, little tail | "wait, that's me", "so what?" |
| K | **Logo strip** | 2 rows of small brand logos at chest height, popping in L→R with 1-frame stagger | credibility beat |
| L | **Photo cards** | small rounded photo cards with yellow label pill on top ("full-time job", "3 kids"), slide/fade in one after another, top-left | personal proof |
| M | **Phone insert** | iPhone screen-recording mockup **scales up from ~60% at bottom-centre to ~80% width in 2–3 frames**, camera roll scrolls fast while a giant yellow number counts 0→18,000 on top | ~1.5 s, hard cut out |
| N | **Ghost screen** | screen recording of a doc at ~60% opacity laid over the whole frame while she keeps talking | showing the freebie |
| O | **Follow card** | dark rounded card (avatar, name, blue **Follow**) at chest; cursor arrow glides in, clicks, button turns grey "Following" | last ~6 s |
| P | **CTA pill** | yellow pill, black bold "comment ***RISE***" with italic keyword | close |

---

## 5. Full-screen moments

1. **Blur quote card**: hard cut to the same footage **heavily Gaussian-blurred and
   darkened (~35%)**. A 2–3 line statement builds line by line: white sans lines, then
   the payoff in **big yellow italic serif**, optional handwriting sub-line.
   Lines fade in over 2 frames. Exit: 3–4 frame dissolve back to sharp footage.
   Use for theses ("this plan is for people with *full lives.*", "it's not the topic, it's how you
   *introduce it*", "stop scrolling."). Sometimes a strikethrough plays inside it.
2. **Yellow chapter card**: full-bleed `yellow`, top row: "step 1 / days 1–14 /
   month 2" (small bold) left and **page dots `●○○○`** right (dots fill per chapter).
   Headline in big ink sans, payoff word in big ink italic serif, revealed on her words.
   Extras: underline that draws under "*smarter.*", strikethrough on "topic.",
   checkbox that ticks ☐→☑ on "*do.*", hand-drawn arrow "↘ a *consequence.*".
   - **In:** **slides up from the bottom** in ~4 frames (fast ease-out). The text
     inside lags a frame (slight parallax).
   - **Out to footage:** 3-frame cross-dissolve.
   - **Out to another full-screen:** **push up**: the next card/notepad slides up and
     shoves the yellow card off the top (~4 frames).
3. **Cream → yellow flood**: once per video, the chapter card starts on `cream`, and
   on the payoff word yellow **floods up from the bottom in ~3 frames** (like a
   highlighter filling the page) while the serif word fades in.
4. **Notepad**: a yellow legal pad (small header "brain dump" / "before you post")
   fills the screen. A **pencil writes a numbered list in handwriting, letter by letter**,
   synced to her voice (~8–10 s). Then a bracket/line is drawn down the margin.
   Entered by the push-up from the chapter card.
5. **Grayscale punchline**: hard cut to black-and-white footage on the punchline
   ("**used: 0**", "boring topic", "boring organization tip"), held ~1–1.5 s, hard cut back.

---

## 6. Cuts & rhythm

- **Jump cuts** between every sentence or breath, alternating between the base framing and
  a **~110–115% punch-in** so cuts feel intentional. No camera moves otherwise.
- Something on screen changes about **every 2–3 s** (caption aside): overlay swap, card,
  blur, grayscale, insert.
- Full-screen cards come in at the **start of every chapter**, and blur cards at
  **every thesis line**, roughly every 15–25 s.
- Overlay changes land **on the spoken word**, never on a beat of the music.
- Ending: last chapter → CTA/follow beat → (platform outro; not part of the edit).

### Audio
The audio is continuous under the voice (only one silence in ~2 min), which suggests a
quiet music bed ducked well under speech. I couldn't confirm per-transition whooshes or
pops from the mix. If recreating, use a low lo-fi bed at about −25 dB under the voice,
plus optional soft "pop"/"tick" SFX on counters and checkbox ticks, and a pencil-scratch
loop on the notepad.

---

## 7. Beat maps of the references

**Ref 1 — "Build your brand in 100 days" (1:50)**
| t | Beat |
|---|---|
| 0:00 | Hook title (A) |
| 0:05 | Pill row "2 weeks · month 1 · month 2 · month 3 / 4 stops, 100 days" (F) |
| 0:07 | Rolling counter saved: 1,204 (B) → 0:10 **grayscale** "used: 0" (5) |
| 0:12 | Logo strip "brands I have worked with" (K) |
| 0:14 | Photo cards "full-time job / 3 kids" (L) |
| 0:16.5 | Blur card "this plan is for people with *full lives.*" |
| 0:19 | Yellow card "days 1–14 · the first 2 weeks: *empty your brain.*" |
| 0:22.5 | Push-up → notepad "brain dump" list |
| 0:31.5 | Fill-in-blank "I'm the person who ___" (H) |
| 0:33 | Day grid "day 1→14 of 100 + your front door" (C) |
| 0:35 | Yellow card "month 1 · it's about *showing* **up.**" |
| 0:37 | M T W T F S S chips "3 a week is plenty" · strikethroughs (E) · 1/2/3 format boxes (F) · "posts" grid 0→12 |
| 0:50 | Day grid → day 44 |
| 0:52.5 | Yellow card "month 2 · where we get *smarter.*" (underline draws) |
| 0:54.5 | "open insights on every post" icons build · "your strongest idea, said 3 new ways ×3" |
| 1:02 | Blur card "please stop assuming *it didn't work* just because it didn't go viral" |
| 1:05.5 | Counter "2,000 views — that's a full theater" |
| 1:09 | Cream→yellow card "month 3 · where we build *momentum.*" |
| 1:11 | Day grid → 74 · "ep.1 ep.2 ep.3" chips · "you asked, I answered" · fill-in-blank |
| 1:22 | Bubble "could you do this on your worst week?" · day grid → 100 |
| 1:29 | Checklist pills (G) · "a personal brand is just what people expect from you" |
| 1:36 | Blur card "not by waiting ~~until you're ready~~ *a plan* you can actually follow" |
| 1:39.5 | CTA pill "comment *RISE*" · ghost-screen doc (N) · follow card (O) |

**Ref 2 — "How to make boring content addictive" (2:27)**
| t | Beat |
|---|---|
| 0:00 | Hook title; 0:04 **grayscale** on "boring topic" |
| 0:06 | Logo strip; 0:08.5 "yes, *even yours.*" |
| 0:10.5 | Blur card "it's not the *topic* — it's how you *introduce it*" |
| 0:15 | Numbered boxes 1 2 3 4 "same example, all 4 times" |
| 0:20 | Retention-curve graphic "step 2 — where they scroll away" |
| 0:23 | Yellow card "step 1 · start with a *moment,* not a ~~topic.~~" |
| 0:27.5 | **Battery 4%** interesting |
| 0:30 | Title pill "5 ways to organize your camera roll ×100" → **phone insert** 0→18,000 (M) |
| 0:39 | Fake search "No Results" (I) · bubble "wait, that's me" |
| 0:44 | Blur card "that's what makes them **stop** scrolling." |
| 0:46 | Battery → 25% |
| 0:49.5 | Yellow card "step 2 · give the problem ↘ a *consequence.*" |
| 0:52 | Retention curve · bubble "so what?" · "same topic, now with stakes" · timer 10:47→20:00 · "Recently Deleted" |
| 1:07.5 | **Grayscale** "~~boring organization tip~~ cost: 20 min + 1 post" |
| 1:11.5 | Battery → 50% |
| 1:13.5 | **Cream→yellow** "step 3 · show the moment something *changed.*" |
| 1:15.5 | "storytellers call this *the turn*" · fill-in-blank story frame |
| 1:22.5 | Blur card "~~too many photos~~ no *system*" |
| 1:26.5 | Albums widget fills (I) · 1:32 blur card "same *topic.*" |
| 1:35 | Battery → 75% |
| 1:39 | Yellow card "step 4 · give them something they can actually *do.* ☐→☑" |
| 1:42 | Quote "~~just get organized!~~" · breadcrumb "Collections › Albums › + New Album" · "5:00 tonight" timer |
| 1:51.5 | **Battery → 100% addicting** |
| 1:53.5 | Blur card 🔖 "the kind of content they *save.*" |
| 1:57 | Notepad "ask yourself 4 questions" |
| 2:07 | Blur card "make your audience *care*" |
| 2:10 | Recap pills "1 a moment · 2 a consequence · 3 what changed · 4 what to do" |
| 2:16.5 | "0 → 20,000 by Thanksgiving, come watch." + follow card click |

---

## 8. How to rebuild it on a new clip

1. **Script/transcript first.** Get word-level timestamps (everything syncs to words).
2. **Mark the structure:** hook → credibility → thesis (blur card) → N chapters (yellow
   card each) → recap → CTA. Choose the **progress motif** (day X/100, battery %,
   level bar…) and the value it reaches at each chapter.
3. **Tag words:** 1-in-~10 serif keywords; punchline words for grayscale; numbers for
   counters; "wrong → right" pairs for strikethroughs.
4. **Assign one receipt overlay per 2–6 s of talking** from the kit in §4.
5. **Cut:** jump cuts on breaths, alternate 100% / ~112% framing.
6. **Build:** keep the three typefaces and one yellow. Use the motion timings in §4–5
   (fast 3–4 frame moves, ease-out, no bounce).
7. **Audio:** quiet bed, light SFX on ticks and counters.

Tools: CapCut or Premiere/After Effects by hand, or code (Remotion / HTML-canvas +
ffmpeg). For an automated pass, feed this file and `reference/style-sheet.jpg` into the
Reel Kit style step as the inspiration source.
