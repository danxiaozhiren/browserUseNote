# Source Code

Implementation will live here later.

Suggested modules:

```text
src/
|-- fetchers/       # API, RSS, browser, and GitHub/HF fetchers
|-- normalizers/    # Convert source-specific data into common items
|-- scoring/        # Importance, novelty, action value, credibility, relevance
|-- reporters/      # Markdown daily/weekly report generation
`-- storage/        # Local cache or database
```

Keep the first implementation boring and observable before adding more agent behavior.
