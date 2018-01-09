---
layout: post
title: Helping the Business Understand the Value of Specific Tech Tasks
---
# Helping the Business Understand the Value of Specific Tech Tasks

When the business asks questions like, *"What are you working on?"* they
are usually trying to understand *why* developers are choosing their
current work item. They are seeking visibility into how you
are investing time.

Often the answers to these questions from the business lead to clumsy
and uncomfortable conversations. The developers feel unfairly judged and
the business feels powerless.

An effective way to avoid this situation is for the developers to do the
work of understanding the *why* behind the work themselves. If we don't
understand the business value of the work we are doing, then we can't be
effective technical representatives of the business.

## How To Do It

For each of the non-trivial "Tech Tasks" you want to work on, ask
yourself [*5 Whys*](https://en.wikipedia.org/wiki/5_Whys). It's likely
that you will discover how this work could make sense to the
business. The *5 Whys* is a Six Sigma technique for Root Cause Analysis
and that's similar to what we want to understand about these Tech Techs.
We want to understand the core business value behind this work.

Once you can explain the business value of this Tech Task, you
can either work with the Business to prioritize it as a Tech Task or
even reframe it as as User Story.

## Example of 5 Whys
> I want to refactor this class.

**Why?**

> So our code easy to test

**Why?**

> So we write more automated tests

**Why?**

> So we find defects quicker

**Why?**

> So we have fewer defects

**Why?**

> So we reduce our time to market


## Reframing Tech Tasks as User Stories
I'm not yet convinced that we always (or even often) want to rewrite
Tech Tasks as Stories, but this is a technique to try if you want to
invest in improving communication between developers and the business.

[Mike Cohn says that user stories](https://www.mountaingoatsoftware.com/agile/user-stories)
take the form:
> As a `<type of user>`, I want `<some goal>` so that `<some reason>`.

Getting these three parameters right is critical to using Stories successfully.

We can't know the ***what*** (`<some goal>`) or the ***why***
(`<some reason>`) until we understand the ***who*** (`<type of user>`).

Our choices are usually `As a developer` or `As the product owner`.
If we look at the *5 Whys* listed above, we see that the topmost answer
is from the developer perspective and the bottommost is from the business
perspective and the answers in the middle are a combination of the two.

If you intend to write Tech Tasks for stories, I'd advocate for having an
Epic User Story or Theme that relates to the highest level answer and have
the finer grained stories be written more technically. This allows us to
honor both perspectives while still being able to capture simple Acceptance
Criteria.

#### The Epic
We can write the epic story for our example as:

> As the product owner, I want to reduce our time to market, so that we get
more rapid feedback from our customers.

#### The User Story
> As a developer, I want to refactor this class, so that our code
is easier to test.

At this point we could choose to stop writing stories and just get to work.
We could also create tiers of stories, on for each level of the *5 Whys*.
Each tier of stories would be the `so that` clause for the level of stories
below it.

## Have the Conversations
The real key here is to have the conversations between developers and
the business where you truly try to understand the perspective of the
other and you work hard to present your perspective in a language that
the other can easily understand.

