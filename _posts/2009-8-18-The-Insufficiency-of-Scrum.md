---
layout: post
title: The Insufficiency of Scrum: The Importance of Internal Quality When Practicing Scrum
---
*I originally posted this in 2009 without the sub-title and received a lot of feedback that helped me understand that my title was leading readers to think that I am anti-Scrum or anti-Agile. For context, I am a long time agile zealot and think that Scrum can be a great agile introduction or transition for non-agile teams.*

Scrum is often promoted and adopted as a holistic software development methodology. It simply isn't. It doesn't help us manage our project goals, and it encourages us to build software that grows increasingly hard to change. Scrum is great at what it is intended to do, but it only provides a subset of the Agile practices we need to succeed.

Scrum fails to acknowledge the entire scope of software development. To demonstrate this, I'm going to break down the levels of scope the same way Scrum does.
Project: This is about deciding what the project goals are and steering towards those goals.
Milestone: This is a sub-interval of the overall project in which part of the project is delivered.
Feature: A change to the software that has value to the client. This is often described as a requirement or user story. Features are usually intended to fit within a single Milestone.
Scrum does a great job of addressing the Milestone level of scope but mostly punts on the other levels.

Project
At the project level, Scrum calls for a product backlog, but doesn't describe how to create or manage the backlog. The benefit of this is that it helps projects transition from the expensive Big Design Up Front of Waterfall. The major drawback is that many teams feel they can change the direction of the product without cost, because Scrum largely ignores that cost.

Milestone (Sprint)
This is where the heart and soul of Scrum lives. It teaches teams good habits with regard to dynamic steering and continuous improvement.

Feature (User Story)
This is where Scrum breaks down. It focuses entirely on finishing the user story (as defined by the Product Owner at the beginning of the Sprint). While this is a good contrast to development that is focused entirely on creating 'systems' as defined by programmers, it does not do a good job of honoring the complexity of software development. In particular, it doesn't account for the cost of removing duplication in code, data, or concepts. This leads to 'code debt', which means future features will be more expensive to implement than they need to be.

Dissonance
Scrum tells us that we can steer projects as though they were speed boats while allowing us to turn the project into a barge. At the project level, we are told that changing our project design is as easy as changing the backlog. At the feature level, Scrum encourages practices that make changes to the project become more expensive as each feature is completed.

The Story
Some well intentioned person in product management, looking for ways to improve their process, discovers Scrum. It is the answer to their prayers; no more late projects that don't perform the way the client expects!

Three of the managers from the team go to a couple of days of classes and become Certified Scrum Masters. Now they know what they're doing! As the new project is ramping up, they teach everyone on the team how Daily Scrums, Sprint Reviews,and Sprint Planning meetings all work and everyone starts doing them.

Everything goes great: valuable features get finished, the product backlog changes without a hiccup, and the team spends much less time planning and writing documenting while spending more time making progress.

Some time passes...

Things are a little tougher now. Programmers occasional mumble about re-factoring, engine work, etc. They ask to work on things that are clearly not user stories. Some features start slipping, or are perceived as 'hard' where just a month ago they would have been easy.

More time passes...

Things are definitely worse now. Most estimates are higher than the Product Owner expects. People are falling back into their old development patterns (e.g. wanting to write a technical design before they will make an estimate). Bug counts are increasing. What used to be easy is now hard.

The Advice
Ensure that there is resonance between the way you plan the project and implement the features. While there is the Scrum layer between them, they are still tightly coupled. For example (and this is not what I recommend), if you use Waterfall to build your product backlog, then you might want to have your programmers do more Big Design Up Front so they can benefit from the large amount of project planning that you did up front.

An example of good resonance would be:
Project planning using Agile Estimating and Planning by Mike Cohn
Milestone planning with Scrum
Feature implementation with Extreme Programming (XP)
All three of these methodologies are Agile, and support the flexibility and discipline of the others.
Agile project planning is still in its infancy, but Agile Estimating and Planning will get you started on the right foot. Remember to take care when you steer your project, because change is rarely free. Make sure that you integrate all relevant perspectives before you make a significant change to your product backlog. 

Get the right developers, product designers, and client in a room and let them candidly discuss the change. Ask the developers what changes they think would be good to make. They know what is easy to change and probably have a pretty good idea of what is valuable to you.
Extreme Programming is a great match for Scrum (they even share a lot of the same practices). XP has two main effects on a project:
The programmers get better at programming faster than they would without it.
Change in project direction is less painful because the software itself is easier to change.
XP also fixes some of the outdated concepts in Scrum by bringing the client and developers together and by allowing user stories to change as soon as the client realizes they should.

Scrum is definitely an improvement for many projects, but you should not switch to it lightly. Make sure you understand how it fits together with the way you plan projects and the way your developers implement features.