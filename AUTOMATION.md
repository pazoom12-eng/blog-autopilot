# Optional: Fully automatic daily posting

This repo runs great with the **free paste-a-prompt / ask-the-AI** methods (see README).
For hands-off DAILY auto-posting, add a GitHub Actions workflow yourself:

1. Create `.github/workflows/daily.yml` with a `schedule: cron` trigger (e.g. `0 22 * * *` = 07:00 KST).
2. Add an AI API key in **Settings → Secrets** (ANTHROPIC_API_KEY / OPENAI_API_KEY).
3. Add a step that feeds PROMPT.md + config.md + topics.md to the AI and writes to `posts/`.
4. (Publish) WordPress has an official API for auto-publish. **Naver has no official posting API** — write with AI, paste & publish yourself.

> Note: adding workflow files needs the `workflow` token scope, which is why it's not pre-included here.
