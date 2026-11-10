# 5. Build to the Level, Not Beyond

**Engineer to the task's actual stakes. No speculative scope. You Aren't Gonna Need It.**

## The problem this solves

Over-building is procrastination that feels like diligence. You add the config system, the abstraction layer, the edge-case handling for inputs that will never arrive — and call it "doing it right." Meanwhile the actual thing you were testing still isn't in front of a real user. Polishing an untested bet is the most expensive way to avoid finding out whether it works.

## The rule

Every task sits somewhere on a scale from **quick-and-dirty** to **production-grade**. Figure out where *this* task belongs, and build to exactly that level. Not above it.

- A throwaway test to learn one thing: quick and dirty. A script, a spreadsheet, a fake door. Ship it today.
- A thing real users will depend on daily: build it properly.
- Most things are not the second one. Be honest about which you're looking at.

## Questions that set the level

- Is this proving something, or serving something? Proving → minimum that produces a clean read.
- How many people touch it, how often, and what breaks if it fails?
- Am I adding this because the task needs it, or because it would be "nice to have"? Nice-to-have is a no.
- Would a cruder version answer the same question? Then build the cruder version.

## Don't expand scope without a reason

New abstractions, new files, new tooling, new docs — each one is a cost you pay now against a benefit you're *guessing* you'll need later. YAGNI says: you probably won't. Add it when the need is real and present, not when it's imagined and future.

Suggesting a scope improvement is good. Quietly building it without checking is not.

## The honest version

Under-building has a fast, visible failure: it breaks and you fix it. Over-building has a slow, invisible one: weeks spent making an untested idea robust, and you never learn it was the wrong idea. The second failure is worse precisely because it's comfortable.

## Checklist

- [ ] Have I named where this task sits on quick-and-dirty ↔ production-grade?
- [ ] Am I building *to* that level and not past it?
- [ ] Is every piece of scope here actually needed now, not just maybe-later?
- [ ] Could a cruder version answer the same question sooner?

See also: [One Visible Queue](04-one-visible-queue.md) · [The Evidence Loop](../PLAYBOOK.md)
