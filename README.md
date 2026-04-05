# Coding Agent Wisdom

This repo is a plain distillation of Peter Steinberger's writing on coding agents and agentic engineering at [steipete.me](https://steipete.me/).

It is meant to be short.
It is meant to help real work.

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

This is my best public reading as of April 5, 2026.
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

## Notes

See [NOTES.md](NOTES.md) for source notes and supporting references.
