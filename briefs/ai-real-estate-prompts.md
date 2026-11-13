# AI Prompts for Real Estate Agents

42 copy-paste briefs for listings, social posts, video tours, staging, emails and market updates, plus 5 compliance checks, with Fair Housing guardrails in every brief.

Works with: Claude or ChatGPT for text, image models for virtual staging concepts, video models for short clips

Copy buttons for every brief: [https://brief-library.pages.dev/ai-real-estate-prompts/](https://brief-library.pages.dev/ai-real-estate-prompts/)

## How to write a real estate listing prompt

Use the same structure every time (Directed Brief):

| Part | What goes in it |
|---|---|
| **ROLE** | Who the AI should act as, so the tone and skill level are set. |
| **CONTEXT** | The facts you supply: property, client, market source and goal. |
| **TASK** | The one job the AI must do in this run. |
| **CONSTRAINTS** | Hard limits: length, tone, Fair Housing, data rules and banned content. |
| **OUTPUT** | The exact format, count and length you want back. |

## 6 free real estate prompts

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Single family home
*Listing descriptions*

Use when: You are writing the main description for a standard house listing.

```text
ROLE: You are a real estate copywriter for a US residential agent.
CONTEXT: Single family home at [NEIGHBORHOOD]. [BEDS] beds, [BATHS] baths, [SQFT] sq ft, lot [LOT_SIZE]. Key features: [FEATURE_LIST]. Updates and years: [UPDATES_WITH_YEARS]. Nearby places I verified: [VERIFIED_PLACES].
TASK: Write a listing description that leads with the strongest feature and moves through the home in a logical walk.
CONSTRAINTS: 150 to 180 words. Plain US English. No clichés like 'must see'. Use only the facts above. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: 1 description in 2 short paragraphs, then 1 line listing 3 facts I should double-check.
```

Tip: Put the feature buyers ask about most first in FEATURE_LIST so the opening line uses it.

### Just listed
*Social posts*

Use when: A new listing goes live and you want a launch post.

```text
ROLE: You are a social media writer for a US real estate agent.
CONTEXT: Just listed at [NEIGHBORHOOD]. [BEDS] beds, [BATHS] baths, [SQFT] sq ft. 3 best features: [FEATURE_1], [FEATURE_2], [FEATURE_3]. Link or contact: [LINK_OR_CONTACT]. Agent and brokerage: [AGENT_NAME], [BROKERAGE_NAME].
TASK: Write 3 caption options for a just listed post.
CONSTRAINTS: Each caption 40 to 70 words. One call to action each. 5 hashtags each, local and plain. No invented urgency. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: 3 captions, each with hashtags, and a 1-line note on which photo to pair with each.
```

Tip: Use the 3 options on different platforms rather than posting all of them in one place.

### 30-second walkthrough plan
*Video tour shot lists*

Use when: You need a quick tour video planned before you shoot.

```text
ROLE: You are a video producer who plans short real estate tours.
CONTEXT: Property at [ADDRESS_OR_AREA]. Rooms and features: [ROOM_LIST]. Best natural light time: [LIGHT_TIME]. Camera: [CAMERA_OR_PHONE] at 4K 30fps, horizontal 16:9.
TASK: Plan a 30-second walkthrough with clip timings.
CONSTRAINTS: 8 to 10 clips, each 2 to 4 seconds. Include one opening clip and one closing clip with contact details [CONTACT]. Show only what is really there. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: A table of clip number, duration in seconds, location, camera move, and on-screen text of 6 words or fewer.
```

Tip: Shoot a few extra seconds of each clip so you have room to trim.

### Empty living room staging concept
*Virtual staging and photos*

Use when: You have a vacant living room photo and want a staged concept.

```text
ROLE: You are an interior stylist writing prompts for an image model.
CONTEXT: Real photo of an empty living room, [ROOM_SIZE] ft, with [FIXED_FEATURES] such as windows, fireplace and flooring. Style direction: [STYLE]. Palette: [PALETTE].
TASK: Write 3 prompts for a virtually staged version of the photo with furniture and decor only.
CONSTRAINTS: Keep walls, windows, doors, floors, ceiling and room dimensions exactly as in the photo. Furniture must fit the real scale. No people. Include the required label: Virtually staged. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: 3 prompts under 70 words each, a negative prompt list, and a 1-line disclosure for the listing caption.
```

Tip: Name the real flooring and wall color so the model does not repaint them.

### New lead reply
*Emails and follow-ups*

Use when: A new inquiry arrives and you want to respond quickly and clearly.

```text
ROLE: You are an email writer for a US real estate agent.
CONTEXT: Lead name [LEAD_NAME], source [LEAD_SOURCE], inquiry text: [INQUIRY_TEXT]. My availability: [AVAILABILITY]. Agent and brokerage: [AGENT_NAME], [BROKERAGE_NAME].
TASK: Write a reply that answers the question asked and proposes one next step.
CONSTRAINTS: 90 to 120 words. Warm, direct, no pressure. No guesses about the lead's situation. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: 1 subject line, 1 email body, and 1 text message version under 40 words.
```

Tip: Paste the lead's exact message so the reply answers what they actually asked.

### Monthly market update
*Market updates and education*

Use when: You publish a monthly update using numbers you pulled yourself.

```text
ROLE: You are a market update writer for a US real estate agent.
CONTEXT: Area [AREA], month [MONTH_YEAR]. Data I pulled from [MY_DATA_SOURCE]: median price [MEDIAN_PRICE], closed sales [CLOSED_SALES], active listings [ACTIVE_LISTINGS], days on market [DAYS_ON_MARKET]. Prior month figures: [PRIOR_MONTH_FIGURES].
TASK: Write a plain-language monthly update that compares this month with last month using only these numbers.
CONSTRAINTS: 200 to 260 words. Name the data source and date in the text. Do not predict future prices. No numbers beyond what I gave. Follow Fair Housing rules: describe the property and not the people, no words about who should live there. Market data only from my own sources, never invented.
OUTPUT: 1 article with 3 subheads, 1 email summary under 80 words, and 1 social caption under 50 words.
```

Tip: If a figure is missing, leave it blank and ask the AI to skip it rather than guess.

## How to use these briefs

1. Pick the brief that matches your task and copy the whole block into Claude or ChatGPT.
2. Replace every [PLACEHOLDER] with facts from your own listing file, MLS entry or client notes.
3. Paste your real numbers and sources. Never ask the AI to supply prices, stats or trends.
4. Read the draft against the property. Fix anything the AI added that you cannot verify.
5. Run the finished copy through a Compliance check before you publish.
6. You are responsible for the final review of every word, image and disclosure.

## The full pack

[AI Prompts for Real Estate Agents: Listings, Social Posts & Video Tours](https://whop.com/ease-out-studio/ai-real-estate-prompts), $12, one-time, instant download (PDF, a page with copy buttons, a plain text file).

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
