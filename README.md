# Viral Outliers agent skills

A Hermes Agent "tap" (and a plain skills repo for any agent that reads `skills/<name>/SKILL.md`).

## Viral Outliers

Find viral outlier posts on TikTok, Instagram and YouTube, pull creator stats, transcribe and analyse videos, build competitor watchlists, and crawl profiles on demand. Prepaid credits, MCP or REST. Docs: https://viraloutliers.com/docs

### Install

Hermes Agent:

```
hermes skills tap add Viral-Outliers/agent-skills
hermes skills install viral-outliers
```

OpenClaw (published on ClawHub):

```
openclaw skills install @MatsClaes2/viral-outliers
```

Claude Code, Cursor, Codex and other agents that support the open Agent Skills standard (via Vercel's skills CLI):

```
npx skills add Viral-Outliers/agent-skills
```

Also discoverable via https://viraloutliers.com/.well-known/skills/index.json (agent-skills discovery).

You need a Viral Outliers API key in `VIRAL_OUTLIERS_API_KEY` (create one at https://viraloutliers.com/settings?tab=api-keys). The free trending and pricing endpoints work without one.

## Layout

```
skills/
  viral-outliers/
    SKILL.md
    references/
      skills.md
      getting-started.md
```

The skill files are generated from the Viral Outliers API registry (never hand-edited); this repo mirrors the published bundle.
