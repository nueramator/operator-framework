# The Evidence Loop

This is the engine. The eight principles are the discipline; this is the cadence that puts them to work. It's how you take a bet from "I think this might work" to a clean verdict — keep going, change one thing, or stop — without lying to yourself along the way.

Run it on a fixed interval. Weekly is a good default. The interval matters less than the fixedness: a loop you run on a schedule beats a brilliant plan you run once.

---

## The loop

```
   ┌─────────────────────────────────────────────┐
   │                                             │
   ▼                                             │
1. FRAME      →  2. DEFINE THE READ   →  3. RUN  →  4. READ  →  5. DECIDE
   the bet         metric + sample       to size     honestly    (one move)
                      size                                         │
   ▲                                                               │
   └───────────────────────────────────────────────────────────── ┘
```

### 1. Frame the bet

Write it in one sentence: *"I believe [who] will [do what] because [why]."*

Then split it:
- **Core (frozen):** the part you're actually testing. Off-limits until the test reads.
- **Variables (tunable):** wording, channel, targeting, price, sequence. Fair game.

→ Principle: [One Frozen Bet](principles/01-one-frozen-bet.md)

### 2. Define the read — *before* you run

This is the step everyone skips, and skipping it is why most tests never conclude. Decide up front:

- **The one metric** that proves or kills the bet. One. Not a dashboard.
- **The sample size** that makes a result real. How many attempts / users / data points before you're allowed to draw a conclusion. Write the number down now, while you can't yet be tempted to move it.
- **The kill line:** the result at or below which the bet is dead. Also written now.

If you can't name the metric and the number, you don't have a test yet. You have a hope.

→ Principles: [Evidence Over Opinion](principles/02-evidence-over-opinion.md) · [Research the Operators](principles/03-research-the-operators.md)

### 3. Run it to sample size

Execute. Keep the work in [one visible queue](principles/04-one-visible-queue.md) and build each piece to [the level it needs](principles/05-build-to-the-level.md) — no more. When you hit a wall, [beat the roadblock](principles/06-beat-the-roadblock.md) instead of stopping.

The one unbreakable rule of this step: **do not change the core while the test is running.** Tune variables if you must, and note what you changed. But the bet stays frozen until the number you wrote in step 2 is reached.

### 4. Read the result honestly

Did it hit the sample size? If not, you have no verdict yet — keep running, don't conclude. If yes:

- Compare the metric to the kill line. Plainly. No reinterpreting a failure into a success because you're attached to it.
- Report what actually happened, including what went wrong and what got skipped.

### 5. Decide — exactly one move

Based on a test that *actually read*:

| Result | Move |
|---|---|
| Hit the target | Keep the bet. Scale it or push to the next rung. |
| Missed, but a variable was clearly off | Keep the core. Tune **one** variable. Run again. |
| Missed at sample size, variables were sound | Kill the bet. Now — and only now — you're allowed to pick a new one. |

Then loop. Every non-trivial change gets a [fresh-eyes review](principles/08-fresh-eyes.md) before it counts as done. Every mistake along the way becomes a [patched rule](principles/07-mistakes-are-system-defects.md), not an apology.

---

## The one-page template

Copy this per bet. Fill it in order. Don't run until steps 1–2 are complete.

```
BET (one sentence):
  I believe ______ will ______ because ______.

CORE (frozen):           ___________________________
VARIABLES (tunable):     ___________________________

THE READ (fill before running):
  Metric:                ___________________________
  Sample size:           ______  (what counts as a real test)
  Kill line:             ______  (at/below this, the bet is dead)

RUN:
  Started:               ______
  Variables changed:     ___________________________
  Reached sample size?   yes / no

RESULT:
  Metric came in at:     ______
  Verdict:               hit / tune-a-variable / kill

NEXT MOVE (exactly one):
  ___________________________________________________
```

---

## The two failure modes this prevents

Everything above is aimed at exactly two ways work dies:

1. **Impatience** — pivoting before the test reads. The sample size defined in step 2 is the cure. You literally cannot conclude until you hit the number you wrote down.
2. **Opinion** — deciding without evidence. The metric and kill line are the cure. The decision in step 5 is made by a number, not by how you feel about the bet that day.

Protect those two cures and the loop works. Erode them and you're back to four pivots a month and nothing shipped.
