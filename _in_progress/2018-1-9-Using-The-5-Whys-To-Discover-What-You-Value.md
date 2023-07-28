---
layout: post
title: Using the 5 Whys to Discover What You Value
---
This is a follow-on post to
[Helping the Business Understand the Value of Specific Tech Tasks]() and
will be easier to understand if you read that post first.

## Example of '5 Whys'
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

## Relating Technical Decisions to Value Statements
As we ask '5 Whys' for many Test Tasks, we'll discover themes to the
answers we give ourselves. They might be "Reduce Time to Market" or
"Go Faster in the Future". We could even create a hierarchy of these
answers.

* We can go faster in the long-term because...
  * We have fewer defects because...
    * We find defects more quickly because...
      * We have more automated tests because...
        * We keep our code easy to test.

* We get results quickly now because...
  * We can put all of our effort into features because...
    *  We don't prioritize Tech Tasks


Both of the root statements are positive. We want both of them even if we
can't usually have both of them.

Using the model of the [Agile Manifesto](http://agilemanifesto.org/)
"this over that" value statements, we could write value statements like:

> We value **Getting Results Quickly Now** even over **Going Faster in the Long-Term**


Why? Because...
How? By..