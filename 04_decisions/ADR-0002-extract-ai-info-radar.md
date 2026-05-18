# ADR-0002: Extract AI Info Radar Into A Separate Repository

- Date: 2026-05-18
- Status: accepted

## Context

AI Info Radar started as a practice direction inside this Browser Use learning
repository.

During product discussion, it became clear that AI Info Radar is broader than a
Browser Use exercise. Its product goal is to track the AI frontier across models,
tools, papers, products, open-source projects, and industry changes, with an
adjustable learning focus.

Keeping it as a subfolder would make this repository mix two concerns:

- Browser Use / browser-agent learning notes and experiments.
- A standalone AI information radar product.

## Decision

Extract AI Info Radar into its own repository:

https://github.com/danxiaozhiren/ai-info-radar

Keep this repository focused on Browser Use understanding, research, and small
browser-agent labs.

## Consequences

The Browser Use notebook stays clean and focused.

AI Info Radar can evolve as an independent product with its own source strategy,
scoring model, prompts, outputs, and implementation.

This repository can still reference AI Info Radar as an external practice
context for Browser Use and Agent learning.
