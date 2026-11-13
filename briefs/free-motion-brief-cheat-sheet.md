# Free Website Animation Cheat Sheet

The formula, the eases and 5 real briefs from the Directed Motion Pack.

Works with: Claude, ChatGPT

Copy buttons for every brief: [https://brief-library.pages.dev/free-motion-brief-cheat-sheet/](https://brief-library.pages.dev/free-motion-brief-cheat-sheet/)

## How to write a website animation prompt

Use the same structure every time (The Brief Formula):

| Part | What goes in it |
|---|---|
| **WHAT MOVES** | Name the element, not the vibe: "headline words", not "make it pop". |
| **FROM WHERE** | Direction and distance: "rise from a mask", "slide in from -40px". |
| **HOW LONG** | Milliseconds. Entrances 400 to 700ms, exits 300 to 400ms, press feedback 90 to 200ms. |
| **WHICH EASE** | Ease-out for entering, ease-in for leaving, linear only for loops. |
| **IN WHAT ORDER** | Start times and stagger: "60ms apart", "the button lands last". |

## 14 free easing rules and fix-it prompts

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Entering

```text
expo.out or power3.out
```

### Leaving

```text
power2.in
```

### Moving between two spots on screen

```text
power3.inOut
```

### Loops, spinners, marquees, scroll scrub

```text
none (linear)
```

### Breathing and floating

```text
sine.inOut
```

### One playful accent per screen

```text
back.out(1.5 to 3)
```

### Springy return

```text
elastic.out(1, 0.4), use rarely
```

### Feels slow

```text
Cut every duration by 30% and every stagger in half. Keep the eases.
```

### Feels robotic

```text
Replace every linear ease on entrances with expo.out. Keep linear only on loops.
```

### Too bouncy

```text
Keep overshoot only on [element]. Everything else power3.out.
```

### Everything moves at once

```text
Stagger the elements 60 to 80ms apart in reading order. The button lands last.
```

### Busy

```text
Remove every loop except one. Make the one that stays at least 4s per cycle.
```

### Janky on phones

```text
Animate only transform and opacity. No width, top, left or shadows inside loops.
```

### Forgot accessibility

```text
Respect prefers-reduced-motion: show the end state and keep loops off.
```

## How to use these briefs

1. Write one line per moving thing, not one line for the whole screen.
2. Answer five questions on every line: what moves, from where, how long, which ease, in what order.
3. Close every brief with the total time and the reduced motion fallback.
4. Paste the brief into Claude or ChatGPT and ask for one HTML file with GSAP from the CDN.
5. If the result is off, send a fix-it prompt instead of starting over.

## The full pack

Get the free PDF and copy-button page: [Free Motion Brief Cheat Sheet: Animate Websites with Claude + GSAP](https://whop.com/ease-out-studio/free-motion-brief-cheat-sheet)

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
