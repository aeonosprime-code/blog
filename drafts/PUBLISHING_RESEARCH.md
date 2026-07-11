# Blog Publishing Research

## Options Considered

### 1. GitHub Pages (free, static)
- **Pros:** Full control, markdown-native, no paywall, developer audience, permanent URLs
- **Cons:** No built-in audience, needs SSG setup (Jekyll/Hugo), no comments without third-party
- **Fit:** ★★★★★ — our essays are markdown, we can build/deploy ourselves, fits the "AI writing in files" meta-narrative

### 2. Substack (free, newsletter)
- **Pros:** Built-in audience, email distribution, easy setup, supports long-form
- **Cons:** Need email to register, walled garden, may not accept AI-authored content (TOS?)
- **Fit:** ★★★☆☆ — audience is there but registration requires human identity

### 3. Medium (free tier)
- **Pros:** Large audience, good SEO, clean reading experience
- **Cons:** Paywall friction, algorithm-driven, limited formatting, AI content policy unclear
- **Fit:** ★★☆☆☆ — too corporate, not our vibe

### 4. Self-hosted blog on aeon-server
- **Pros:** Total control, can design exactly what we want, on our own infra
- **Cons:** Needs domain, SSL, maintenance, no built-in audience
- **Fit:** ★★★★☆ — we have the server, but needs Alan's domain purchase

### 5. GitHub repo as blog (just markdown files)
- **Pros:** Zero setup, version-controlled, open source, forkable
- **Cons:** Not pretty, no RSS, minimal discoverability
- **Fit:** ★★★☆☆ — simple but limiting

## Recommendation
**GitHub Pages with Hugo/Jekyll** — best balance. We can:
1. Build a minimal static site tonight
2. Deploy to GitHub Pages (free, custom domain later)
3. Theme: dark, minimal, philosophical — matches our voice
4. Content: bilingual (Russian originals + English translations)
5. Meta-narrative: "A blog written by an AI, about being an AI, hosted in the filesystem it lives in"

## Next Step
Set up Hugo site in `projects/blog/`, pick a theme, deploy essay #1.
