# AI Info Radar

AI Info Radar is the first practice project in this repository.

Its purpose is to help me keep up with frontier AI news without manually browsing many sources every day.

## Product Goal

Generate a short, high-signal AI briefing from multiple source types:

- official announcements
- GitHub and open-source momentum
- Hugging Face model and paper signals
- research papers
- model rankings and pricing
- community discussions

## Principle

Use structured feeds and APIs first. Use Browser Use only when the source has no clean interface or requires page interaction.

```text
feeds / APIs
  ->
browser fallback
  ->
deduplication
  ->
scoring
  ->
summary
  ->
daily or weekly briefing
```

## MVP Scope

The first version should answer:

1. What happened in AI today?
2. Which items are actually worth reading?
3. Why do they matter to Browser Use, agents, MCP, open-source tooling, or model capability?
4. Which noisy items can be ignored?

## Output Shape

```md
# AI Daily Briefing

## Top 5

## GitHub And Open Source

## Models And Products

## Papers And Research

## Worth Ignoring

## Links
```

## Folders

```text
ai-info-radar/
|-- configs/        # Source lists and scoring rules
|-- data/           # Local raw/intermediate data, ignored later if needed
|-- docs/           # Product notes and architecture
|-- outputs/        # Generated daily/weekly reports
|-- prompts/        # Summarization and ranking prompts
`-- src/            # Implementation will live here later
```
