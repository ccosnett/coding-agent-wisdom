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

## Notes

See [NOTES.md](NOTES.md) for source notes and supporting references.
