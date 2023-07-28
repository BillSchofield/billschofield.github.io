There’s No Such Thing As Good Code
Bill Schofield, Eric Diamond, and Najati Imam

Target Audience: Developers who want to make better decisions.
Reading time: 5min

You can write readable code that isn't scalable, high-performance code that’s difficult to debug, and a beautiful user interface that’s cumbersome to maintain. Code that’s great in one way could be improved in another. Everyone on your team is going to have a different opinion about what good code looks like, because they all have different assumptions about success.

We advocate that teams understand their stakeholders definition of success and use that understanding to guide their feature implementation.
A difficult choice
While working on a game, Bill faced a difficult choice between two good implementations.

He found a method that was causing long load times, because a string was being instantiated inside of a tight loop slowing the whole method down. Moving the variable declaration outside of the loop massively reduced load times.

Unfortunately, moving the variable made the method harder to read because it now violated Resource acquisition is initialization (RAII).

Did this change make the code better or worse? The method was harder to understand after the change, yet the player experience was significantly improved. Bill’s team decided that this change made sense because they valued user experience even over code legibility.
Defining Success
In order to decide which constraints are more important for a team, they need a good definition of success. It’s important for success here to be defined across the project as a whole, and not within the scope of a particular feature or story. Teams should look to their stakeholders to define that success.

Most teams are good at translating the functional outcomes of their product (e.g. user stories or features) and worse at understanding their constraints, which are often called non-functional requirements(NFRs). We’re going to focus on constraints instead of features because they seem to be a bigger opportunity for improvement for most teams.

Stakeholders and product teams often have very different definitions of done from team members, and understand unspoken constraints or invariants that are critical to the product. For example, it’s reasonable for your stakeholders to assume that every feature is performant, secure, and maintainable (“why would we ever pay for insecure software?”). It’s also reasonable for the team to assume that each feature only includes functional behavior described in the acceptance criteria.

You can stay in sync with your stakeholders by frequently discussing risks with them. Work together to understand:
Which constraints/NFRs are most important for this project?
What’s the cost of ignoring a constraint until later?

The best time to start these discussions is at the beginning of a project; the second best time is now.
Prioritizing constraints
When prioritizing constraints, the order doesn’t need to be strict. It’s just important to have a sense of which constraints carry more weight when you are making day-to-day decisions. Decide whether, for example, security takes precedence over performance, or if maintainability is more important that usability.

After the team has decided how to prioritize constraints, it’s helpful to make them visible so we remember to use them. Having the artifact makes the team agreement easier to introduce into regular conversation and smaller decisions, where tunnel vision can make it easy to forget about the broader context.
Use constraints to make better technical decisions
Every variable you name, class you write, and library you choose is a decision that you’re making about the constraints on our application. Having a shared sense of constraints and their priority can turn every decision into a chance to improve your outcome.

As an example, let’s consider a tech lead writing a method that sends alerts to customers with overdrawn checking accounts. Like many developers, they are trying to write the code in a way that reveals its intention and are considering two options: one based on a filter that selects overdrawn accounts and another based on a for loop with an if statement.

They personally prefer using filters in this situation. However, their team is mostly newer developers. When the team discussed constraints, they decided that making the code more readable for less experienced devs was more important than making it readable for the tech lead. So the tech lead chooses the for loop. They also schedule a ‘lunch & learn’ about filters and first class collections!

Something as simple as choosing between filters and a for loop can be a decision that has broad impact across the team. You can only know which is the right tool for the job if you have enough information to know why one tool might be better than another.
Turn the implicit into the explicit
When people make decisions they base those decisions on assumptions that they usually are not even aware of. By making those assumptions explicit and visible, you allow your team to make more consistent and better informed decisions.
