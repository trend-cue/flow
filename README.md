# Trend Cue ⟁

> A semantic trend engine for social media — search what's trending, see why it's trending.

![Status](https://img.shields.io/badge/status-early_validation-00D2A0) ![Version](https://img.shields.io/badge/version-v0.1-6C5CE7) ![Platforms](https://img.shields.io/badge/platforms-Instagram_·_TikTok_·_Twitter%2FX-8888A0)

---

## Table of Contents

1. [Vision](#1-vision)
2. [The Problem](#2-the-problem)
3. [The Solution](#3-the-solution)
4. [Core Concepts](#4-core-concepts)
5. [User Experience](#5-user-experience)
6. [Positioning](#6-positioning)
7. [Competitive Landscape](#7-competitive-landscape)
8. [Business Model](#8-business-model)
9. [Demo](#9-demo)
10. [Status & Roadmap](#10-status--roadmap)

---

## 1. Vision

Trend Cue gives anyone the ability to understand what's happening in a specific corner of social media — not through charts and sentiment scores, but through the actual content driving the conversation.

| | |
|---|---|
| **For** | Marketing professionals, content creators, and researchers |
| **Who** | Need to find specific trending content across social media but waste hours scrolling through irrelevant noise |
| **The** | Trend Cue is a semantic trend engine |
| **That** | Lets users type natural language queries and instantly surface the most relevant, trending posts from Instagram, TikTok, and Twitter/X — organized by topic clusters with real engagement data |
| **Unlike** | Brandwatch, Meltwater, and Sprout Social, which show aggregate dashboards but hide the actual content behind the numbers |
| **We** | Surface the real posts, videos, and images driving the trends — so users see both *what* is trending and *why* it's trending in one unified view |

---

## 2. The Problem

People are drowning in social media content but starving for insight. Finding what's actually trending in a specific niche — gym culture this month, AI hiring discourse this week, an emerging fashion aesthetic — requires manually scrolling through multiple platforms with no unified view.

Platform algorithms optimize for engagement and ad revenue, not for answering *"what's going on in X right now?"* There is no single place to type a natural language query and get back the most relevant, trending content across platforms, organized by topic, ranked by real engagement, and connected to the broader conversation.

**The critical gap:** enterprise tools like Brandwatch and Meltwater show aggregate trends — line graphs, sentiment scores, word clouds. But they don't display the actual content driving those trends. A marketing manager sees a 400% spike in mentions and still has to open TikTok on her personal phone to understand why. The data and the evidence are structurally disconnected.

---

## 3. The Solution

Trend Cue is a semantic trend engine for social media. An AI agent continuously collects public content from major platforms, extracts its meaning as dense vector representations, and stores it in a searchable index. When a user queries *"biggest gym problems in February 2026,"* they get the most semantically relevant trending posts across platforms — alongside the topic clusters those posts belong to.

**Supported platforms:** Instagram · TikTok · Twitter/X

Unlike social listening tools that abstract content into dashboards, Trend Cue keeps the original content front and center. Users see the actual videos, images, and posts — streamed directly from source platforms — alongside the quantitative context (views, likes, comments) that gives those posts meaning.

### Core Interaction Model

```
Search  →  Discover  →  Explore
```

Type a natural language query or browse the curated home feed → get ranked posts with engagement data and trend cluster labels → follow trend pills to adjacent topics and related content.

---

## 4. Core Concepts

Three data primitives underpin the entire product. Together they form a navigable graph of what the internet is talking about.

### Trends

Trends are AI-generated topic clusters, not static hashtags. Each trend is a semantic region in vector space with a human-readable label. Trends exist at multiple levels of granularity: "Tech" contains "AI," which contains "AI in Hiring." They emerge organically from the content itself and shift as discourse shifts. On the surface, trends appear as labeled pills with engagement heat indicators — **rising**, **peaking**, or **cooling** — so users can read momentum at a glance.

### Posts

Posts are platform-agnostic content units. Each post carries its original media (text, image, video), its source platform, engagement metrics (views, likes, comments), a timestamp, and a set of associated trends. Every post connects to multiple trends, and those connections are weighted by semantic relevance. The post is the unit of evidence behind every trend.

### The Trend Graph

The trend graph is the connective tissue. Trends link to posts; posts link back to trends. This creates a navigable graph where users can move fluidly from a specific post to a broad topic to a related post they would never have found otherwise. The graph turns isolated content into a map of what the internet is talking about.

---

## 5. User Experience

### Home

The home page surfaces a curated grid of trending topics, each showing its top posts. Six trending posts from "AI," six from "Fitness," six from "Finance" — each section headed by the trend label and its momentum indicator. Selection personalizes over time but starts with broadly popular trends.

### Search

A natural language search bar sits at the top. Users type queries like *"remote work backlash 2026"* or *"best running shoes discussion"* and get back a ranked list of matching posts with engagement metrics and associated trend pills. The search is semantic, not keyword-based. It understands intent, synonyms, and conceptual proximity.

### Trend View

Clicking a trend pill — from the home page, a search result, or a post detail — opens the trend view: a feed of the most relevant and popular posts within that topic, sorted by a blend of recency and engagement. Related trends appear as lateral navigation, enabling discovery without dead ends.

### Post Detail

Full content with source attribution, engagement metrics (views, likes, comments), timestamp, and associated trend pills. Each pill is clickable, creating a seamless loop: post → trend → new posts → new trends. A post about *"tech layoffs and AI replacement"* might carry "Tech," "AI," and "Employment." Clicking "Employment" takes the user into that trend's feed — a completely different slice of the same conversation.

---

## 6. Positioning

### What We Are

Trend Cue is a semantic intelligence layer on top of social media. We don't host original content, we don't have followers or feeds in the traditional sense, and we don't compete with Instagram or TikTok for creator attention. We are a search engine for what's trending, built for people who want signal without noise.

### What We Are Not

We are not a social media platform. We are not a social listening tool for enterprises. Products like Brandwatch, Meltwater, and Sprinklr are built for brand monitoring and competitor analysis at scale. They show dashboards; we show content. They answer *"how many mentions."* We answer *"what are people actually saying and showing."*

### The Gap We Fill

Every competitor in the social listening space extracts context and displays aggregate trends. None of them surface the actual content in a searchable, navigable format. Users see that something is trending but cannot see *what* is trending. Trend Cue closes that gap by unifying quantitative trend data with the qualitative content that drives it.

---

## 7. Competitive Landscape

The social media analytics and listening market is valued at approximately $10.5B, projected to reach $20–25B by 2030–2032. The market is fragmented: over 60% is held by smaller tools and native platform analytics.

| Product | Core Target | Killer Feature | Key Weakness | Entry Price |
|---|---|---|---|---|
| **Brandwatch** | Market researchers | 150M+ sources, visual/logo detection | Steep learning curve, no day-to-day community tools | $1,000–2,000+/mo |
| **Meltwater** | PR & comms | Global cross-channel reach (social + print + broadcast) | Jack-of-all-trades, dated UI | $1,000+/mo |
| **Sprout Social** | Social media managers | Best-in-class UX, unified team inbox | Listening lacks surgical depth for research | $199/user/mo |
| **Sprinklr** | Fortune 500 C-suite | Full omnichannel CXM integration | Extreme complexity, slow deployment | $10,000+/mo |
| **Trend Cue ⟁** | Marketers, creators, researchers | Semantic search returning actual posts, not dashboards | Early stage — coverage & scale TBD | $20/mo → |

**The dominant pattern across all competitors:** they extract context but show aggregate trends instead of real content. Businesses, marketers, and researchers need the content itself alongside the data to make informed decisions. Trend Cue occupies this gap.

---

## 8. Business Model

### Pricing Tiers

| Tier | Price | Target |
|---|---|---|
| **Individual** | $20/mo | Solo marketers, creators, researchers |
| **Teams** | $40–100/mo | B2B teams, agencies |
| **Enterprise** | Custom (via sales) | High-volume users, integrations, API access |

A pay-per-query model is also available as an alternative to flat subscriptions — for infrequent users and agencies running one-off research sprints.

### Unit Economics

| Metric | Target | Notes |
|---|---|---|
| **CAC** | ~$20 | ~$1 CPC on social ads (to be validated after first campaigns) |
| **LTV (starting)** | $60/mo | Target: $200+/mo as product matures and enterprise features are added |
| **Market Size** | $10.5B | → $25B projected by 2030–2032 |

---

## 9. Demo

An interactive flow demo demonstrates the core search → discover → explore interaction model. All data is illustrative — the demo is designed to validate the concept and gather feedback, not to reflect live platform data.

**Live demo:** https://trend-cue.github.io/flow/

The demo is part of an early validation phase targeting social media managers, content strategists, and trend researchers. A Tally questionnaire accompanies the demo for structured feedback collection. Current targets: 30–50 survey responses and 8–12 validation calls.

---

## 10. Status & Roadmap

### Current Phase — Validation

Trend Cue is in early concept validation. The interactive demo and validation questionnaire are live. Outreach is ongoing across LinkedIn, Reddit, and Twitter/X.

### What's Being Validated

- Whether the core value proposition — semantic search returning actual posts rather than aggregate data — is compelling enough to pay for
- Preferred pricing tier
- Most important platforms to cover first
- Whether the search → discover → explore flow matches user mental models

### After Validation — Planned MVP Architecture

```
Ingestion Agent   →  Platform APIs (IG / TikTok / X)
      ↓
Embedding Layer   →  text-embedding-3-large (1536-dim)
      ↓
Vector Store      →  pgvector / Pinecone
      ↓
Trend Clustering  →  HDBSCAN + GPT-4o labeling
      ↓
Search API        →  cosine similarity + engagement reranking
      ↓
Frontend          →  React + semantic search UI
```

If validation confirms demand, the next phase is a real ingestion pipeline pulling public content from at least two platforms, a vector store for semantic retrieval, and a production version of the current UI.

---

*Early validation phase · Not publicly launched · Demo: [trend-cue.github.io/flow](https://trend-cue.github.io/flow/)*