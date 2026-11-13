# AI Logo Design Prompts

40 copy-paste logo briefs for Midjourney, Ideogram, GPT Image and Claude SVG, plus 6 checks to run before you use a logo.

Works with: Midjourney, Ideogram, GPT Image, and Claude or ChatGPT for SVG code

Copy buttons for every brief: [https://brief-library.pages.dev/ai-logo-design-prompts/](https://brief-library.pages.dev/ai-logo-design-prompts/)

## How to write an AI logo prompt

Use the same structure every time (Directed logo brief):

| Part | What goes in it |
|---|---|
| **MARK** | What the logo is and what it says. |
| **STYLE** | The drawing approach and level of detail. |
| **SHAPES** | The forms and geometry to use. |
| **COLOR** | The exact palette and how many colors. |
| **TYPE** | The letterform style for any text. |
| **BACKGROUND** | The canvas, ratio and framing. |
| **AVOID** | What the model must leave out. |
| **ROLE / CONTEXT / TASK / CONSTRAINTS / OUTPUT** | The five parts used for Claude SVG and motion briefs. |

## 6 free AI logo prompts

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Geometric sans wordmark
*Wordmarks*

Use when: You want a modern, neutral name for a software or services brand.

```text
MARK: wordmark logo, the text "[BRAND_NAME]" only, for a [INDUSTRY] business
STYLE: flat vector, precise, minimal, balanced spacing
SHAPES: circular O and C forms, uniform stroke weight, no extra icons
COLOR: one dark color [HEX_COLOR] on white
TYPE: geometric sans serif, medium weight, tight but even kerning
BACKGROUND: plain white, centered, 3:2 ratio, generous margin
AVOID: gradients, shadows, 3D, taglines, extra symbols, misspelled letters
```

Tip: Add "lowercase" or "uppercase" to the TYPE line to change the tone fast.

### Single letter in a shape
*Lettermarks and monograms*

Use when: You need an avatar-ready mark from one initial.

```text
MARK: lettermark, the single letter "[LETTER]" inside a [SHAPE] for [BRAND_NAME], a [INDUSTRY] brand
STYLE: flat vector, bold, simple, app icon feel
SHAPES: one [SHAPE] container, letter centered, 12 percent padding
COLOR: container [HEX_COLOR_1], letter white
TYPE: geometric sans serif, bold, uppercase
BACKGROUND: white, 1:1 ratio, centered
AVOID: gradients, shadows, bevels, extra letters, textures
```

Tip: Try a square with rounded corners, a circle and a hexagon as three runs.

### Abstract geometric symbol
*Symbol marks*

Use when: You want a modern mark that does not depict anything literal.

```text
MARK: abstract geometric symbol for [BRAND_NAME], a [INDUSTRY] company, suggesting [IDEA_WORD]
STYLE: flat vector, bold, balanced, minimal
SHAPES: 3 to 4 basic shapes (circle, triangle, square), overlapping with clean edges
COLOR: 2 colors: [HEX_COLOR_1] and [HEX_COLOR_2]
TYPE: no text
BACKGROUND: white, 1:1 ratio, centered
AVOID: gradients, shadows, 3D, text, more than 4 shapes, realistic objects
```

Tip: Name the feeling in [IDEA_WORD], such as growth, trust or flow.

### Friendly animal mascot
*Mascots and emblems*

Use when: You want a character for a kids brand, local shop or app.

```text
MARK: friendly [ANIMAL] mascot for [BRAND_NAME], a [INDUSTRY] brand, head and shoulders
STYLE: flat vector, thick 5 px outline, simple shapes, 3 shading-free fills
SHAPES: round head, large simple eyes, small smile, one accessory: [ACCESSORY]
COLOR: 4 colors maximum: [HEX_COLOR_1], [HEX_COLOR_2], cream, dark outline
TYPE: no text
BACKGROUND: plain white, 1:1 ratio, centered
AVOID: realistic fur, gradients, scary expressions, tiny details, copyrighted characters
```

Tip: Describe the personality in 2 words, such as calm and curious.

### Turn a concept into clean SVG
*Claude SVG builds*

Use when: You have a logo idea in words and want a first vector draft.

```text
ROLE: You are a senior vector logo designer who writes clean, hand-readable SVG.
CONTEXT: Brand [BRAND_NAME], a [INDUSTRY] business. Concept: [CONCEPT_DESCRIPTION]. Mood: [MOOD_WORDS].
TASK: Draw the logo as one SVG: a symbol on the left and the name "[BRAND_NAME]" on the right.
CONSTRAINTS: viewBox="0 0 600 200". Flat fills only. No gradients, filters, or embedded raster images. Maximum 3 colors: [HEX_COLOR_1], [HEX_COLOR_2], [HEX_COLOR_3]. Use basic shapes and paths. Convert text to simple paths if possible, otherwise use a generic font-family stack and note it. Group parts with ids: symbol, wordmark.
OUTPUT: One SVG code block only, then 3 short bullet notes on what to adjust.
```

Tip: Ask for 3 variations in the same message if you want to compare.

### Shapes assemble
*Make it move*

Use when: You want the symbol to build from separate pieces on a website intro.

```text
ROLE: You are a motion developer who writes GSAP 3 animations for SVG.
CONTEXT: My logo SVG is below, with shapes inside group id="symbol". Brand: [BRAND_NAME].
TASK: Animate the shapes flying in from offset positions and locking into place, then fade in the wordmark.
CONSTRAINTS: Load GSAP 3 from a CDN script tag. Each shape starts 60 px away with opacity 0. Duration 700 ms each, stagger 90 ms, ease "power3.out". Wordmark fades in over 400 ms after 200 ms delay. Total under 2000 ms. Use transform and opacity only. Add a replay button. Under @media (prefers-reduced-motion: reduce), skip animation and show the final logo.
OUTPUT: One HTML file with inline CSS and JS.

[PASTE_SVG_HERE]
```

Tip: Raise the stagger to 140 ms for a calmer build.

## How to use these briefs

1. Pick the brief that matches the logo type you need and copy the whole block.
2. Replace every [PLACEHOLDER] with your own details before you paste.
3. Image briefs go into Midjourney, Ideogram or GPT Image. SVG and motion briefs go into Claude or ChatGPT.
4. Generate 4 options, change one line at a time, and keep the prompt that worked.
5. Run the checks at the end before any logo goes on a sign, site or invoice.
6. Treat results as concepts. Search for similar marks before commercial use.

## The full pack

[AI Logo Design Prompts: 40 Briefs for Midjourney, Ideogram & Claude SVG](https://whop.com/ease-out-studio/ai-logo-design-prompts), $12, one-time, instant download (PDF, a page with copy buttons, a plain text file).

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
