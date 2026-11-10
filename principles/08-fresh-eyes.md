# 8. Fresh Eyes

**After any real change, an independent reviewer with minimal context checks it. Loop until clean.**

## The problem this solves

The person who just built the thing is the worst person to catch what's wrong with it. They know what it's *supposed* to do, so they read that intention into the output and skim right past the bug, the leftover placeholder, the assumption that didn't hold. Context, here, is a liability. It hides the flaws.

## The rule

After any non-trivial change, hand it to a reviewer who **didn't** build it and has **minimal** context about what it was supposed to be.

- Give them the change and the standard to check against. Not the whole backstory — that just re-introduces the same blindness.
- Their only job is to find problems. Not to praise, not to agree.
- Fix what they find. Then send it back.
- **Loop until the review comes back clean.** One pass is a check. The loop is the mechanism.

The reviewer can be a colleague, a separate pass by yourself after real distance, or a cheap independent agent. The requirement isn't who — it's *independent* and *low-context*.

## Why minimal context matters

A reviewer who knows the full plan evaluates the thing against the plan in their head, and quietly forgives every place reality drifted from it. A reviewer who only sees the output and the standard evaluates what's *actually there*. The second one catches the things you can't, precisely because they can't see what you meant.

## Why it loops

The first review surfaces the obvious problems. Fixing those sometimes creates or reveals new ones. A single pass gives false confidence. Looping — review, fix, review again — is what actually drives the defect count to zero. Stop when a pass returns nothing, not when you're tired of reviewing.

## The honest version

It stings to hand your finished work to someone whose entire job is to find what's wrong with it, and it's tempting to skip it when you're sure it's fine. "Sure it's fine" is exactly the state of mind this principle exists to check. The cost is a few minutes. The thing it catches is the bug you'd have shipped.

## Checklist

- [ ] Did an independent, low-context reviewer look at this?
- [ ] Was their job strictly to find problems, not to approve?
- [ ] Did I fix what they found and send it back?
- [ ] Did I loop until a pass came back with nothing?

See also: [Mistakes Are System Defects](07-mistakes-are-system-defects.md)
