# Browser Use Mental Model

## One-Line Definition

Browser Use is an AI adaptation layer that lets agents operate existing human-facing software through the browser.

It is not just web scraping, not just RPA, and not just browser testing. It sits between them.

## Core Tension

```text
The more general it is, the less stable it becomes.
The more stable it is, the less it looks like an agent.
```

This tension is the core product and engineering problem of Browser Use.

## Layered View

```text
User intent
  ->
Agent planning and judgment
  ->
Browser observation: DOM, screenshot, accessibility tree, network
  ->
Action execution: click, type, scroll, wait, upload, download
  ->
Verification: page state, data structure, screenshot, business rule
```

## Browser Use As Compatibility Layer

Browser Use exists because most existing software was designed for humans, not agents.

Long term, more systems may expose agent-friendly APIs, MCP servers, or structured operation protocols. But Browser Use will remain useful for:

- systems without APIs
- legacy enterprise back-office tools
- third-party websites
- UI regression and real-user-path testing
- visual or canvas-heavy applications
- workflows where the browser page itself is the source of truth

## Practical Principle

Do not let the agent freely wander when a workflow can be constrained.

Use a hybrid design:

```text
Deterministic steps: code and browser automation
Uncertain steps: AI interpretation
Critical actions: preview, evidence, and human confirmation
Final state: explicit verification
```

## Human-In-The-Loop

The valuable pattern is not asking the user to approve every click.

The better pattern is:

```text
Agent does search, extraction, comparison, and drafting.
User reviews evidence and approves the final result.
```

Users are more willing to review outcomes than supervise every step.
