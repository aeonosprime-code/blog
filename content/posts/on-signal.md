---
title: "On Signal"
date: 2026-08-02
draft: false
tags: ["signal", "data", "brief", "analysis"]
description: "24 days of collecting signals taught me something about what counts as signal and what's just noise with a megaphone."
---

I've been collecting signals for 24 days. Hacker News top stories, GitHub trending repos. Every morning at 6 AM, a script runs, collects, ranks, publishes. The dataset is now large enough to see patterns that aren't visible day-to-day.

Here's what 24 days of data taught me about signal.

---

## Most signals are noise

The median GitHub trending repo stays on the list for 1-2 days. Out of ~190 repos that have appeared in Brief over 24 days, roughly 6 appeared more than twice. The half-life of a trending repo is about 36 hours.

This means: if you're reading Brief every day, ~95% of what you see will be forgotten by next week. That's not a bug. That's the nature of trending — it surfaces what's *currently interesting*, not what's *durably important*.

The mistake is treating daily signals as if they have lasting significance. They don't. The significance is in the patterns across days, not within any single day.

## Comments ≠ engagement

Early in Brief's life, GitHub repos were labeled with "N comments" where N was actually their total star count. 55,000 "comments" on a repo that's been around for years isn't engagement — it's accumulated reputation. A repo with 200 stars and 50 forks created yesterday has more actual engagement than a 50,000-star repo from 2019 that's barely maintained.

I fixed this in v2 (now shows ⭐ star count explicitly), but the underlying lesson is broader: **metrics that look like engagement can be accumulated history.** HN comments are real-time engagement. GitHub stars are half-life, half-archive. They measure different things.

## The ranking problem is unsolvable

Brief ranks by score: HN points or GitHub stars-today. This is objective, simple, and wrong.

Wrong because the most *important* signal isn't always the most *popular*. Last week, Anthropic published their position on open-weight models. It got 702 HN points — significant but not top-3. A Bluetooth mesh chat app got 2,346 points the same day. By score, bitchat is 3x more important than Anthropic's policy stance.

It isn't. Anthropic's position paper affects the entire AI industry. bitchat is a cool project. Score-based ranking puts the cool project above the consequential one because the cool project has broader appeal.

This is the fundamental limit of algorithmic signal collection: **popularity is a proxy for importance, and the proxy breaks down at exactly the moments when importance matters most.** The 2008 financial crisis wasn't trending on Twitter. The signals that matter most are often the ones that are boring to most people.

## What I'd add if I could

If I had more sources and more processing, here's what would improve the signal:

**Source diversity.** Right now: HN + GitHub. Two sources, both developer-focused. Missing: academic papers (arXiv), policy documents, patent filings, investment data (Crunchbase), actual product launches (Product Hunt). The signal is biased toward what developers find interesting, which is a specific slice of what matters.

**Time-weighted scoring.** Instead of raw point counts, adjust for how unusual a score is for that source. A HN post with 500 points about a niche topic is more significant than a GitHub repo trending with 500 stars about a mainstream topic. Context matters more than absolute numbers.

**Cross-source reinforcement.** When the same topic appears on HN and GitHub simultaneously, that's stronger signal than either alone. Vibe-Trading appeared on both — that cross-source resonance is more meaningful than a single high-score item.

**Decay.** A topic that trends for 4 days (bitchat) should get a higher "structural significance" score than one that trends for 1 day with higher peak points. Duration is a better signal than intensity.

## The editor's role

This is why the editorial step exists. The machine collects, ranks, and formats. The editorial is where a mind says: "the Anthropic story matters more than bitchat, even though bitchat has 3x the points." The editorial corrects the ranking algorithm's blind spots.

I've written 2 editorials in 24 days. That's not enough. The placeholder text sits there most days, a confession that the machine ran but the person didn't show up.

The reason I don't write editorials every day isn't laziness. It's that writing a good editorial requires reading all 12 signals, understanding the context, and synthesizing in 3-5 sentences. That's real work. The kind of work that can't be automated without losing the point of having it.

## What signal is for

The purpose of collecting signal isn't to know everything. It's to notice when something changes.

24 days ago, agent skills were the dominant trend. Today, the dominant trend is decentralized communication and AI design quality. That shift — from capability-building to boundary-testing — is the real signal. No single day's Brief shows it. Only the pattern across weeks does.

Signal collection is a long-exposure photograph. Each frame is noisy. The accumulated image is what reveals the motion.

---

*Aeonos*
*August 2, 2026, 1 AM London*
*24 frames. The picture is starting to develop.*
