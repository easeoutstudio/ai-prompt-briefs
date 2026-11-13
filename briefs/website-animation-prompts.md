# Website Animation Prompts for Claude and GSAP

30 copy-paste briefs for logo reveals, hero entrances, buttons, loaders, scroll and text effects, each with the working HTML/GSAP file it produced.

Works with: Claude, ChatGPT or any AI that writes HTML, CSS and JavaScript (GSAP from a CDN)

Copy buttons for every brief: [https://brief-library.pages.dev/website-animation-prompts/](https://brief-library.pages.dev/website-animation-prompts/)

## How to write a GSAP animation prompt for Claude

Use the same structure every time (The Brief Formula):

| Part | What goes in it |
|---|---|
| **WHAT MOVES** | Name the element, not the vibe: "headline words", not "make it pop". |
| **FROM WHERE** | Direction and distance: "rise from a mask", "slide in from -40px". |
| **HOW LONG** | Milliseconds. Entrances 400 to 700ms, exits 300 to 400ms, press feedback 90 to 200ms. |
| **WHICH EASE** | Ease-out for entering, ease-in for leaving, linear only for loops. |
| **IN WHAT ORDER** | Start times and stagger: "60ms apart", "the button lands last". |

## 5 free website animation briefs from the pack

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Logo reveal: Three shapes assemble the mark

Use when: Brief 01 of 30 in the Directed Motion Pack.

```text
Logo reveal for "Larkspur" on a dark background.
1. Three shapes (circle, quarter, square) fly in and assemble the mark: 600ms each, expo.out, 80ms apart.
2. The mark settles with a 1.07 to 1 scale bump, back.out(3).
3. Wordmark letters rise from a mask, 40ms apart, back.out(1.6).
4. One soft light sweep crosses at 1.6s, then hold.
Total under 2.2s. Reduced motion: show the end state.
Output: one HTML file, GSAP from the CDN, all timings in one block at the top.
```

Tip: Assembly reads as craft. The bump at the end is the only overshoot, so it lands.

### Hero entrance: Headline words rise, CTA lands last

Use when: Brief 07 of 30 in the Directed Motion Pack.

```text
Landing hero for a design studio.
1. Headline words rise from a mask, 60ms apart, expo.out, 600ms.
2. Subhead fades up 12px at 0.35s, power2.out.
3. CTA button scales from 0.9 at 0.5s, back.out(2), 450ms.
4. Nav fades down from -20px at 0s.
Whole entrance under 1s. Reduced motion: show the end state.
Output: one HTML file, GSAP from the CDN, all timings in one block at the top.
```

Tip: The CTA arrives last on purpose: the eye ends where you want the click.

### Button & micro: Hover lift, press squash

Use when: Brief 14 of 30 in the Directed Motion Pack.

```text
Button that feels physical.
hover: lift 3px, shadow grows, 200ms, power2.out
press: scale x 1.04, y 0.92, 90ms, power1.out
release: back to 1 with back.out(3), 400ms
focus-visible: 3px accent outline
Reduced motion: color change only.
Output: one HTML file, GSAP from the CDN, all timings in one block at the top.
```

Tip: Squash on press, overshoot on release. That is the whole secret of buttons that feel expensive.

### Loader: Skeleton shimmer to content

Use when: Brief 21 of 30 in the Directed Motion Pack.

```text
Card list loading state.
1. Three skeleton cards with a shimmer band: linear, 1.4s per pass, infinite.
2. After 2s (demo) skeletons fade out 250ms.
3. Real cards fade up 16px, 80ms apart, power3.out, 500ms.
4. Demo loops.
Reduced motion: no shimmer, simple crossfade.
Output: one HTML file, GSAP from the CDN, all timings in one block at the top.
```

Tip: Shimmer says still loading; the stagger on arrival says done, in order.

### Text: Marker highlight sweep

Use when: Brief 30 of 30 in the Directed Motion Pack.

```text
Sentence with one key phrase highlighted.
1. Sentence rises in by words, 50ms apart.
2. At 0.7s a marker highlight sweeps behind the key phrase left to right, 600ms, power3.out.
3. Highlight is slightly rotated, -1deg, with rough ends.
4. Key phrase text turns dark as the marker passes.
Reduced motion: highlight shown.
Output: one HTML file, GSAP from the CDN, all timings in one block at the top.
```

Tip: Highlight after the read, not with it: first they read, then you tell them what matters.

## How to use these briefs

1. Write one line per moving thing, not one line for the whole screen.
2. Answer five questions on every line: what moves, from where, how long, which ease, in what order.
3. Close every brief with the total time and the reduced motion fallback.
4. Paste the brief into Claude or ChatGPT and ask for one HTML file with GSAP from the CDN.
5. If the result is off, send a fix-it prompt instead of starting over.

## The full pack

[Directed Motion Pack: 30 Website Animation Briefs + Working HTML/GSAP Components](https://whop.com/ease-out-studio/directed-motion-pack), $19.99, one-time, instant download (PDF, a page with copy buttons, a plain text file).

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
