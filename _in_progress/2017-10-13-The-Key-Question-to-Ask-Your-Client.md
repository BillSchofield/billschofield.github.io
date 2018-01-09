---
layout: post
title: The Key Question to Ask Your Client
---
A couple of years ago I noticed a recurring pattern in the way my teams
and clients were prioritizing work. I saw a lot of conflict surrounding
"technical tasks", "refactoring", and "technical debt".

Software developers and business stakeholders typically have a difficult
time integrating their disparate perspectives. I believe that asking one
key question can radically improve how we communicate about prioritization
of work by reframing how we understand return on investment.

# A Common Business Perspective

The business has a deadline or high priority outcome and is under
pressure to deliver. They are investing significant time, money, and
attention on their project and it is important that they get the most
for their money.

When they see new features working, they have evidence that they are
spending wisely and they feel safe. When they see developers working,
but they don't see new features being completed, they worry. They don't
have visibility into whether their investment is giving them a return.
So they focus the teams energy on completing features as quickly as
possibly.

This perspective is healthy, useful, and also incomplete. 

# A Common Developer Perspective
Developers want to do the best work they can, deliver lots of value for
the business, and work sustainably. They want to get the best results
for the time and energy they invest in their work.

When they see their software systems getting more complex and harder to
extend, they worry that they will be blamed for the project slowing down
or that they will be expected to work unsustainably. Developers want to
work in a way that is safe and effective in the long-term. So they focus
their energy on making their software extensible and maintainable.

This perspective is healthy, useful, and also incomplete. 

# Return on Investment (ROI)
Both of these perspectives are focusing on the same concept, Return on
Investment, but with quite different assumptions.

The business is assuming that repeatedly optimizing for short-term
return will yield the optimal long-term return. The Developers are
assuming that the extensibility and maintainability investments they are
making will pay off over time.

These assumption have a critical dependency that even the ROI formula
misses out on...
```
ROI = Return/Investment
```

# Time

Whenever we make investments in our personal lives, we always consider
the time interval that we want to optimize for. We would never purchase
a new house just so we could live in it for one week. We don't rent
furniture that we plan to use for more than five years.

We must consider time when we are make decision where ROI is a factor.
This leads us to the key agreement that Product and Development must
have to optimize the teams investments and the subsequent return those
investments yield.

How do we figure out what time frame we should use to understand our
return on investment? This is an important topic because it is a
decision that the business can make that informs **every** technical
decision we make.

The simplest way for us to discover this information is to ask for it.
We can ask an incredibly simply question that should tell us what we
need to know...


# The Question
***"What time frame is more important than all others?"***

*"Should we go fast this week even if it causes us to go slower for the
rest of the year?"*

*"Is getting the most done for next Quarter's release more important than
maximizing our results this month?"*

What this question does is clarify that in order to go fast this week,
we will need to go slower next week and if we want to get the most done
over the next year, we will need to invest more time this week into
going well.

As developers, we're not making these decisions or even judging which
priority is "right". Instead, we're exposing the business decision that
will inform our technical decisions like how much effort to invest in
refactoring, testing, and experimentation.

Another version of this question is *"What business result is more
important than all others."* This relates to the concept of
[Minimum Viable Product (MVP)](https://en.wikipedia.org/wiki/Minimum_viable_product).

# The Conflict of "Clean Code" versus "Business Results"
Even after we develop a shared understanding of the most important time
frame for the business, there is still more work to do. Unless we have
extremely trustful relationships, the business will still feel tension
about what the developers are working on. This tension is natural and
can also be reduced or eliminated by increasing transparency in very
specific ways.

## Separating Business Concerns from Technical Concerns
During a normal day developing software (or just working in general),
people make hundreds or thousands of decisions about where they invest
their time. This is unavoidable and generally a good thing. We make most
of these decisions autocratically (or with a pair). We don't involve our
team in every list decision we make because we'd never get any thing done.

This is more true of technical decisions (how do I name this variable)
versus business decisions (how should present information to the user).
An important concept is that there are many decisions that are
intrinsically technical.

We don't discuss renaming a variable with
non-developers because *how* we implement a feature is not a business
concern, it's a technical concern. We are making investment decisions
for the business because we have the context and the expertise to do so.

It takes trust to separate these concepts. As a developer, you can earn
trust by being transparent and

### Internal and External Quality

# Have the conversations!