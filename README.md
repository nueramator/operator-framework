# The Operator Framework

A disciplined operating system for finding, validating, and shipping — whether you're building a product, testing a business, or running work through an AI agent.

Most work doesn't fail because the idea was wrong. It fails from **drift**: abandoning a bet before any test ran long enough to tell you anything, and swapping evidence for opinion whenever a decision got uncomfortable. This framework is a small set of constraints that keep one bet alive long enough to read, and keep every decision tied to data instead of vibes.

It is deliberately generic. Nothing here is tied to a specific industry, product, or person. Drop it in as-is, or copy the pieces you need.

---

## The core idea

> Pick one bet. Define what would prove it. Run the test to sample size without touching the bet. Read the result. Then — and only then — tune a variable or kill the bet.

Everything below exists to protect that loop from the two things that break it: **impatience** (pivoting early) and **opinion** (deciding without evidence).

---

## The principles

| # | Principle | In one line |
|---|-----------|-------------|
| 1 | [One Frozen Bet](principles/01-one-frozen-bet.md) | Commit to a single direction. Tune the variables around it, never the core, until a real test reads. |
| 2 | [Evidence Over Opinion](principles/02-evidence-over-opinion.md) | Decisions come from data with sources. "No data found" triggers research, never a guess. |
| 3 | [Research the Operators](principles/03-research-the-operators.md) | Learn from people who actually do the thing. Primary sources, real numbers, labeled assumptions. |
| 4 | [One Visible Queue](principles/04-one-visible-queue.md) | A single FIFO list. New ideas get appended, not swapped in. |
| 5 | [Build to the Level](principles/05-build-to-the-level.md) | Engineer to the task's actual stakes. No speculative scope (YAGNI). |
| 6 | [Beat the Roadblock](principles/06-beat-the-roadblock.md) | A block is the start of the work. Exhaust real workarounds before calling it impossible. |
| 7 | [Mistakes Are System Defects](principles/07-mistakes-are-system-defects.md) | No blame, no apology. Find the missing rule and fix the system. |
| 8 | [Fresh Eyes](principles/08-fresh-eyes.md) | After any real change, an independent reviewer checks it. Loop until clean. |

The engine that ties them together is the **[Evidence Loop](PLAYBOOK.md)** — the weekly cadence for running a bet to a verdict.

---

## When to use it

- You have a goal but every plan to reach it feels like a guess.
- You keep starting over. New direction every week, nothing ever finishes.
- You (or your team, or your agent) argue from opinion and call it strategy.
- You want a repeatable way to decide: keep going, change one thing, or stop.

## When not to use it

- The work is a known, bounded task with a clear finish. Just do it.
- You're in pure exploration with no intent to commit yet. Come back when you're ready to bet.

---

## How to adopt it

1. Read the [Evidence Loop](PLAYBOOK.md) first. It's the spine.
2. Skim the eight principles. They're short on purpose.
3. Write down **your** bet and your **kill metric** using the template in the playbook.
4. Run one full loop before changing anything about the framework itself.

The framework is a set of constraints, not a to-do list. Its whole value is in what it stops you from doing: pivoting early, deciding blind, and expanding scope you were never going to need.

---

## License

MIT. See [LICENSE](LICENSE). Use it, fork it, rename it, strip the attribution. It's yours.
