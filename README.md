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

His setup changed during 2025, so the dates matter.

On August 25, 2025, his explicit setup was Ghostty as the main terminal, VS Code on the side, and Claude Code as the main coding agent.

By October 14, 2025, and more clearly by December 28, 2025, his writing shows a shift toward codex as the main coding agent.
My reading is that the latest setup is:

- Ghostty as the main terminal
- VS Code on the side for looking at code
- codex as the main coding agent
- GPT-5 Pro as an escalation path for harder questions
- Opus for some general computer automation tasks

This part is partly direct statement and partly inference:

- Ghostty is the latest terminal he names explicitly.
- codex is the latest coding agent he clearly favors.
- I did not find a later post saying he abandoned Ghostty.

### How he seems to work

- He usually works iteratively, not from a giant fixed spec.
- He starts a discussion with the model, explores, refines the plan, and then tells it to build.
- He often watches the stream instead of reading every line of code.
- He queues more work as new ideas appear.

### Worktrees or not

Usually not.

His latest explicit statement is that he simply commits to `main`.
He says worktrees slow him down.
He says codex sometimes creates one automatically when things get messy, but that this is rare and usually only for exceptional cases.

### Does he work on `main`

Mostly yes, by his own description.

He says he commits to `main`.
He also describes cases where work may happen in a separate folder or produce a PR when he wants to inspect an approach, but the general pattern he describes is linear work on `main`, not a worktree-heavy flow.

### How many terminals or agents

The number varies with the task.

- On August 25, 2025, he wrote that he usually runs 1-2 agents, and around 4 is a sweet spot for cleanup, tests, and UI work.
- In the same post, he says his display fits 4 Claude instances plus Chrome.
- On December 28, 2025, he writes that he often works across 3-8 projects at a time, and gives an example of running refactors on 4 projects while writing.

So the safe reading is:

- 1-2 is normal for focused work
- around 4 is common for parallel cleanup or refactor work
- more can be in flight across projects, but 4 appears to be a practical working number

### How he knows an agent has finished

I did not find a post where he says he relies on a formal notification system.

What he does describe is simpler:

- he watches terminal output
- he uses terminal titles and status indicators to see what each session is doing
- he uses VibeTunnel to check on agents remotely and see whether a task is finished

So my understanding is that he mostly knows by visibility, not by elaborate orchestration:

- terminal title
- current stream of output
- remote check-in through VibeTunnel
- queueing follow-up messages when a task may stall

Sources for this section:

- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow)
- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it)
- [Shipping at Inference-Speed](https://steipete.me/posts/2025/shipping-at-inference-speed)
- [Command your Claude Code Army, Reloaded](https://steipete.me/posts/command-your-claude-code-army-reloaded)
- [VibeTunnel: Turn Any Browser into Your Mac's Terminal](https://steipete.me/posts/2025/vibetunnel-turn-any-browser-into-your-mac-terminal)

## Notes

See [NOTES.md](NOTES.md) for source notes and supporting references.
