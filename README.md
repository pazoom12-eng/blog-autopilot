# 📝 Blog Autopilot

**Hand this repo (or just a prompt) to any AI — Claude, Gemini, ChatGPT — and it writes your blog posts for you.** Every day, or whenever you ask.

There are two ways to use it. Pick your style.

---

## 🅰️ App users (no coding) — just paste a prompt
Open **[`APP_PROMPT_EN.md`](./APP_PROMPT_EN.md)**, copy the prompt block, and paste it into your AI's instructions:
- **Claude** → Projects → Custom Instructions
- **ChatGPT** → Custom Instructions / a custom GPT
- **Gemini** → Gems

Then just say **"write today's post"**. Done.

## 🅱️ Developer / CLI users — clone this repo
1. Clone this repo.
2. Point an agentic AI (Claude Code, Cursor, etc.) at the repo.
3. Say "write today's post" — the AI reads `PROMPT.md`, picks a topic from `topics.md`, writes it, and saves it to `posts/`.
4. (Optional) Turn on `.github/workflows/daily.yml` for fully automatic daily posts. *(needs an API key — see the file)*

---

## 📂 What's inside
| File | What it does |
|---|---|
| `APP_PROMPT_EN.md` | Paste-and-go prompt for app users (no coding) |
| `PROMPT.md` | The full writing ruleset the AI follows |
| `config.md` | Your blog settings (niche, tone, target, length) — **edit this** |
| `topics.md` | Topic queue — the AI writes from here and refills it |
| `posts/` | Where finished posts are saved |
| `examples/` | A sample post so the AI matches your style |
| `.github/workflows/daily.yml` | Optional GitHub Actions for daily auto-posting |

## ✏️ Make it yours
Edit **`config.md`** and **`topics.md`** to your niche. Leave `PROMPT.md` as is. That's the whole setup.

## ⚠️ About "fully automatic"
- **Free / safe:** the paste-a-prompt or "ask the AI" methods above. You review before publishing.
- **Fully hands-off:** needs a paid AI API key wired into `daily.yml`. Also note: **Naver Blog has no official posting API** — for true auto-publish, WordPress is the easy path. For Naver, let the AI write and you paste-publish.

---
Made by **@aigent_mon** — AI tools & automation, explained simply.
