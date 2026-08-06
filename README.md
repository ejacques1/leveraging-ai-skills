# Custom AI Assistant

Stop building custom GPTs you don't own.

This is a free skill for [Claude Code](https://claude.com/claude-code). Run it, answer five
questions, and it builds you a real AI assistant as a web app — your instructions, your knowledge,
your domain, your customers. Optionally behind a login and a Stripe paywall.

Nothing is held back. The paywall step is included.

---

## Install

Open Claude Code and paste these two lines, one at a time:

```
/plugin marketplace add ejacques1/leveraging-ai-skills
```

```
/plugin install leveraging-ai@leveraging-ai-skills
```

That's it. No terminal, no downloads, no folders to find.

Then just say:

> build me a custom AI assistant

It asks you five questions, then builds the whole thing.

<details>
<summary>If the install says "Run /reload-plugins to activate"</summary>

Run `/reload-plugins` and you're set.
</details>

<details>
<summary>Manual install instead</summary>

```bash
git clone https://github.com/ejacques1/leveraging-ai-skills.git /tmp/lai
mkdir -p ~/.claude/skills
cp -r /tmp/lai/plugins/leveraging-ai/skills/build-assistant ~/.claude/skills/
```
</details>

---

## What you get

- A chat app (Next.js + TypeScript) running on Claude Opus 5
- **`assistant-instructions.md`** — the brain. Edit that one file, the assistant changes.
- **`/knowledge`** — drop in your documents; they load into every conversation
- Streaming replies, markdown and tables, light and dark mode
- Web search, so it answers with current information instead of stale training data
- Prompt caching, so repeat messages cost roughly a tenth as much
- Ready to deploy to Vercel on your own domain
- Optional: Supabase login + Stripe subscription, members only

## What you need

- [Claude Code](https://claude.com/claude-code)
- An [Anthropic API key](https://console.anthropic.com) — you pay Anthropic per message
- A free [Vercel](https://vercel.com) account to put it online
- No coding experience. You'll copy a key and click Deploy.

---

## The honest part

The build works. The **deploy** is where people get stuck — API keys, environment variables,
knowing which button to press on Vercel. That's not a knowledge gap you should feel bad about.
It's just the part nobody explains.

If you hit a wall, or you want help taking it further — adding the paywall, getting it in front
of customers, building something bigger — that's what I do inside my community.

**→ https://www.skool.com/leveragingai/about**

It's where you build AI-powered web apps that people subscribe to. Bring your error message.

— Dr. Erin Jacques

---

## License

MIT. Use it, fork it, ship it, sell what you build with it.
