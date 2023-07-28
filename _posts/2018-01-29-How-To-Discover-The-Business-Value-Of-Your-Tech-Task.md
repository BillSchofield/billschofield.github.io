---
layout: post
title: How to Discover the Business Value of Your Tech Task
---
*This is Part 1 in a series about improving communication between
programmers and the business.*

Audience: Programmers and Project Managers

Estimated Reading Time: 4 minutes

---

Software development teams often face significant challenges with 
inter-role communication. I've noticed a recurring pattern of programmers 
wanting to focus their energy on changes whose value is difficult for
the business to understand. We often capture this work as Tech Tasks and
prioritize it based on how vocal people are, not on its return on
investment.

### The Problem
When the business asks questions like, "What are you working on?", they
are usually trying to understand *why* programmers are choosing their
current work item. They are seeking visibility into how the team is
investing time and the business' money.

Often the answers to these questions lead to clumsy and uncomfortable
conversations. The programmers feel unfairly judged and the business feels
powerless to steer their project.

### The Solution
An effective way to increase the effectiveness of these situations is
for the programmers to share the *why* behind this work with the business.
If programmers don't understand the business value of the work they are
doing, then they can't understand the Return on Investment (RoI) of the
Task and thus can't safely prioritize it for the business. If developers
can discover the business value of these Tech Task by asking
themselves, "Why?", then they can share this information with the
business and work with them to prioritize these Tasks the same way the
team does User Stories.

### How To Do It
We are seeking the core business value behind our technical tasks. To
discover this value, ask yourself [*5 Whys*](https://en.wikipedia.org/wiki/5_Whys)
and your answers will lead you to the value this Tech Task provides to
the business.
The *5 Whys* is a Six Sigma technique for Root Cause Analysis
and the root cause of our desire to do this Tech Task is what we want to
better understand.

Once you can explain the business value of this Tech Task, you
can either work with the Business to prioritize it as a Tech Task or
even reframe it as as User Story.

### Example of 5 Whys
Suppose while you're in the process of finishing your last User Story, you discover
that it was difficult to test interactions between the `Order` and `Customer`
classes. In particular, it is difficult to "add" an `Order` to a `Customer`
and you believe the solution is to fundamentally change how `Customers`
interact with `Orders`.

> I want to refactor the `Customer` class.

**Why?**

> So our code is easy to test

**Why?**

> So we write better automated tests

**Why?**

> So we find defects quicker

**Why?**

> So we have fewer defects

**Why?**

> So our product is more usable

### Reframing Tech Tasks as User Stories
If you want to invest in improving communication between programmers and
the business, you can write your Tech Tasks as User Story.

[Mike Cohn says that User Stories](https://www.mountaingoatsoftware.com/agile/user-stories)
take the form:
> As a `<type of user>`, I want `<some goal>` so that `<some reason>`.

Getting these three parameters right is critical to writing great User Stories.

We can't know the ***what*** (`<some goal>`) or the ***why***
(`<some reason>`) until we understand the ***who*** (`<type of user>`).

Our choices for the ***who*** are `As a programmer` or `As the product owner`.
If we look at the *5 Whys* listed above, we see that the topmost answer
is from the programmer perspective and the bottommost is from the business
perspective and the answers in the middle are a combination of the two.

If you intend to write Tech Tasks as User Stories, I'd advocate for having an
Epic User Story or Theme that relates to the highest level ***Why***. This means that
the Epic is written in purely business language. Next, we can write finer grained
User Stories that are written using more technical language, but still have a
"So That" clause that relates to a business concern.

This allows us to honor both perspectives while still being able to capture simple
Acceptance Criteria.

#### The Epic
We can write the Epic User Story for our example as:

> As the product owner, I want my product to have fewer defects, so that
my customers find it more usable.

#### The User Story
> As a programmer, I want to refactor the `Customer` class, so that our code
is easier to test.

#### User Story Hierarchy
At this point we could choose to stop writing User Stories and just get to work.
We could also create tiers of User Stories, on for each level of the *5 Whys*.
Each tier of User Stories would be the `so that` clause for the level of User Stories
below it.

These hierarchies are more useful for clarifying the business value of
Tech Tasks and Non-Functional Requirements (aka Cross Functional
Requirements) and are generally not helpful for conventional stories.

> * Usability - As the product owner, I want my product to have fewer defects, so that
my customers find it more usable.
* Quick Defect Discovery - As a Quality Analyst, I want to find defects quicker, so that we have
fewer defects.
* Test Automation - As a Quality Analyst, I want better automated tests, so that we find
defects quicker.
* Easy to Test Code - As a programmer, I want our code to be easier to test, so that we
write better automated tests.
* Refactor Customer Class - As a programmer, I want to refactor the `Customer` class, so that our code
is easier to test.

#### Tags
We can also tag our User Stories with all of the Themes or Epics that they
support.

> As a programmer, I want to refactor this class, so that our code
is easier to test.
>
> Tags: Usability, Time-to-market, Maintainability

### Have the Conversations
The real key here is to have the conversations between programmers and
the business where you truly try to understand the perspective of the
other and you work hard to present your perspective in a language that
the other can easily understand.

