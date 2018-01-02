---
layout: post
title: The Key Question to Ask Your Client
---
#Intro
Software developers and business stakeholders typically have a difficult
time resolving their disparate priorities. I believe that asking one key
question can radically improve how we communicate about prioritization
of work by reframing how we understand return on investment.

#The Business Perspective

The business has a deadline or high priority outcome and is under
pressure to deliver. They are investing significant time, money, and
attention on their project and it is important that they get the most
for their money.

When they see new features working, they have evidence that they are
spending wisely and they feel safe. When they see developers working,
but they don't see new features working, they worry. They don't have
visibility into whether their investment is giving them a return. So
they focus the teams energy on completing features as quickly as possibly.

This perspective is healthy, useful, and also incomplete. 

#The Developer Perspective
Developers want to do the best work they can, deliver lots of value for
the business, and work sustainably. They want to get the best results
for the time and energy they invest in their work.

When they see their software systems getting more complex and harder to
extend, they worry that they will be blamed for the project slowing down
or that they will be expected to work unsustainably. Developers want to
work in a way that is safe and effective in the long-term. So they focus
their energy on making their software extensible and maintainable.

This perspective is healthy, useful, and also incomplete. 

#Return on Investment (ROI)
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

Time.

Whenever we make investments in our personal lives, we always consider
the time interval that we want to optimize for. We would never purchase
a new house just so we could live in it for one week. We would also not
rent furniture that we plan to use for more than five years.

We must consider time when we are make decision where ROI is a factor.
This leads us to the key agreement that Product and development must
have to optimize the teams investments and the subsequent return those
investments yield.

How do we figure out what time frame we should use to understand our
return on investment? This is an important topic because it is a
decision that the business can make that informs **every** technical
decision we make.

The simplest way for us to discover this information is to ask for it.
We can ask an incredibly simply question that should tell us what we
need to know...


#The Question
***What time frame is more important than all others?***

*Should we go fast this week even if it causes us to go slower for the
rest of the year?*

*Is getting the most done for next Quarter's release more important than
maximizing our results this month?*

What this question does is clarify that in order to go fast this week,
we will need to go slower next week and if we want to get the most done
over the next year, we will need to invest more time this week into
going well.

As developers, we're not making these decisions or even judging which
priority is "right". Instead, we're exposing the business decision that
will inform our technical decisions, like how much effort to invest in
refactoring, testing, and experimentation.



#Notes



#Visibility



#Useful ways to think about...
## The Business Perspective
Because humans tend to prioritize
['The Urgent' over 'The Important'](https://www.amazon.com/Tyranny-Urgent-Charles-Hummel/dp/087784092X), we're likely to 
focus on our next deadline at the expense of all other priorities. This makes sense from a reductionist point of view; 
if we complete each part of our problem as quickly as possible then we'll complete the whole thing as quickly as 
possible.
_Tone here seems too formal/mean_
~~What this reductionist perspective misses out on is that our ability to deliver future results are strongly influenced
by how we work right now. This is really just saying the we often choose to incur technical debt, but it's important to 
call this out as a recurring pattern if we want to improve on it.~~

## The Developer Perspective


I realized a couple of years ago that I was failing to ask my clients a key question and that my teams/clients 
were in a lot of pain because our discussions were not aligned with each other. This was especially true in terms of 
investment in "technical tasks" or "refactoring".

The repeated patterns of many projects looked like this:

>The client says, “We need to go fast right now, so don’t {refactor, pair program, test drive, write automated tests}!” 
We’d react by either not doing that important practice or by ignoring our client (or some combination). This rarely led 
to a happy team or client. It certainly was not effective for either.
>
>The client or the team decides that we need to work extra hours this iteration and focus on visible results over 
investing in internal quality so we can “get enough done” this iteration because “it’s the most important iteration of 
the project”. Then we do the same thing the next iteration, the iteration after that, and so on...
>
> ~~Some experienced team members might try to have a conversation with the client about the team being experts at 
building software and the client is not an expert, so the client should just trust us to do a good job. This usually 
freaks out the client because they need these features done ASAP and it sounds like the team is not in any rush to 
actually get finished.~~

Another way we attempt to solve whatever the underlying problem is to try to give the client a different knob to turn 
other than “get more work done this week”. Clients usually feel powerless and the only tool they perceive is to yell 
louder about getting more work done now. We often talk about using velocity to predict how much will get done by a 
certain date and that the client can make business decision about **what** will get done by that date but can’t dictate 
**how much** will get done by that date. This helps some because it shows the client that they have more power and 
control than they thought, but we’re really saying to them, “You’re going to get less than you want.” This also does 
not address that the client still wants us to go faster.

The business decision that our clients can make that will inform both our technical and business priorities is: 
**“What time frame should we prioritize over all others?”**

*Should we go fast this week even if it causes us to go slower for the rest of the year?*

*Is getting the most done for next Quarter's release more important than maximizing our results this month?*

What this question does is clarify that in order to go fast this week, we will need to go slower next week and if we 
want to get the most done over the next year, we will need to invest more time this week into going well.

As developers, we're not making these decisions or even judging which priority is "right". Instead, we're exposing the
business decision that will inform our technical decisions, like how much effort to invest in refactoring, testing, and
experimentation.
