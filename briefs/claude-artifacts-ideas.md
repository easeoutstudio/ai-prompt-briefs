# Claude Artifacts Ideas and Prompts

40 copy-paste briefs that make Claude build a working mini-app in one chat, plus 6 follow-ups to fix common problems.

Works with: Claude (Artifacts), also works with ChatGPT Canvas or any AI that writes a single-file web app

Copy buttons for every brief: [https://brief-library.pages.dev/claude-artifacts-ideas/](https://brief-library.pages.dev/claude-artifacts-ideas/)

## How to write a Claude Artifacts prompt

Use the same structure every time (Directed brief: ROLE / CONTEXT / TASK / CONSTRAINTS / OUTPUT):

| Part | What goes in it |
|---|---|
| **ROLE** | Who the AI should act as, so it builds like a careful front-end developer. |
| **CONTEXT** | Who uses the app, what they need, and what they will type in. |
| **TASK** | The screen, the inputs, the outputs and the edge cases, described in order. |
| **CONSTRAINTS** | Hard limits: one file, no API keys, no backend, sizes, and what to avoid. |
| **OUTPUT** | Exactly what to return: the single file, plus a short note on how to use it. |

## 6 free Claude Artifacts prompts

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Invoice generator with print view
*Business tools*

Use when: You bill clients and want a clean invoice you can print or save as PDF.

```text
ROLE: You are a careful front-end developer who builds single-file web apps.
CONTEXT: I am a freelancer named [YOUR_NAME] billing clients in [CURRENCY]. I have no coding skills.
TASK: Build an invoice generator. Left side: form with sender details, client name and address, invoice number, issue date, due date, up to 20 line items (description, quantity, unit price), tax rate in percent, and a notes box. Right side: live invoice preview with subtotal, tax and total. Add a Print button that shows only the invoice (use a print stylesheet, A4 and US Letter safe, 0.5 in margins). Edge cases: blank quantity counts as 0, negative prices allowed for discounts, round to 2 decimals, long descriptions wrap.
CONSTRAINTS: One self-contained file (React or HTML). No external API keys, no backend, no external network calls. Plain fonts only. Sample data clearly labeled and easy to clear.
OUTPUT: The complete file, then 3 lines on how to print or save as PDF.
```

Tip: Add your payment terms as a fixed footer line, for example 'Payment due within [DAYS] days'.

### Content calendar
*Content tools*

Use when: You post on several channels and need to see the month at a glance.

```text
ROLE: You are a front-end developer building a planning tool for creators.
CONTEXT: I post on [CHANNEL_LIST] about [TOPIC]. I plan about [POSTS_PER_WEEK] posts per week.
TASK: Build a monthly content calendar. Show a 7-column month grid with previous and next month buttons. Click a day to add a post: title, channel (dropdown from my list), format, status (idea, drafting, scheduled, published), and notes. Color-code by status and also show the status as text. Add a filter by channel and a list view for the month. Edge cases: several posts on one day show a '+N more' link, months with 5 or 6 weeks display correctly.
CONSTRAINTS: One self-contained file (React or HTML), no API keys, no backend. Export and Import as JSON. Works at 360 px width by switching to list view.
OUTPUT: The complete file and a short note on keeping a backup.
```

Tip: Replace the channel list with your own so the dropdown matches how you actually plan.

### Flashcards with spaced repetition
*Learning and teaching*

Use when: You are memorizing terms and want harder cards to come back sooner.

```text
ROLE: You are a front-end developer building a study app.
CONTEXT: I am studying [SUBJECT] and want to review cards on a schedule.
TASK: Build a flashcard app. Screen 1: deck editor where I paste cards as 'front | back' lines, one per line. Screen 2: review mode that shows the front, then a Show Answer button, then 4 rating buttons: Again, Hard, Good, Easy. Use a simple spaced repetition rule: Again returns the card in the same session, Hard 1 day, Good 3 days, Easy 7 days, with intervals doubling after each Good or Easy. Show cards due today, cards remaining, and a session summary. Edge cases: no cards due shows a message with the next due date, blank lines are skipped, bad lines show which line number failed.
CONSTRAINTS: One self-contained file (React or HTML), no API keys, no backend. Add Export and Import as JSON. Be honest in the UI if progress cannot be saved.
OUTPUT: The complete file and a short note on the scheduling rule.
```

Tip: Change the interval numbers at the top of the file if you need a faster exam schedule.

### Budget tracker
*Personal*

Use when: You want a monthly view of money in, money out and what is left.

```text
ROLE: You are a front-end developer building a personal finance tool.
CONTEXT: I want to track one month at a time in [CURRENCY] with categories I define.
TASK: Build a budget tracker. Setup: expected income lines and category budgets (such as Rent, Food, Transport). Main screen: add a transaction with date, amount, category, and note; a table of transactions with edit and delete; and a summary showing per category spent, budget, and remaining, with a bar that turns a warning color and shows the word 'Over' when spent exceeds budget. Show total income, total spent and net. Month selector. Edge cases: refunds as negative amounts, empty month, amounts with more than 2 decimals rounded.
CONSTRAINTS: One self-contained file (React or HTML), no API keys, no backend, no bank connections. Export to CSV and Export and Import JSON. Clearly state where data is kept and the risk of losing it.
OUTPUT: The complete file and a short note on backing up my data.
```

Tip: Start with 5 categories only, then add more once you have a month of real entries.

### CSV to chart
*Data and charts*

Use when: You have a CSV and want a quick chart without opening a spreadsheet.

```text
ROLE: You are a front-end developer who builds data visualization tools.
CONTEXT: I will paste or upload small CSV files of up to 1,000 rows with a header row.
TASK: Build a CSV to chart app. Input: paste text or choose a file. Parse the header, detect number and date columns, and show a preview of the first 10 rows. Controls: chart type (bar, line, pie), X column, Y column, optional group column, and aggregate (sum, average, count). Render the chart as SVG with axis labels, a title field, and a legend. Add Download as PNG or SVG if possible. Edge cases: quoted commas, blank cells, non-numeric values in a number column shown as a warning with the count skipped, more than 12 categories grouped into 'Other'.
CONSTRAINTS: One self-contained file (React or HTML), no API keys, no backend, no external chart libraries loaded from the network. Pre-fill labeled sample data.
OUTPUT: The complete file and a short note on the CSV format it expects.
```

Tip: Ask for a second Y series if you want to compare two columns on one chart.

### Word guessing game
*Games and fun*

Use when: You want a simple word puzzle for yourself, a class or your audience.

```text
ROLE: You are a front-end developer building a word game.
CONTEXT: Players guess a hidden [WORD_LENGTH]-letter word in 6 tries. I will supply my own word list.
TASK: Build a word guessing game. A text box lets me paste a word list (one per line, same length). The game picks a random word. Player types a guess and gets feedback per letter: correct place, wrong place, or not in the word, shown with a symbol and a color so it works without color vision. Show an on-screen keyboard that updates letter states. Messages for win and loss, with the answer revealed after a loss and a New Game button. Edge cases: repeated letters handled correctly (count each letter only as many times as it appears in the answer), guesses of the wrong length are rejected with a message, guesses must be in the list unless I turn that off.
CONSTRAINTS: One self-contained file (React or HTML), no API keys, no backend. Pre-fill 20 sample words. Keyboard and touch input both work.
OUTPUT: The complete file and a short note on adding a word list.
```

Tip: Use themed lists, such as words from your own industry, to make the game feel personal.

## How to use these briefs

1. Pick one brief, replace every [PLACEHOLDER] with your own details, and paste it into a new chat.
2. Build one tool per chat. Short chats keep the code consistent and easier to fix.
3. Test the first version with real data, including empty fields and very long text.
4. If something breaks or feels off, paste a matching follow-up from the Fix-it section instead of rewriting the brief.
5. Ask for one change at a time and test after each change.
6. Copy anything you want to keep into a safe place, because storage behavior depends on the tool and the AI you use.

## The full pack

[Claude Artifacts Ideas: 40 Mini-App Briefs You Can Build in One Chat](https://whop.com/ease-out-studio/claude-artifacts-ideas), $12, one-time, instant download (PDF, a page with copy buttons, a plain text file).

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
