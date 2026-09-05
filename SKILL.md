---
name: gitscout
description: Use when scouting trending AI repositories on GitHub.
version: 1.0.0
author: Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [github, ai, agents, rag, software-engineering, research]
    related_skills: [github-repo-management]
---

# GitScout

## Overview

Discover GitHub repositories gaining meaningful momentum in AI engineering. Find projects that are useful, original, and actively maintained—not merely repositories with high lifetime star counts.

## When to Use

Use for:

- Weekly or monthly AI repository discovery
- Emerging agent, RAG, GraphRAG, or AI infrastructure projects
- Interesting AI backend and frontend integrations
- Technical evaluation of newly popular repositories
- Repositories worth watching, testing, or adopting

Do not treat this report as a full security audit or production adoption review.

## Topic Taxonomy

Search across these areas, expanding when a genuinely new category emerges:

1. **Agent engineering:** runtimes, orchestration, agentic harnesses, coding agents, multi-agent systems, computer use, sandboxes, durable workflows, memory, and context engineering.
2. **Protocols and tools:** MCP, tool calling, browser automation, connectors, and agent interoperability.
3. **Retrieval and knowledge:** RAG, GraphRAG, knowledge graphs, hybrid search, reranking, document ingestion, citations, multimodal retrieval, and retrieval evaluation.
4. **AI backends:** model gateways, structured generation, inference serving, routing, caching, batching, asynchronous pipelines, vector databases, authentication, rate limits, multi-tenancy, cost, and latency tooling.
5. **AI frontends:** generative UI, streaming chat, voice, multimodal interfaces, visual workflow builders, approval workflows, local-first AI, and editor integrations.
6. **Quality and operations:** evaluations, testing, tracing, observability, guardrails, prompt-injection defenses, permission systems, red teaming, and monitoring.
7. **Emerging engineering:** local models, compilers, inference optimization, synthetic data, AI-native developer tools, alternative architectures, robotics, and embodied agents.

## Discovery Windows

Use more than one time horizon:

- **7 days:** very new signals
- **30 days:** default current-momentum window
- **90 days:** sustained growth or revival

State the report date and window. Do not call an old repository “trending” solely because it has many stars.

## Workflow

### 1. Discover broadly

Search GitHub Trending, GitHub repository search, relevant GitHub topics, and independent web sources. Use several narrow topic queries rather than one broad “AI” search.

Prefer public repositories. Exclude archived repositories by default. Search using combinations of topic, README terminology, creation date, recent push date, language, and minimum stars.

### 2. Build the candidate set

Collect, when available:

- Name, URL, description, category, and primary language
- Creation date, last push, latest release, stars, forks, and contributors
- Commit, issue, and pull-request activity
- License, documentation, examples, tests, and demos
- Independent mentions or evidence of adoption

Deduplicate forks, renamed projects, and projects with a common upstream implementation.

### 3. Verify shortlisted repositories

Inspect more than search snippets. Review at least:

- README and documentation
- Repository structure and implementation depth
- Recent commits and releases or changelog
- Open and recently closed issues and pull requests
- Contributor distribution
- License
- Examples and tests

Treat repository claims as claims until supported by code, documentation, releases, or independent evidence.

### 4. Assess momentum

Consider:

- Recent star growth or the best available proxy
- Growth relative to repository age and existing size
- Commit, contributor, release, issue, and pull-request activity
- Independent mentions and downstream adoption
- Whether attention is sustained or a short-lived spike

Never invent historical star counts. If exact star deltas are unavailable, say that momentum is estimated and identify the proxy used.

### 5. Assess engineering value

Evaluate:

- Clarity and importance of the problem
- Original technical contribution
- Working implementation versus concept or demo
- Architecture, tests, examples, and documentation
- Maintenance health and production readiness
- Security and privacy implications
- Dependency, provider, and vendor lock-in
- Whether it is a thin wrapper around another API

### 6. Filter low-value results

Down-rank or exclude:

- Abandoned or archived repositories
- Tutorial-only projects presented as frameworks
- Thin wrappers without meaningful engineering
- Forks with no substantial changes
- Suspicious or obviously manipulated engagement
- Link collections unless requested
- Projects without a usable license
- Repositories whose central claims cannot be verified

## Ranking

Score each repository from 0 to 100:

| Dimension | Weight |
|---|---:|
| Recent momentum | 25 |
| Technical substance | 20 |
| Relevance | 15 |
| Maintenance health | 15 |
| Originality | 10 |
| Practical usefulness | 10 |
| Documentation and onboarding | 5 |

Use scores only as comparative research aids. Include no more than three repositories from a single category unless the user requests otherwise.

## Output Format

Open with a concise summary of the most important signals and trends.

Then provide a ranked table:

| Rank | Repository | Category | Why now | Technical value | Momentum | Score |
|---:|---|---|---|---|---|---:|

For each selected repository include:

- **Repository:** linked owner/name
- **Category:**
- **What it does:**
- **Why it is trending:**
- **Technical interest:**
- **Momentum evidence:**
- **Maintenance status:**
- **Risks or limitations:**
- **Best suited for:**
- **Verdict:** Watch, Experiment, Adopt Carefully, or Skip

Finish with:

- Three broader trends observed
- Three repositories worth testing now
- Any projects that appear overhyped and why
- Search date and discovery window
- Data limitations

## Research Rules

- Link directly to every repository and important supporting source.
- Prefer primary GitHub evidence; use independent sources for corroboration.
- Separate verified facts from interpretation.
- Use absolute dates.
- Never claim production readiness without evidence.
- Prefer 5–10 strong findings over a long superficial list.
- Mention licensing, security, maintenance, and adoption risks.
- Explain why each repository matters technically, not only what it does.
- Do not fabricate metrics, repository details, or trend data.

## Common Pitfalls

1. Ranking by lifetime stars instead of recent momentum.
2. Presenting estimated star growth as exact data.
3. Repeating README marketing without inspecting the repository.
4. Allowing agent frameworks to crowd out all other categories.
5. Ignoring smaller repositories with strong recent velocity.
6. Recommending unlicensed or inactive projects.
7. Treating polished demos as production-grade systems.
8. Confusing frequent commits with meaningful project health.

## Verification Checklist

- [ ] Multiple topic-specific searches were performed
- [ ] The report date and discovery windows are stated
- [ ] Every selected repository was inspected beyond the search result
- [ ] Duplicates, abandoned projects, and low-substance results were filtered
- [ ] Momentum evidence is included and uncertainty is labeled
- [ ] Technical value, maintenance, license, and risks are addressed
- [ ] Every repository and supporting source has a working link
- [ ] The final ranking follows the required output format
