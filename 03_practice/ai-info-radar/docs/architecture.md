# Architecture

## Pipeline

```text
source registry
  ->
fetchers
  ->
normalizer
  ->
deduplicator
  ->
scorer
  ->
summarizer
  ->
report writer
```

## Fetching Strategy

1. Prefer RSS, API, or static structured content.
2. Use browser automation for dynamic pages, pages without feeds, and pages that require interaction.
3. Store source URL and fetch timestamp with every item.

## Verification Strategy

Each report item should keep:

- original URL
- source type
- timestamp
- relevance tags
- short reason for inclusion
- confidence level

## Browser Use Role

Browser Use should be a fallback and enrichment layer, not the entire system.

Good uses:

- GitHub Trending pages
- pages without RSS
- dynamic changelog pages
- product pages where details require interaction

Bad uses:

- sources with stable APIs
- bulk crawling without a clear question
- pages where structured access is simpler and more reliable
