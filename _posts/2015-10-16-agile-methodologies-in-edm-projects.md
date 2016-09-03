---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
keywords: []
description: Everybody loves Agile. Right?
datePublished: '2016-08-31T20:19:15.287Z'
dateModified: '2016-08-31T20:19:14.834Z'
title: ''
sourcePath: _posts/2015-10-16-agile-methodologies-in-edm-projects.md
authors: []
publisher: {}
author: []
via: {}
starred: true
url: agile-methodologies-in-edm-projects/index.html
_type: Article

---
Everybody loves Agile. Right?

I see it every day. The Scrum Master opens the daily ceremony with a flourish of his Sharpie, and we're off! What we did yesterday! What we're going to do today! Roadblocks eliminated, index cards flying across the board, six fully coordinated project teams passionately iterating in glorious Fibonacci sequence! Productivity emerges as an inevitable by-product of the self-actualized, optimally-sized, relentlessly upward spiral of lather-rinse-repeat!

_Woo hoo._

Now, sitting on the other side of the room---next to the grown-ups in suits who write the checks---is your senior EDM Engineer. He thinks Scrum is fun, too, but he's wearing a frown because he's already aware of something that the Scrum Master may not notice for another five or six sprints, and he's trying hard to figure out how to deliver the message without dampening the enthusiasm in the room.

The message is this: **there's no such thing as a free iteration**.

The [second principle of the Agile Manifesto][0] is this: 
> 
> Welcome changing requirements, even late in development. Agile processes harness change for the customer's competitive advantage.

That's powerful stuff! It gives a team permission to miss the mark, especially if it gives the client a solid piece of ground to stand on while aiming for a _better _mark. It's the difference between a sniper's bullet (which is only aimed once) and a guided missile: mid-course corrections can turn a miss into a hit almost every time.

Like a guided missile, though, a project's capacity to change course is limited. In rocketry, that limit is a function of _inertia_: the faster a missile is moving---and the more massive it is---the more force its control surfaces must exert to track its target. Eventually something breaks. Inertia applies to software development as well: some changes are harder to make than others, and **a project team that gets the easy stuff right on Day One, but iterates on the hard stuff sprint after sprint, will quickly find itself running at top speed just to stay in place**.

So two questions then:

1. How to identify sources of inertia in a project?
2. How to apply agile principles in a way that _accounts _for inertia?

I think the best answer to the first question is easy: _ask someone who knows_. Seriously. They probably learned the hard way. Don't repeat their mistakes.

I know Enterprise Data Management implementations. And I can tell you right away what some of the major sources of inertia are in an EDM project:

There are people who know how to do all of these things. I'm pretty sure I know all six of them. But knowing how to _do _a thing and getting a client to _prioritize _a thing are not at all the same animal. Particularly when none of these efforts---and each of these is a multi-sprint affair---is going to move the ball an inch closer to whatever goal line the business has set for your project. 

So listed above are three double-whammies. At any but the most forward-thinking of firms, there isn't even a hint of a requirement for any of them. Yet _not _having them---and, let's be honest, _none _of the major EDM products ships with this stuff---makes literally everything the development and test teams do take an order of magnitude longer than they might. For developers accustomed to NUnit and Git, it's like skin diving in quicksand with a cocktail straw for a snorkel. 

Sub-optimal.

Clearly we can identify sources of inertia in our projects: the bits, present or absent---or, bless you, the people---that just make everything more ponderous. I know mine, and if you don't know yours then you should get off the Internet and go find out, because whatever it is you do, they're with you.

So what to do about it? We're already Agile, and glad of it. And the heart of Agile is iteration. Yet, at least in the EDM world, we can identify a handful of issues that, until they are fixed, make every iteration more difficult. Slower. Less productive. It isn't that the work is harder, but that the process of iteration _itself _is too costly.

Examples help, so here's one: I want to tweak my table naming convention, rename a bunch of tables. In Visual Studio, I've got a bunch of tools that could do that for me, across the entire project, in a couple of mouse-clicks. But in everybody's favorite EDM tool, well, not so much. I'm going to spend days rebuilding components to reflect the new table names, and hours more propagating the changes to the edge of the blast area. So if I wanted to get anything correct, right off the bat, naming conventions would be a pretty good candidate... and having a robust tool to track the specification and implementation of low-level requirements would go a long way toward ensuring that my naming convention actually gets implemented as specified, the first time around.

So the second question above easily translates to: **when your Agile project is suffering from inertia, how do we use Agile to _fix _Agile?**

Let's go back to that Scrum meeting. At the same moment the senior EDM engineer is pondering sources of friction, the Scrum Master is asking the team to identify roadblocks. And the EDM guy is probably going to sit on his hands, because although those sources of friction will certainly _become _roadblocks, they aren't roadblocks _yet_. At least, not as much as the test lead's unexpected long weekend, which begins this afternoon right in the middle of regression testing.

Now some roadblocks are immediate, obvious, and can be Scrummed around before the end of the sprint. But others are subtle. They're systemic. And by the time they graduate from _potential _roadblocks to _actual _roadblocks, fixing them will be an order of magnitude more expensive than it would have been early on. As issues they are low-urgency but high-impact, and there exists no business requirement to support addressing them one way or the other. But---are you listening, senior EDM engineers?---_there should be!_

And that's the key.

Any competent engineer can build a system that fulfills his client's requirements. That's the _definition _of a competent engineer. But a lead engineer, operating in a consultative mode, has to do more than that. He has to go beyond confirming that he can build to the client's requirements and address the requirements _themselves_. **He has to be willing to get up on a table---metaphorically, usually, but I've done it for real---and make the most powerful case he can for what he believes his client's requirements _should _be.**

All my most successful EDM implementations have been Agile. And the most successful of those have started with a critical review of the client's high-level requirements, generally resulting in the addition of a few my client didn't know they needed until I explained why. And then we spent time---often several sprints---building to those new requirements, generally before writing a lick of code intended to move enterprise data around.

**We started by writing user stories that treated the development team as clients of their own platform**, and expressed the frustrations they were sure to experience if they allowed those potential roadblocks to establish themselves. Then we designed our way out of the problem, iterated until we were satisfied, and _then _got on with the business of managing enterprise data.

And all those hours we spent removing potential roadblocks? You know the answer: we got all that time back, and then some, because---wait for it---_we never had to deal with the actual roadblocks_. 

Sweet.

Along the way there were some tense conversations with the business. After all, deadlines are deadlines, and nobody wants to watch a million-dollar team moving sideways when the clock is ticking. But that's what a good consultant does: you make a solid case for what you know to be the right approach, you stick to your guns, and when your reluctant client profits by your persistence, you make the biggest deal you can about what great decisions they made.

Of course you'll wind up doing it again in six months when the next potential source of friction shows up on your radar. But having successfully demonstrated the virtue of identifying and neutralizing that stuff early rather than late, you're likely to find your client much more receptive to your ideas the second time around.

Now _that's _Agile.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/d2a2e937-56c7-473d-af2a-5b13cf11383f.jpg)

[0]: http://agilemanifesto.org/principles.html