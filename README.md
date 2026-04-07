# What Is Peter Steinberger's Workflow?

This repo tries to answer one simple question: what is Peter Steinberger's workflow for coding with agents?

It is a plain distillation of Peter Steinberger's writing on coding agents and agentic engineering at [steipete.me](https://steipete.me/).

It is meant to be short.
It is meant to help real work.

## Source Archive

The full source posts now live in `sources/peter-steinberger-blog/posts/`.

They were copied on April 7, 2026 from Peter Steinberger's public website repo:

- upstream repo: `https://github.com/steipete/steipete.me`
- upstream commit: `01506429797d8097a5722deba2a0224741fb1613`
- archive scope: 108 Markdown blog posts

## The Main Things

- Speak plainly.
- Give the agent real context.
- Keep the loop fast.
- Ask for small steps.
- Review the work.
- Keep human judgment in charge.
- Use discipline. The pace can carry you away.

## Simple Rules

### Speak plainly

Say what you want.
Name the files.
State the constraints.
Ask for the result you need.

Clear instruction beats clever prompting.

### Give real context

Agents do better with real material than with elaborate ceremony.

Useful context:

- the relevant files
- the failing command
- the expected behavior
- the right docs
- one good example
- a screenshot when the UI matters

### Keep the loop fast

Fast feedback matters more than fast typing.

You want to see the change quickly.
You want to test it quickly.
You want to know quickly if the agent is on the right path.

### Start small

Begin with one concrete task.

Small tasks are easier to review.
They fail more cleanly.
They teach you whether the agent understands the work.

### Prefer simple tools

A plain CLI is often better than a fragile special layer.

Good tools for agents are simple, testable, and easy to recover from.
Bad tools waste time and blur responsibility.

### Keep the human in charge

The agent can move fast.
The human should still own:

- priorities
- architecture
- risk
- taste
- final acceptance

Speed is useful.
It is not judgment.

### Use tools that make the loop clearer

The recurring pattern in Steinberger's posts is not magic.
It is practical support for the work:

- screenshot tools
- auto-build tools
- readable docs
- terminal helpers

This is ordinary discipline.
It matters.

### Watch the downside

Agentic work can become compulsive.

It feels productive because so much is always moving.
That is not the same as good judgment.

Stop on purpose.
Review the work.
Rest before you get sloppy.

## A Plain Workflow

1. Pick one real task.
2. Give the minimum useful context.
3. Ask for a small result.
4. Inspect the diff.
5. Run the check that matters.
6. Correct course.
7. Repeat.

## Test Yourself

Ask:

- Is the task clear?
- Is the context real?
- Is the change reviewable?
- Is the feedback fast?
- Is the human still deciding?

If yes, the workflow is probably sound.

## Peter's Current Setup

This is my best public reading as of April 7, 2026.
It is based on his latest posts from August 2025 to February 2026, plus his public GitHub profile.

The short version:

- Ghostty as the main terminal
- VS Code on the side
- codex as the main coding agent
- GPT-5 Pro as a harder-question path
- Opus for some general computer automation tasks
- likely CodexBar, VibeTunnel, Peekaboo, and Poltergeist around it

The workflow seems simple:

- work in Ghostty
- talk to the model, then tell it to build
- watch the stream more than the code
- queue follow-up work as ideas appear
- keep the loop tight with CLI-first tools

Branch flow also seems simple:

- mostly work on `main`
- avoid worktrees unless things get messy

Parallelism seems moderate:

- 1-2 agents is normal
- around 4 is a practical working number

He appears to know an agent is done by visibility, not by a grand control plane:

- terminal output
- terminal titles
- remote check-ins through VibeTunnel

This summary is partly direct statement and partly inference from these public sources:

- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow)
- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it)
- [Shipping at Inference-Speed](https://steipete.me/posts/2025/shipping-at-inference-speed)
- [Command your Claude Code Army, Reloaded](https://steipete.me/posts/command-your-claude-code-army-reloaded)
- [VibeTunnel: Turn Any Browser into Your Mac's Terminal](https://steipete.me/posts/2025/vibetunnel-turn-any-browser-into-your-mac-terminal)
- [Peter Steinberger on GitHub](https://github.com/steipete)

## Questions

### Q1. What do you mean by "stream" here: watch the stream more than the code

Answer:

Here "stream" means the live flow of agent output while it works.
That includes terminal output, tool output, progress, and in UI work the visible changes in the browser.

My reading is that he means this:

- he watches the agent's live activity
- he samples key parts of the code when needed
- he does not read every generated line

References:

- [Shipping at Inference-Speed](https://steipete.me/posts/2025/shipping-at-inference-speed): he says he does not read much code anymore and instead watches the stream
- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it): he describes watching the model build and the browser update in real time

### Q2. Does Peter just have multiple agents pushing to `main`? How does he keep things atomic and avoid merge conflicts?

Answer:

Mostly, yes, he appears to work on `main`.
But the public sources do not describe a rigid system for atomic commits or a formal merge-conflict prevention method.

What he does say:

- he tried worktrees and found they slowed him down
- he believes multiple areas can move in parallel if the areas are chosen carefully
- when an approach is uncertain, he may isolate it in a separate folder and inspect it as a PR
- the blast radius of the task matters when deciding how many agents to run

So the safe answer is:

- he seems to avoid conflicts mainly by partitioning work well
- he does not appear to rely on heavy branch machinery for normal work
- I did not find a public explanation of how he enforces atomic commits

References:

- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow): he says all of these work on `main`, worktrees slowed him down, and avoiding cross-pollination depends on careful choice of work areas
- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it): he describes one uncertain task in a separate folder so he can inspect the PR while the main repo continues refactoring

### Q3. What does he do after he has launched an agent on a task? Does he keep all terminals on one screen? Does he use notifications?

Answer:

At the desk, yes, he appears to keep several terminals visible on one large ultrawide display.
He explicitly says his 3840x1620 monitor fits 4 Claude instances plus Chrome without moving windows.

He also uses status and visibility tools:

- session title and session ID in the status line
- terminal titles for each agent session
- VibeTunnel for remote check-ins when away from the machine

I did not find a public post where he says he relies on notifications.
The evidence points more toward watching, checking, and polling than push notifications.

References:

- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow): Ghostty setup, wide monitor, 4 visible agent windows, status line and session ID
- [Command your Claude Code Army, Reloaded](https://steipete.me/posts/command-your-claude-code-army-reloaded): terminal titles used as status indicators
- [VibeTunnel: Turn Any Browser into Your Mac's Terminal](https://steipete.me/posts/2025/vibetunnel-turn-any-browser-into-your-mac-terminal): check on agents remotely and continue giving tasks

### Q4. When should a human use more than one agent?

Answer:

Use more than one agent when the work is separable and the blast radius is small.
Do not multiply agents just because you can.

Peter's public guidance points this way:

- 1-2 agents is normal
- around 4 can be good for cleanup, tests, and UI work
- the task boundary matters more than the raw number

References:

- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow): 1-2 agents normally, around 4 for certain kinds of work, depending on blast radius

### Q5. Does good agentic work require big specs?

Answer:

Not usually.

His later writing moves away from long spec-first workflows.
The pattern is more conversational and iterative:

- discuss the idea
- gather context
- start building
- refine while the work is visible

He still uses specs for tricky work, especially when he wants GPT-5 Pro to review the plan, but not as the default for everything.

References:

- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it): he says the old long-spec approach is no longer his default, and that he usually starts a discussion with codex

### Q6. Why does he prefer CLI-first tools?

Answer:

Because text is easy for agents to call, inspect, and verify.
That shortens the loop.

This is one of the clearest practical themes in his writing:

- start as CLI when possible
- let the agent call it directly
- verify output quickly

References:

- [Shipping at Inference-Speed](https://steipete.me/posts/2025/shipping-at-inference-speed): he says many things start as CLI because agents can call them directly and verify output

## Notes

See [NOTES.md](NOTES.md) for source notes and supporting references.
