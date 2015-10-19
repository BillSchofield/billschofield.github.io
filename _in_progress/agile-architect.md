---
layout: post
title: What does an Agile Architect Look Like?
---

Purpose of a software architect.

Our job is to change existing code so that it is easier for our teams to do the right thing than it is for them to do the wrong thing.

While we work on features that consist of a small amount of code and that take only an hour or two to implement we tend to mentally focus more on code involved in this feature and what we are changing right now

Most of the work that an average development team does is implementing features. We tend to focus on getting the feature working quickly and in a straight-forward way. Often, the expedient thing to do is to add a few lines of code in a convenient place. This place is a seam in our code. A place where it is easy to make a change. If this seam is in the middle of a method then we add our new code in the middle of that method (and maybe extract the code into a well named method). 

While we work on individual features it is easy to miss the forest for the trees. While pairing and refactoring help us understand our code better, we still miss opportunities unless we spend some time working and thinking at higher level of scope. When we do this, we are filling the role of architect. For some people this is a full time job and on some teams individuals take turns doing this. 

 



The structure of our existing code determines where our seams are. If our code has lots of large classes with lots of large methods then most of our seams will be in the middle of big methods and when we make an easy change we will tend to make those methods bigger and more complex. This makes our code worse and adds more seams that are in the middle of large methods.

If our code leans on Dependency Injection (or other behavior decoupling pattern) our seams will tend to be at an interface. For instance, if we want to sort our account numbers in reverse order when our user is from Backwardslandia then we can implement a new concrete class that implements the AccountNumberSorter and inject that strategy when appropriate. We have made our code no worse


I am contrasting the role of an agile architect with two alternatives: the non-programming architect (they do seem to still exist) and the Agile team, where everyone fills the role of architect all of the time.


Thinking at a higher level of scope
Finding large scale conceptual duplication AND doing something about it.
Helping the team increase readability/consistency by solving similar problem with the same tools. Individual programmers letting personal preference win out over consistency with existing code hurts the team.
Our work is about finding opportunities to improve the code and socializing a solution.

Find an opportunity. We find the most valuable opportunities while we are adding features because we feel the pain caused by "sharp edges" in the code the team is actively changing.



