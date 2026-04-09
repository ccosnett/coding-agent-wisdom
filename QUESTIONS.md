# Questions About Peter Steinberger's Coding-Agent Workflow

This file collects questions worth answering as the repo gets better.

The point is not to speculate.
The point is to identify what to look for in his posts, repos, screenshots, talks, and public code.

## Terminal Setup

- Which terminal does he use?
- Why does he use that terminal instead of the alternatives?
- Which features matter most to him: speed, stability, tabs, panes, titles, remote access, rendering, or scripting?
- Does he publish his terminal config anywhere on GitHub or in a GitHub Gist?
- If a config exists, which parts of it seem essential to his workflow and which parts are just preference?
- How does he name or organize many concurrent agent sessions in the terminal?
- Does his terminal setup depend on a wide monitor, multiple windows, or a specific macOS layout?

## Agent Loop

- What does a normal session look like from start to finish?
- How small are the tasks he usually gives an agent?
- When does he say "plan only" versus asking the agent to implement immediately?
- How often does he interrupt and redirect the agent?
- What signals tell him a session is going well or going off track?
- What does he watch while the agent works: terminal output, diffs, browser refreshes, tests, or screenshots?

## Context And Prompting

- What context does he reliably provide before asking an agent to work?
- What kinds of context does he think are better than long prompt engineering?
- How does he describe constraints, expected output, and acceptance criteria?
- When does he prefer voice dictation over typing?
- Does he keep reusable prompt fragments, or is his workflow mostly conversational and situational?

## Codebase Understanding

- How does he approach a new codebase before asking for changes?
- What is his actual process for creating a software design document or spec for agent work?
- Which tools does he use to inspect code, docs, screenshots, and live behavior?
- What role do screenshots play in understanding and steering UI work?
- How does he decide when the agent has enough context to act?

## Repo And Branch Strategy

- Does he usually work on `main` or on branches?
- When does he use a separate folder instead of a worktree?
- How does he avoid cross-pollination between parallel agent efforts?
- What kinds of changes are safe to run in parallel and which ones are not?
- How does he review and merge agent-made changes?

## Tools And Automation

- Which CLI tools are central to his workflow?
- Why does he prefer CLI-friendly tools for agents?
- Which tools has he built specifically to make agent work easier?
- How does he use tools like Peekaboo, Poltergeist, and VibeTunnel together?
- Which tools does he reject, and why?
- What does he believe makes a tool agent-friendly rather than just flashy?

## Testing And Feedback

- How does he keep the feedback loop fast?
- What tests or checks does he run locally during agent work?
- When does he add CI in a new project?
- How does he detect stale work, wrong assumptions, or hidden regressions early?
- What kinds of feedback does he want to surface directly inside the terminal?

## Models And Provider Choice

- Which models does he use for which kinds of tasks?
- When does he prefer Claude, Gemini, Codex, or open models?
- How often does he switch models inside the same project?
- What tradeoffs matter most to him: latency, coding quality, context size, reliability, or price?
- What caused him to adopt or abandon specific model/tool combinations?

## Human Judgment

- Which decisions does he delegate comfortably and which ones does he keep for himself?
- What does he treat as the human's job even in a fast agent loop?
- How does he review output before trusting it?
- What are his standards for "good enough" versus "needs correction"?
- How does he keep taste, architecture, and product judgment from being diluted by speed?

## Failure Modes

- What mistakes does he see people make when using coding agents?
- What parts of his earlier workflow has he explicitly changed his mind about?
- Where does he think subagents, heavy planning, or abstraction layers go wrong?
- What signs show that agentic work is becoming sloppy, compulsive, or misdirected?
- What safeguards does he use to stop bad loops early?

## Public Evidence To Check

- Which blog posts are the strongest primary sources for his workflow?
- Which GitHub repos show his workflow in code rather than just description?
- Which screenshots in his posts reveal concrete setup details?
- Which talks, podcasts, X posts, or commit histories add useful detail?
- Where does he show configuration files, scripts, or shell aliases that support the workflow?
