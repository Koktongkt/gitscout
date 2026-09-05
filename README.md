# GitScout

GitScout is a Hermes Agent skill for discovering and evaluating trending AI engineering repositories on GitHub.

It focuses on recent momentum and technical substance rather than lifetime star counts.

## Coverage

- Agent runtimes, agentic harnesses, coding agents, and multi-agent systems
- MCP, tool calling, computer use, sandboxes, memory, and context engineering
- RAG, GraphRAG, knowledge graphs, retrieval, reranking, and document pipelines
- AI backends, model gateways, serving, routing, caching, and observability
- Evaluations, testing, guardrails, security, and red teaming
- Generative UI, voice, multimodal, and human-in-the-loop integrations

## How it works

GitScout uses 7-day, 30-day, and 90-day discovery windows. It inspects shortlisted repositories beyond their search snippets and ranks them using:

- Recent momentum
- Technical substance
- Relevance
- Maintenance health
- Originality
- Practical usefulness
- Documentation and onboarding

The resulting report includes verified links, momentum evidence, engineering value, risks, maintenance status, and a practical verdict for each repository.

## Installation

Copy this repository into your Hermes skills directory:

```text
<HERMES_HOME>/skills/research/gitscout/
```

The directory must contain `SKILL.md`. Start a fresh Hermes session after installation so the skill index reloads.

## Usage

Ask Hermes for a GitScout report, for example:

```text
Use GitScout to find the 10 most interesting AI engineering repositories trending this month.
```

You can narrow the request to agent infrastructure, RAG, AI backends, frontend integrations, evaluation, or another area in the skill taxonomy.

## License

MIT
