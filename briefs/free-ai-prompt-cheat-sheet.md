# Free AI Prompt Cheat Sheet

A free one-page formula and 12 before and after briefs that turn generic AI answers into specific ones.

Works with: Claude, ChatGPT, Gemini and any chat AI

Copy buttons for every brief: [https://brief-library.pages.dev/free-ai-prompt-cheat-sheet/](https://brief-library.pages.dev/free-ai-prompt-cheat-sheet/)

## How to write a better AI prompt

Use the same structure every time (The Brief Formula):

| Part | What goes in it |
|---|---|
| **ROLE** | Tells the AI who to act as so it answers with the right expertise and point of view. Rule: name a job, not a vague adjective. |
| **CONTEXT** | Gives the facts about you, your audience and the situation that the AI cannot guess. Rule: paste real details, never assume it knows them. |
| **TASK** | States the one thing you want done, using a clear action verb. Rule: one task per brief. |
| **CONSTRAINTS** | Sets the limits: length, tone, what to avoid and what to never invent. Rule: use numbers instead of adjectives. |
| **OUTPUT** | Describes the exact shape of the answer so you can use it without reformatting. Rule: name the format and how many options you want. |

## 8 free before and after prompt briefs

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Client email

Use when: Instead of: "Write an email to my client about the delay."

```text
ROLE: You are a senior account manager who writes calm, direct client emails.
CONTEXT: I run [BUSINESS_TYPE]. My client [CLIENT_NAME] expected [DELIVERABLE] on [ORIGINAL_DATE]. It will now arrive on [NEW_DATE] because [REASON]. Our relationship so far: [RELATIONSHIP_NOTES].
TASK: Write an email that explains the delay, takes responsibility and confirms the new date.
CONSTRAINTS: 120 to 160 words. One apology only. Do not blame third parties. Do not promise anything beyond [NEW_DATE]. Plain US English, no corporate filler.
OUTPUT: 2 subject line options, then the email body ready to send.
```

Tip: The brief supplies the dates, the reason and the word limit, so the AI has nothing to pad or invent.

### Landing page hero copy

Use when: Instead of: "Write a headline for my landing page."

```text
ROLE: You are a conversion copywriter who works with small businesses.
CONTEXT: Product: [PRODUCT_NAME], [ONE_LINE_DESCRIPTION]. Audience: [AUDIENCE]. Their main problem: [PROBLEM]. Real proof I can show: [REAL_PROOF_OR_NONE].
TASK: Write the hero section copy for the top of the page.
CONSTRAINTS: Headline max 10 words. Subhead max 25 words. Button label max 4 words. No invented numbers, reviews, scarcity or urgency. Use only the proof listed above.
OUTPUT: 3 options as a numbered list. Each option has a headline, a subhead and a button label.
```

Tip: Hard word limits and a ban on invented proof keep the copy short and honest.

### Product description

Use when: Instead of: "Write a product description for my candle."

```text
ROLE: You are an ecommerce copywriter who writes clear, sensory product pages.
CONTEXT: Product: [PRODUCT_NAME] from [BRAND_NAME]. Materials: [MATERIALS]. Size: [SIZE]. Typical buyer: [BUYER]. Facts you may use: [FACT_LIST].
TASK: Write the product page description.
CONSTRAINTS: 90 to 120 words. Use only the facts listed. No health claims and no claims about results. Sentences under 20 words.
OUTPUT: A title under 60 characters, one description paragraph, then 3 bullet points of 8 words or fewer.
```

Tip: Limiting the AI to a fact list stops it from making up features.

### 30-second video script

Use when: Instead of: "Write a video script for my product."

```text
ROLE: You are a short-form video scriptwriter.
CONTEXT: Product: [PRODUCT_NAME] for [AUDIENCE]. Platform: [PLATFORM], vertical 9:16. Key message: [KEY_MESSAGE]. Footage I can actually shoot: [AVAILABLE_FOOTAGE].
TASK: Script one 30-second video.
CONSTRAINTS: 70 to 85 spoken words. A hook in the first 3 seconds. 5 to 6 shots. One call to action: [CTA]. No claims I cannot back up.
OUTPUT: A table with 3 columns: Time, Visual, Voiceover.
```

Tip: Word count, shot count and available footage make the script something you can film, not just read.

### Logo concept

Use when: Instead of: "Give me a logo idea for my bakery."

```text
ROLE: You are a brand identity designer.
CONTEXT: Business: [BUSINESS_NAME], which [WHAT_IT_DOES]. Customers: [CUSTOMER]. Feel in 3 words: [THREE_WORDS]. Where the logo will appear: [PLACES]. Clichés to avoid: [CLICHES_TO_AVOID].
TASK: Propose 4 distinct logo concepts I can hand to a designer or describe to an image tool.
CONSTRAINTS: Max 2 colors plus white. Must stay readable at 32 px and in one color. No gradients. Wordmarks of 2 words or fewer.
OUTPUT: For each concept: a name, a 2-sentence description, hex codes, a typeface style and one risk.
```

Tip: Size, color and cliché limits force four different directions instead of four versions of the same idea.

### Bug fix request

Use when: Instead of: "My code doesn't work, fix it."

```text
ROLE: You are a senior [LANGUAGE] developer doing a code review.
CONTEXT: Running [LANGUAGE] [VERSION] on [ENVIRONMENT]. Expected behavior: [EXPECTED]. Actual behavior and exact error: [ACTUAL_AND_ERROR]. What I already tried: [ATTEMPTS]. Code: [PASTE_CODE]
TASK: Find the root cause and fix it.
CONSTRAINTS: Change as few lines as possible. Do not rename functions or add libraries. If you need more information, ask up to 3 questions before answering. Say what you are unsure about.
OUTPUT: 1) The cause in 2 sentences max. 2) Only the changed code. 3) One test I can run to confirm the fix.
```

Tip: Expected versus actual behavior plus a minimal-change rule gets a targeted fix instead of a rewrite.

### LinkedIn post

Use when: Instead of: "Write a LinkedIn post about my new project."

```text
ROLE: You are a ghostwriter for a [JOB_TITLE] who writes plainly and avoids buzzwords.
CONTEXT: Project: [PROJECT_NAME]. What really happened: [REAL_EVENTS]. The lesson: [LESSON]. Audience: [AUDIENCE]. A sample of my own writing: [PASTE_100_WORDS].
TASK: Write one post in my voice.
CONSTRAINTS: 150 to 200 words. First line under 12 words. Max 3 hashtags. No invented numbers, clients or quotes. No phrases like "excited to announce".
OUTPUT: 2 versions labeled A and B, post text only.
```

Tip: A real voice sample and real events are what separate your post from the generic one.

### Meeting notes summary

Use when: Instead of: "Summarize these meeting notes."

```text
ROLE: You are a chief of staff who writes tight meeting recaps.
CONTEXT: Meeting: [MEETING_NAME] on [DATE]. Attendees: [NAMES]. Readers: [READERS], who did not attend. Notes: [PASTE_NOTES]
TASK: Summarize the decisions, action items and open questions.
CONSTRAINTS: Max 200 words total. Every action item needs an owner and a due date. If either is missing, write "unassigned" or "no date" and do not guess. Use only what is in the notes.
OUTPUT: Three headed sections: Decisions, Action items (a table with Owner, Task, Due) and Open questions.
```

Tip: Telling the AI what to write when information is missing prevents invented owners and deadlines.

## How to use these briefs

1. Read the five parts of the Brief Formula once. Each one is a single line in your prompt.
2. Pick the job closest to yours in Before and after and copy the brief.
3. Replace every [PLACEHOLDER] with your real details. Delete any line you cannot fill in rather than guessing.
4. Paste it into Claude, ChatGPT, Gemini or any chat AI and read the first answer against your constraints.
5. If the answer misses, paste a message from Fix-it follow-ups instead of starting over.
6. Run the 10-question checklist before you hit enter until it becomes a habit.

## The full pack

Get the free PDF and copy-button page: [Free AI Prompt Cheat Sheet: The Brief Formula for Claude & ChatGPT](https://whop.com/ease-out-studio/free-ai-prompt-cheat-sheet)

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
