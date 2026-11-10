# 7. Mistakes Are System Defects

**No blame, no apology. Find the missing rule and fix the system.**

## The problem this solves

When something goes wrong, the default reactions are both useless: apologize (which fixes nothing) or assign blame (which fixes nothing and makes people hide the next mistake). Both treat the error as a moral event. It isn't. It's information about where your system has a gap.

## The rule

Treat every mistake as a defect in the process, not a failing of the person or tool that surfaced it.

When something goes wrong:

1. **Don't apologize or assign blame.** Skip it entirely. It adds nothing.
2. **Find the gap.** What rule, instruction, or check was missing or ambiguous enough to let this happen?
3. **State it plainly.** "This happened because the process didn't specify X."
4. **Propose the exact fix.** The specific rule or guardrail that would have caught it, written out.

The output of a mistake is an improved system. If a mistake doesn't make the system better, you wasted it.

## Why this works

A mistake usually isn't a one-off. It's a category. The same gap will produce the same error again under the same conditions, no matter how sorry anyone is. Patch the category and that whole class of error stops happening. Patch nothing and you'll be back.

Blame also has a hidden cost: it makes the next mistake get buried instead of surfaced. A no-blame system gets told the truth early, which is the only time the truth is cheap to act on.

## Example

| Blame response | System-defect response |
|---|---|
| "My bad, I messed that up." | "The process never said which source was authoritative, so the wrong one got used. Fix: add a rule naming the source of truth for this." |
| "The tool's broken." | "We assumed the tool validated input and it doesn't. Fix: add an explicit validation step before the call." |

## The honest version

This isn't about dodging responsibility. It's the opposite — it's the most responsible possible response, because it's the only one that actually prevents the repeat. "Sorry" is cheap and changes nothing. A patched rule is accountability you can see.

## Checklist

- [ ] Did I skip the apology and the blame?
- [ ] Did I identify the specific gap that allowed this?
- [ ] Did I write down the exact fix, not a vague "be more careful"?
- [ ] Is the system now better than before the mistake?

See also: [Fresh Eyes](08-fresh-eyes.md)
