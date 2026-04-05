# Coding Agent Wisdom

This repo is a plain distillation of Peter Steinberger's writing on coding agents, AI tools, and agentic engineering at [steipete.me](https://steipete.me/).

The aim is simple:

- gather what is useful
- remove noise
- keep what helps real work

This is not a transcript.
It is a working guide.

## The Short Version

- Talk to the agent plainly.
- Give it real tools and real context.
- Keep the loop fast.
- Ask for small, visible steps.
- Review the work.
- Keep the human in charge of judgment.
- Watch for excess. The speed is real. So is the pull.

## Plain Rules

### 1. Speak simply

Do not hide the task inside a clever prompt.

Say what you want.
Name the files.
State the constraints.
Ask for proof.

Clear work beats prompt theater.

### 2. Put the agent close to the work

Coding agents are strongest when they can act in the real environment:

- terminal
- editor
- tests
- documentation
- screenshots
- build tools

The more direct the path from idea to feedback, the better.

### 3. Prefer simple interfaces

A plain CLI often beats a fragile special integration.

The tool should be easy for both a human and an agent to use.
If a tool is hard to explain, hard to debug, or hard to test, it will slow the loop down.

### 4. Keep the feedback loop tight

Fast work depends on fast feedback.

That means:

- rebuild quickly
- test quickly
- inspect quickly
- recover quickly

At some point, the bottleneck is not typing.
It is how fast you can see what the agent just did and decide what comes next.

### 5. Start small, then widen

Begin with one concrete task.

Do not ask for a grand rewrite when a narrow change will prove the path.
Small changes make review easier.
They also make failure cheaper.

### 6. Give context, not ceremony

The agent needs the right materials more than the perfect speech.

Useful context includes:

- the relevant files
- the failing command
- the expected behavior
- a screenshot
- the docs that matter
- one good example

This is usually more valuable than adding more instructions about how to think.

### 7. Use more than one agent only when the split is clean

Parallel work is useful when tasks are clearly separate.

If two agents are stepping on the same files or the same decision, you create confusion instead of speed.

Divide by responsibility, not by hope.

### 8. Let the human own judgment

The agent can draft, search, refactor, test, and move quickly.

The human should still own:

- architecture
- priorities
- risk
- taste
- final acceptance

Speed is not wisdom.

### 9. Treat agent tools like real software

If you build tools for agents, they should be boring in the best sense:

- sensible defaults
- clear descriptions
- helpful errors
- lenient input handling
- logs
- tests
- release discipline

An unreliable tool poisons the whole workflow.

### 10. Protect the loop from drift

Agents can wander.
Sessions can bloat.
Projects can become messy.

Use small commits, visible diffs, and clean checkpoints.
Make it easy to stop, inspect, and restart.

### 11. Protect yourself too

Agentic work can become compulsive.

The speed is exciting.
The volume of ideas grows.
The hours can quietly expand.

So keep some restraint:

- stop on purpose
- watch the time
- rest before judgment gets weak

This is a power tool.
Use it with discipline.

## A Simple Workflow

1. Pick one real task.
2. Give the agent the minimum useful context.
3. Ask for a small change and a clear result.
4. Review the diff.
5. Run the check that matters.
6. Fix what is wrong.
7. Repeat.
8. Scale up only after the loop is stable.

## Good Tooling Helps

Several recurring ideas in Steinberger's posts point to the same lesson: agentic work improves when the environment is built for it.

Useful examples:

- screenshot tools help agents see the real UI state
- auto-build tools remove stale-test confusion
- clean text versions of docs make retrieval easier
- terminal helpers make parallel sessions manageable

This is not glamour.
It is shopkeeping.
But clean shopkeeping matters.

## A Practical Standard

If you want a simple test for whether you are using coding agents well, ask:

- Is the task clear?
- Is the context real?
- Is the feedback fast?
- Is the change reviewable?
- Is the human still deciding?

If the answer is yes, you are probably on solid ground.

## Warnings

- Do not confuse motion with progress.
- Do not trust long sessions just because they are busy.
- Do not hand over architecture because the agent writes fast.
- Do not build a fragile stack of tools you cannot explain.
- Do not let the pace eat your judgment.

## Sources

This README was distilled from Steinberger's relevant posts on AI-assisted development and coding agents, especially these:

- [Shipping at Inference-Speed](https://steipete.me/posts/2025/shipping-at-inference-speed)
- [Just Talk To It - the no-bs Way of Agentic Engineering](https://steipete.me/posts/just-talk-to-it)
- [My Current AI Dev Workflow](https://steipete.me/posts/2025/optimal-ai-development-workflow)
- [Just One More Prompt](https://steipete.me/posts/just-one-more-prompt)
- [Poltergeist: The Ghost That Keeps Your Builds Fresh](https://steipete.me/posts/2025/poltergeist-ghost-keeps-builds-fresh)
- [Self-Hosting AI Models After Claude's Usage Limits](https://steipete.me/posts/2025/self-hosting-ai-models)
- [Peekaboo 2.0 – Free the CLI from its MCP shackles](https://steipete.me/posts/2025/peekaboo-2-freeing-the-cli-from-its-mcp-shackles)
- [Command your Claude Code Army, Reloaded](https://steipete.me/posts/command-your-claude-code-army-reloaded)
- [Essential Reading for Agentic Engineers](https://steipete.me/posts/2025/essential-reading)
- [My AI Workflow for Understanding Any Codebase](https://steipete.me/posts/2025/understanding-codebases-with-ai-gemini-workflow)
- [VibeTunnel: Turn Any Browser into Your Mac's Terminal](https://steipete.me/posts/2025/vibetunnel-turn-any-browser-into-your-mac-terminal)
- [Peekaboo MCP – lightning-fast macOS screenshots for AI agents](https://steipete.me/posts/2025/peekaboo-mcp-lightning-fast-macos-screenshots-for-ai-agents)
- [Claude Code is My Computer](https://steipete.me/posts/2025/claude-code-is-my-computer)
- [The Future of Vibe Coding: Building with AI, Live and Unfiltered](https://steipete.me/posts/2025/the-future-of-vibe-coding)
- [MCP Best Practices](https://steipete.me/posts/2025/mcp-best-practices)

The point of this repo is not to repeat the posts.
It is to extract the working principles.
