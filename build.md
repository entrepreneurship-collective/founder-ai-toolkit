# Build Your MVP with AI

Prices and limits last checked: November 2026. They change often, so confirm on each tool's site.

You can build a working app without writing code: describe it, and an AI app builder makes it. Free plans are small, so plan first and build second.

---

## Pick a builder

| Builder | Free plan | Live link | Database and login | Export code | Best for |
|---|---|---|---|---|---|
| [Google AI Studio](https://aistudio.google.com) (Build mode) | Modest quota; Google doesn't publish numbers | Up to 2 live apps (personal accounts) | Yes | GitHub or ZIP | Best free choice |
| [Lovable](https://lovable.dev) | 5 credits a day (30 a month) | Yes | Yes | GitHub | Most polished apps |
| [Bolt](https://bolt.new) | 1M tokens a month (300K a day) | Yes | Yes | GitHub or ZIP | Most room per day |
| [Base44](https://base44.com) | 25 message credits a month | Yes | Yes | Builder plan and up | Simplest app with logins |
| [Replit](https://replit.com) | Daily Agent credits ("Lite" builds only) | 1 app, offline after 30 days | Yes | GitHub | Apps that need a real backend |
| [Gamma](https://gamma.app) | 400 credits, one time | Yes | No | No | Landing page or pitch deck |

- **Google AI Studio privacy:** on the free plan, Google may have people review what you type. Don't paste secrets.
- **Business website:** [Wix](https://www.wix.com) and [Framer](https://www.framer.com) both have free plans with AI site builders.
- **Quick clickable mockup:** ask [Gemini](https://gemini.google.com) to build it in Canvas, or [Claude](https://claude.ai) to build it as an Artifact, then share the public link. Both work on free plans. In Gemini, add your Gemini Notebook as a source first, so the mockup draws on your research. Anyone with a Gemini Canvas link can see and edit the app's data, so use sample data.
- **Ready to pay?** Entry plans cost about $20 to $25 a month (Lovable Pro, Bolt Pro, Base44 Starter, Replit Core). Replit Core unlocks full builds and unlimited live apps. Pay for one month, then cancel if you don't need more.

---

## Plan first: write a spec

Before you open a builder, ask a chat assistant (Claude, ChatGPT or Gemini) to turn your Lean Canvas into a one-page spec: the screens, what a user can do, the data to save, and what to leave out. The [prompt pack](prompts.md#3-app-spec) has the prompt and template. The same spec works in any builder:

- **Browser builders** (Google AI Studio, Lovable, Bolt, Base44): paste the spec as your first message.
- **Desktop coding agents** ([Google Antigravity](https://antigravity.google/), [Claude Code](https://claude.com/product/claude-code)): save it as spec.md in your project folder and ask the agent to read it.

When you change your mind about the app, update the spec too, so the next tool always gets the latest version.

---

## Make free credits last

1. **Send one big first prompt, then one change per prompt.** Be specific ("move the Sign Up button under the form"), not vague ("make it better").
2. **Avoid fix-loops.** If a bug survives 2 attempts, roll back to the last working version and describe what you see instead.
3. **Think in chat mode.** Where a builder has a separate chat or plan mode (Lovable does), use it to think, then build.
4. **Fake what you don't need.** For a demo, use sample data and skip payments, emails and admin screens.

**When credits run out:** paste your spec into another builder, export your code (Google AI Studio and Lovable) and continue elsewhere, wait for the daily reset, or pay for one month.

---

## Build on your desktop

Google Antigravity is a free desktop app for Windows, Mac and Linux. Its AI agent builds your app, runs it and tests it in a browser. Sign in with a personal Google account (you must be 18+). The free plan uses Gemini 3.8 Flash with a weekly limit that Google doesn't publish.

To keep building a prototype, in Google AI Studio choose Export, then Export to Antigravity.

- **Backups:** [GitHub Copilot Free](https://github.com/features/copilot/plans) in [VS Code](https://code.visualstudio.com/), or [Codex](https://chatgpt.com/codex/) in the ChatGPT desktop app (limited on the free plan).
- **Paid upgrades:** Google AI Pro ($19.99 a month) raises Antigravity's limits. Claude Pro ($20 a month) includes Claude Code. ChatGPT Plus ($20 a month) gives much more Codex use.
- **Terminal tools are optional.** Everything else in this guide works without typing commands.

---

## Spend about $10 for more choice

[OpenRouter](https://openrouter.ai/) gives you one account and one bill for hundreds of AI models.

- **Cost:** on cheap models such as Claude Haiku 5.5, GPT-6 Luna, DeepSeek V4.1 Flash or MiniMax M3, a full day of research and app building costs about $1 to $3. With fees, tax and exchange, $10 USD costs about C$15 to C$17. Save stronger models such as Claude Sonnet 5.5 for a few hard fixes.
- **Use cheap paid models, not free ones.** Free models change often, hit rate limits when busy, and some train on your prompts.

Setup (about 20 minutes):

1. Create an OpenRouter account and buy $10 of credit.
2. In privacy settings, turn off training for paid models.
3. Create an API key with a $5 limit, and keep it in a password manager.
4. Install [Dyad](https://www.dyad.sh/), a free desktop app builder with a live preview. If it asks for Node.js, let it install it.
5. In Dyad, go to Settings, then Model Providers, then OpenRouter, and paste your key.
6. For research, use [OpenRouter Chat](https://openrouter.ai/chat) in your browser with web search on.

If Dyad won't install, try [Goose](https://goose-docs.ai/) Desktop. If you're comfortable typing commands in a terminal, [OpenCode](https://opencode.ai/), [Pi](https://pi.dev/) and [Hermes Agent](https://hermes-agent.nousresearch.com/docs/) also work with your OpenRouter key.
