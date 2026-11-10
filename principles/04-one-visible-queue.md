# 4. One Visible Queue

**A single FIFO list. New ideas get appended, not swapped in.**

## The problem this solves

Mid-task, a new idea shows up. It feels urgent. So you drop what you're doing to chase it. Now two things are half-done. Repeat a few times and you have ten half-finished threads, no memory of the order you meant to do them in, and nothing actually shipped. Context-switching is where throughput goes to die.

## The rule

Treat all work as a single first-in-first-out queue, and keep it visible.

- New ideas, tweaks, and corrections get **appended** to the queue. They do not interrupt the active task.
- You finish — or deliberately park — the current task before starting the next.
- **One exception:** a correction to the task you're doing *right now*, because it's wrong right now, gets fixed in place. Everything else goes to the back of the line.
- "Done" means the queue is empty. Not "the fun part is done." Empty.

## Why FIFO

FIFO isn't the theoretically optimal scheduler. It's the one that resists the specific failure above: the shiny new thing cutting the line. The queue being boring and strict is the point. It removes the in-the-moment negotiation where impulse always wins.

If something genuinely is more important, you can reorder deliberately — as a decision, written down, not as a reflex mid-keystroke.

## Keep it visible

The queue should be something you and anyone watching can see at a glance: a shared list, a board, a task tool. Legibility is half the value. When the current state is visible, nobody has to ask "what's happening right now," and you can't quietly abandon a task by just... not looking at it.

## The honest version

The hardest part isn't maintaining the list. It's obeying it when a better idea arrives and every instinct says "just real quick." Append it. If it's real, it'll still be worth doing when you get there. If it's not, you just saved yourself the detour.

## Checklist

- [ ] Is there one list, and can I see all of it?
- [ ] When a new idea hit, did I append it instead of chasing it?
- [ ] Is the only thing I interrupted for a correction to the *current* task?
- [ ] Am I calling it "done" only when the queue is actually empty?

See also: [Build to the Level](05-build-to-the-level.md)
