# Prompt Pack

Copy-paste prompts for each step, from research to a working app. Each prompt asks the AI for a markdown file: plain text with simple headings that every AI tool can read. Save each file, then paste it into the next step, so every tool works from the same facts.

| Prompt | Use in | You get |
|---|---|---|
| [1. Research brief](#1-research-brief) | [Gemini](https://gemini.google.com) Deep Research | research-brief.md |
| [2. Lean Canvas](#2-lean-canvas) | [Claude](https://claude.ai) or [ChatGPT](https://chatgpt.com) | lean-canvas.md |
| [3. App spec](#3-app-spec) | Claude or ChatGPT | spec.md |
| [4. Build](#4-build) | Any app builder or coding agent | A working app |
| [5. Pitch deck](#5-pitch-deck) | Claude or ChatGPT, then [Gamma](https://gamma.app) | pitch-deck.md |
| [6. Interview guide](#6-interview-guide) | Claude or ChatGPT | interview-guide.md |

**How to use them:**

- Fill in the [brackets] before you send. Where a prompt says [paste ...], open that file, copy everything and paste it there.
- Keep the lines asking for links and "unknown". They cut down on made-up facts.
- **Save each answer as a file.** Click the copy button under the answer, paste it into a plain text editor (Notepad on Windows, or TextEdit on Mac after Format > Make Plain Text), and save it with the name shown. Keep all your files in one folder.
- When your plans change, update the file, so the next tool always gets the latest version.

---

## 1. Research brief

Free deep research runs are limited, so fill in every bracket before you send. If Gemini is out of runs, use ChatGPT's deep research.

```
Research this startup idea and write a research brief.

My idea: [one sentence]
Target customer: [who]
Where: [city, province], Canada

Answer these questions:
1. Customer and problem: who has this problem, how often, and what it costs them today in time or money.
2. Competitors: 8 to 10, including indirect ones (what people use today instead, even spreadsheets or doing nothing), with what each one charges.
3. Market size: how many potential customers there are in [region], from official sources such as Statistics Canada.
4. Trends and rules: what is changing in this market, and any licences or regulations that apply.

Rules:
- Give a link for every fact and number. If you can't find a source, write "unknown". Don't guess.
- Only include companies with a working website. Say whether each price is in CAD or USD.
- Write the brief in markdown, under 1,500 words, using exactly these headings:

# Research brief: [idea]
## Summary
(5 bullets)
## Customer and problem
## Competitors
(table: name, website, what they offer, who they target, price, strengths, common complaints from reviews)
## Market size
## Trends and rules
## Gaps my idea could fill
(3 bullets)
## Open questions
(what I still need to ask real customers)
## Sources
```

Check the key facts before you build on them. The [research guide](research.md#check-before-you-trust) shows how.

---

## 2. Lean Canvas

```
Using my research brief below, fill in a Lean Canvas for my idea.

Rules:
- Use the 9 boxes as headings, in this order: Problem, Customer Segments, Unique Value Proposition, Solution, Channels, Revenue Streams, Cost Structure, Key Metrics, Unfair Advantage.
- Problem: list the top 3 problems. Customer Segments: include early adopters.
- Write 1 to 3 short bullets per box. Label each bullet FACT (backed by the brief) or ASSUMPTION (needs testing).
- End with a "Riskiest assumptions" heading: my 3 riskiest assumptions, and a cheap way to test each one in the next 2 weeks.
- Reply in markdown with only the canvas, starting with "# Lean Canvas: [idea]".

[paste research-brief.md]
```

For the classic one-page layout, copy the boxes into a Lean Canvas template such as [Miro's](https://miro.com/templates/lean-canvas/).

---

## 3. App spec

The spec uses the same plain headings every time, so any builder can follow it. You don't fill in the template; the AI does.

```
Write a spec for the first version of my app, using my Lean Canvas and research brief below. An AI app builder or coding agent will build the app from it.

Rules:
- Keep only what the first version needs to show the idea working: 3 to 5 screens and 5 to 8 things a user can do.
- Use plain language. Don't name programming languages, frameworks or databases; the builder chooses those.
- Use exactly the headings in the template, in the same order. Keep it to one page.
- Reply in markdown with only the spec.

Template:

# App name

## Summary
(2 to 3 sentences: what the app does, who it is for, and the problem it solves)

## Users
- Type of user: what they come to do

## Screens
1. Screen name: what it shows and what a user can do there

## What a user can do
- A user can ...

## Data to save
- Thing: details to save (for example name, email, booking date)

## Login
(No login, email and password, or Google sign-in. Who can see what.)

## Look and feel
(Style, colours and tone, for example clean, friendly, blue and white. Works on phones and computers.)

## Sample data
(5 to 10 realistic examples, so the first version doesn't look empty)

## Leave out for now
- (For example payments, emails, admin screens)

My Lean Canvas:
[paste lean-canvas.md]

My research brief:
[paste research-brief.md]
```

Read the spec before you build. Cut anything the first version doesn't need: every extra screen costs builder credits.

---

## 4. Build

In a browser builder such as [Lovable](https://lovable.dev) or [Google AI Studio](https://aistudio.google.com), send this as your first message. In a desktop coding agent such as [Google Antigravity](https://antigravity.google/) or [Claude Code](https://claude.com/product/claude-code), save spec.md in your project folder and replace the last line with "Read spec.md in this folder."

```
Build the first version of the app described in the spec below.
- Follow the spec. Don't add anything it doesn't list.
- Start with the main screen and the most important thing a user can do, then add the rest.
- Load the sample data so every screen has something to show.
- Make it work on phones and computers.
- When you finish, tell me what works, what doesn't work yet, and any choices you made that the spec didn't cover.

[paste spec.md]
```

**When something breaks:**

```
Something isn't working. Fix only this problem and don't change anything else.
What I did: [the steps, for example "clicked Book on the home screen"]
What I expected: [what should happen]
What happened: [what you saw, with any error message copied word for word]
```

If it's still broken after 2 tries, roll back to the last working version. The [build guide](build.md#make-free-credits-last) has more ways to make credits last.

---

## 5. Pitch deck

```
Turn my Lean Canvas and research brief below into a 10-slide pitch deck outline: Problem, Solution, Why now, Market size, Product, Business model, Competition, Go-to-market, Team, Ask.

My team: [names, with one line about each person]

Rules:
- Give each slide a heading such as "## Slide 1: Problem", up to 25 words of slide text, and a "Notes:" line with what to say.
- Use only facts and numbers from my files. Don't add any I didn't give you.
- Reply in markdown with only the outline, starting with "# Pitch deck: [idea]".

[paste lean-canvas.md]

[paste research-brief.md]
```

Paste the outline into Gamma to design the slides, then edit them by hand.

---

## 6. Interview guide

```
Write a customer interview guide that tests the riskiest assumptions in my Lean Canvas below.

Rules:
- Follow "The Mom Test": ask about past behaviour and real examples, not opinions about my idea. Don't pitch my idea. No leading questions.
- Include a short intro, 8 to 10 open questions, follow-ups such as "Tell me about the last time that happened", and 3 questions about what they spend on this problem today (time or money).
- Add a 5-question screener survey to find the right people to interview.
- Reply in markdown with only the guide, starting with "# Interview guide: [idea]".

[paste lean-canvas.md]
```

Put the screener in [Tally](https://tally.so) or [Google Forms](https://forms.google.com). After 5 or more interviews, add your notes to [Gemini Notebook](https://notebook.google.com) and ask: "Which problems came up most often? Quote the people who said them." Then update lean-canvas.md: change each ASSUMPTION that interviews confirmed to FACT, and run prompt 3 again if the app needs to change.

---

## More prompts

**Customer personas**
```
Create 3 customer personas for [idea], for [target customer] in [Ontario/Canada].
For each: name, role and situation, their problem in their own words, what they use today, what would make them switch, where they spend time online, and who makes the buying decision.
These are guesses to test, so add 3 questions I should ask real people to check each persona. Do not invent statistics.
Reply in markdown.
[paste research-brief.md, or real quotes from reviews, Reddit or interviews]
```

**Market size (TAM, SAM, SOM)**
```
Help me estimate TAM, SAM and SOM for [idea] in [Canada/Ontario] using a bottom-up method (number of customers x price per year), not a top-down "the industry is worth $X billion" number.
1) Tell me exactly which public data I need and where to find it. Prefer Statistics Canada, Government of Canada and other official sources.
2) Show the formula for TAM, SAM and SOM, using placeholders for [number of potential customers] and [price per customer per year].
3) List every assumption separately so I can change it.
Give a link for every number. If you cannot find a source, write "not found". Reply in markdown.
```

**Pricing**
```
I want to price [product/service] for [target customer] in Canada.
1) Find what 5 to 8 similar products charge. Give the link to each pricing page and say if the price is in USD or CAD. If a price is not public, write "not public". Do not guess.
2) Suggest 2 or 3 pricing models that fit (for example monthly subscription, per use, one-time fee), with pros and cons.
3) Write the 4 standard Van Westendorp price questions so I can put them in a survey.
Reply in markdown.
```
