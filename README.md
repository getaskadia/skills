# Askadia skill

[Askadia](https://askadia.ai) shows whether ChatGPT recommends your product when buyers ask what to buy: the
questions, ChatGPT's answers word for word, who it recommends instead, and the pages it reads. This skill lets your
agent (Claude Code, Codex, Cursor and others) use it: read how you're doing, find where you lose and why, review the
questions you track, and make changes when you say so.

## Install

Any agent that reads skills:

```bash
npx skills add getaskadia/skills
```

Claude Code, as a plugin:

```
/plugin marketplace add getaskadia/skills
/plugin install askadia@askadia
```

Then ask your agent how your product is doing in ChatGPT. The first time, it shows you a link to approve its access
to your Askadia account.

## How it works

The skill is a pointer: each time it's used, it reads the current instructions at
[askadia.ai/docs/api.md](https://askadia.ai/docs/api.md), so it doesn't go stale as Askadia gains features.
