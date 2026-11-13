# Claude Code Prompts

50 copy-paste briefs for Claude Code, Cursor and other coding agents, plus 6 guardrail messages for when the agent drifts.

Works with: Claude Code, Cursor, Codex CLI, Windsurf or any coding agent

Copy buttons for every brief: [https://brief-library.pages.dev/claude-code-prompts/](https://brief-library.pages.dev/claude-code-prompts/)

## How to write a Claude Code prompt

Use the same structure every time (ROLE / CONTEXT / TASK / CONSTRAINTS / OUTPUT):

| Part | What goes in it |
|---|---|
| **ROLE** | Who the agent acts as, so it picks the right habits and level of care. |
| **CONTEXT** | Your stack, files, commands and the facts it cannot guess. |
| **TASK** | The one job to finish, with a clear definition of done. |
| **CONSTRAINTS** | Read files first, keep changes minimal, leave unrelated code alone, plus task-specific limits. |
| **OUTPUT** | Run tests or the build, then report what changed and what is left. |

## 7 free Claude Code prompts

Copy a brief, replace every [PLACEHOLDER] with your details and paste it into your AI tool.

### Map an unfamiliar repo
*Start and plan*

Use when: You joined or inherited a codebase and need a working mental model fast.

```text
ROLE: Senior engineer onboarding to a new codebase.
CONTEXT: Repo root is [REPO_PATH]. Main language and framework: [STACK]. I need to work on [AREA_OF_INTEREST].
TASK: Map the repo. Identify entry points, folder layout, data flow for [AREA_OF_INTEREST], key dependencies, and how to run, test and build it.
CONSTRAINTS: Read the README, package or build files, and config first. Do not modify any file. Do not guess: mark anything you could not verify as UNCLEAR. Keep the map under 400 words.
OUTPUT: Run [TEST_COMMAND] and [BUILD_COMMAND] and report whether they pass. Then give: 1) folder map, 2) request or data flow in 6 steps or fewer, 3) risky areas, 4) five questions you still have, 5) what is left unexplored.
```

Tip: Set [AREA_OF_INTEREST] narrowly, such as billing or the job queue, to get a sharper map.

### CRUD endpoint
*Build features*

Use when: You need create, read, update and delete for a new resource.

```text
ROLE: Backend engineer who matches existing patterns.
CONTEXT: Stack [STACK]. Resource: [RESOURCE_NAME] with fields [FIELDS]. Closest existing endpoint to copy: [EXISTING_ENDPOINT_FILE]. Auth rule: [AUTH_RULE].
TASK: Add CRUD endpoints for [RESOURCE_NAME] with validation, correct status codes, and tests for success and failure cases.
CONSTRAINTS: Read [EXISTING_ENDPOINT_FILE] and the data layer first and follow their style. Keep changes minimal. Do not touch unrelated code or change existing endpoints. Validate all input. Return consistent error shapes. Add a migration only if the schema needs it.
OUTPUT: Run [TEST_COMMAND] and [BUILD_COMMAND]. Report files changed, routes added with example requests, and what is left.
```

Tip: Name the endpoint to copy so the agent mirrors your naming and error format.

### Reproduce from a stack trace
*Debug*

Use when: You have an error trace but no clear steps to trigger it.

```text
ROLE: Debugging engineer who proves the cause before fixing.
CONTEXT: Stack [STACK]. Stack trace:
[STACK_TRACE]
What the user was doing: [USER_ACTION]. Version or commit: [COMMIT].
TASK: Locate the failing code, explain the cause in plain words, write a minimal reproduction (a failing test if possible), then fix the root cause.
CONSTRAINTS: Read every file named in the trace and their callers first. Do not fix until the failure is reproduced. Do not silence the error or add a broad try/catch. Keep changes minimal and do not touch unrelated code.
OUTPUT: Run [TEST_COMMAND] to show the new test fails before and passes after. Report cause, files changed, and what is left or uncertain.
```

Tip: Include the line numbers and the exact input if you have them.

### Extract a module
*Refactor*

Use when: A file does too many things and one part deserves its own module.

```text
ROLE: Engineer doing a behavior-preserving refactor.
CONTEXT: Stack [STACK]. Source file: [SOURCE_FILE]. Part to extract: [PART_TO_EXTRACT]. New module path: [NEW_MODULE_PATH].
TASK: Move the part into the new module with a small, clear public interface and update all imports.
CONSTRAINTS: Read the source file, its tests and all its importers first. Run [TEST_COMMAND] before changing anything to record the baseline. No behavior changes, no renames beyond the move, no style cleanup elsewhere. Keep changes minimal and do not touch unrelated code.
OUTPUT: Run [TEST_COMMAND] and [BUILD_COMMAND] again. Report files changed, the new public interface, and what is left.
```

Tip: Ask for a separate commit for the move and any follow-up cleanup.

### Add tests for existing code
*Test*

Use when: A working module has no tests.

```text
ROLE: Engineer writing tests for code they did not write.
CONTEXT: Stack [STACK]. Test framework: [TEST_FRAMEWORK]. Target: [TARGET_FILE]. Example of a good existing test: [EXAMPLE_TEST_FILE].
TASK: Write tests covering the main paths, edge cases and error cases of the target, with clear names that describe behavior.
CONSTRAINTS: Read the target, its dependencies and the example test first and match the style. Do not change the source code. If you find a bug, write the test, mark it clearly and report it instead of fixing it. Mock only external boundaries. Keep changes minimal and do not touch unrelated code.
OUTPUT: Run [TEST_COMMAND]. Report tests added, behaviors covered, suspected bugs, and what is left untested.
```

Tip: Tell it which behaviors matter most so it spends effort there first.

### Responsive fix
*UI polish*

Use when: A page breaks on phones or tablets.

```text
ROLE: Front-end engineer fixing layout at real breakpoints.
CONTEXT: Stack [STACK]. Page or component: [COMPONENT_FILE]. Broken at widths: [BROKEN_WIDTHS] px. Existing breakpoints: [BREAKPOINTS].
TASK: Fix layout at 320, 375, 768 and 1280 px widths: no horizontal scroll, readable text of at least 16 px for body copy, tap targets of at least 44 px, images that scale.
CONSTRAINTS: Read the component, its styles and the shared layout first. Use existing breakpoints and tokens. Do not redesign the desktop view. Keep changes minimal and do not touch unrelated code.
OUTPUT: Run [TEST_COMMAND] and [BUILD_COMMAND]. Report what you changed at each width, files changed, how you checked it, and what is left.
```

Tip: Attach a screenshot or describe exactly what overflows.

### Write a PR description
*Ship and hand off*

Use when: A branch is ready and the reviewer needs context.

```text
ROLE: Engineer writing for a busy reviewer.
CONTEXT: Branch [BRANCH_NAME] against [BASE_BRANCH]. Related issue: [ISSUE_LINK_OR_NOTES].
TASK: Write a PR description with: summary in 2 sentences, why, what changed grouped by area, how to test in numbered steps, risks, screenshots needed (list only), and follow-ups.
CONSTRAINTS: Read the full diff and commit messages first. Describe only what is in the diff. Do not claim tests passed unless you ran them. Do not edit code. Keep it under 250 words.
OUTPUT: Run [TEST_COMMAND] and [BUILD_COMMAND]. Give the description as plain markdown, then list anything in the diff that looks unrelated or unfinished.
```

Tip: Paste your team's PR template into CONTEXT to match it.

## How to use these briefs

1. Copy one brief, replace every [PLACEHOLDER] with real details from your repo, and paste it into your agent.
2. Name real file paths and commands. The more exact the CONTEXT, the smaller the diff.
3. For big work, run a plan brief first and approve the plan before any code is written.
4. Keep the verification line in every brief so the agent runs your tests or build before it reports.
5. Review the diff yourself. Paste a guardrail message the moment the agent goes off track.
6. Commit after each finished step so you can roll back one step at a time.

## The full pack

[Claude Code Prompts: 50 Vibe Coding Briefs for Real Projects](https://whop.com/ease-out-studio/claude-code-prompts), $15, one-time, instant download (PDF, a page with copy buttons, a plain text file).

---

Made by [Ease Out Studio](https://www.youtube.com/@easeoutstudio). Free briefs in this file: CC BY 4.0, credit Ease Out Studio with a link.
