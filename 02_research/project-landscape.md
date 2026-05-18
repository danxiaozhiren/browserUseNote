# Project Landscape

## Layers

```text
Application layer
  AI info radar, RPA, browser assistant, developer debugging, data extraction

Agent layer
  browser-use, Stagehand, Skyvern, LaVague, Midscene, CUA-style agents

Browser control layer
  Playwright, WebDriver, CDP, Puppeteer, browser extensions

Infrastructure layer
  cloud browser, proxy, captcha handling, session management, replay, logs
```

## Project Tracking Template

| Project | Layer | What It Does | Strength | Risk | Notes |
| --- | --- | --- | --- | --- | --- |
| browser-use | Agent | Lets AI agents operate websites | General and popular | Reliability in long workflows | Track examples and cloud direction |
| Stagehand | Agent + code | AI actions on top of Playwright | Production-friendly hybrid approach | Requires workflow design | Good reference for practical architecture |
| Skyvern | AI RPA | Automates browser workflows | Enterprise process focus | Complex deployment | Relevant to AI RPA direction |
| Playwright | Control | Browser automation framework | Stable engineering base | Not an agent by itself | Default low-level practice tool |
| CDP | Control | Low-level Chrome control | Deep browser access | Chrome-specific complexity | Useful for debugging and observability |

## Research Questions

- Which projects are pure agent frameworks and which are production workflow tools?
- Where does Browser Use stop and RPA begin?
- Which problems are solved by better prompts, and which require product constraints?
- How much of the system should use feeds/APIs instead of browser browsing?
