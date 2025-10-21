---
author: Nick LaLone
date: 2018-11-21 12:00:00 +0800
title: Fantasy Console Class Semester Wrap-up
categories: [Computer Science Education, PICO-8]
tags: [PICO-8]
render_with_liquid: false
---

My first course with PICO-8 as an introductory space for games programming is just about complete. What went right? What went wrong? This post gets into the weeds and explores what I need to change, adjust, and transform.

# Fantasy Console Class Semester Wrap-up

Thanksgiving symbolizes the end of the first semester of my Introduction to Game Programming course using PICO-8.

The course can be found on Github at the link below.
[**nicklalone/CIS---102---Getting-Started-with-Video-Game-Development**
*CIS 102 - Getting Started with Video Game Development …*github.com](https://github.com/nicklalone/CIS---102---Getting-Started-with-Video-Game-Development)

What I wanted to do with this course was twofold:

1. Write a course that allows students to slowly take apart video games at the programmatic level.

1. Scaffold the course so that anyone could take the course and succeed.

I wanted the course to serve as a steward for the complexity of video games. I wanted to use the fantasy console environment so that all aspects of each game could be:

* Made tangible.

* But were easily accessible.

* and were easily playable.

* Above all, I wanted this to be a very multimedia experience.

The multimedia experience was important because in addition to teaching programming at a very basic, introductory, and low-pressure way, I also wanted to address computational those skills that every course demands students have but no course actually teaches. These are often called [basic tech or digital literacy skills](https://www.thetechedvocate.org/8-essential-digital-literacy-skills-students-need/) but I very much dislike this term.

![One of the more complex lessons in this course was getting things to interact with each other AND getting them to trigger other game states like loss of a life, game over, and victory. Much of the work I need to do on the course involves these concepts and I think also is central to learning this stuff in general.](https://cdn-images-1.medium.com/max/2000/1*bRrJnCK01wwek70zgOpceA.gif)
*One of the more complex lessons in this course was getting things to interact with each other AND getting them to trigger other game states like loss of a life, game over, and victory. Much of the work I need to do on the course involves these concepts and I think also is central to learning this stuff in general.*

The result of using the term literacy means that not possessing these skills results in being called illiterate. This is not the case as we aren’t referring to something essential to intelligence like reading but the ability to do things like use a computer beyond its intended status as a medium.

The fantasy console allows users to upload games to a code sharing site, record and post .gifs, load from a clipboard, and work across coding environments and various other media simultaneously. I have found that these environments are some of the most well thought out and executed introductory integrated-development environments for coding that just happen to allow their users to see their work compile before them.

![While this product does an amazing job getting folks into game making, it’s still something on a computer and as a result, you just can’t anticipate what each student’s environment will do to hinder them.](https://cdn-images-1.medium.com/max/2000/1*-opsh62LOBqg4F43RrjfyA.png)
*While this product does an amazing job getting folks into game making, it’s still something on a computer and as a result, you just can’t anticipate what each student’s environment will do to hinder them.*

## So what went right?

I based this course off of the amazing work of [Krystian Majewski](https://twitter.com/krystman). His walkthrough of Breakout Hero was a huge inspiration for this course. The big difference between he and I is that i’ve never worked as a coder and my coding skills themselves are not near as high as his. As a result, I am much closer to my students than he could ever be. This is an essential component to teaching introductory programming I think.

In fact, in watching Krystian’s work, I began to think about how to integrate some of the [software carpentry](https://software-carpentry.org/) content into what he was doing and providing a lot more scaffolding for the students in the course. While I recommend engaging the [software carpentry](https://software-carpentry.org/) website, this video provides a ton of inspiration.

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/kmVKGxPlTvc" frameborder="0" allowfullscreen></iframe></center>

That said, Breakout Hero is a fantastic tutorial. The reason I chose this playlist was 2-fold. First, it presents high-level development from origin to completion to release. Second, as you go through the videos, you can see the difficulty result in folks getting frustrated and giving up. The result is that the last video has so few views that you cannot help but feel bad. It is like watching the leaky pipeline in action. This is not the fault of Krystian insomuch as it is the result of the obtuse, inaccessible aspects of programming itself.

Sure, we could all learn to do programming; however, have you ever actually tried to do programming? It often sucks a lot.

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/YQzwVDMIfyU" frameborder="0" allowfullscreen></iframe></center>

But it doesn’t have to. In fact, what I wanted to do for this course was to create an environment that increased complexity steadily, but more slowly than normal. It seems to have worked for about 80–90% of the 25 online students I had.

I think my favorite comment I got this semester was (paraphrased):
> “I felt like I was just given a toolbox and a palette and objectives each week on “The Joy of Programming with Nick Lalone”

And other comments from students at the end of the semester followed the same sort of positivity that I had not expected. The most common response I got in the narrative files students submitted at the end of the semester was, “I never knew how much went into video games! While it is obviously more complex than what i’m doing, I can see how it all fits together!”

And that realization in addition to the increased exposure to the games people have made was incredible. Multimedia use increased exponentially for each student. Additionally, I asked them to upload games to the [lexaloffle carts page](https://www.lexaloffle.com/bbs/?cat=7#sub=2&mode=carts). Because the community there is so welcoming and helpful, many of my students found answers to questions from folks commenting on the games themselves.

All in all, it was so satisfying to see this collection of exercises welcomed with so much enthusiasm. But it was not all good.

![No matter how much you try, someone always jumps into a missile…](https://cdn-images-1.medium.com/max/2000/1*QIVqZJ0BrDyMnlUyrnolFA.gif)
*No matter how much you try, someone always jumps into a missile…*

## So what went wrong?

One of the issues with teaching programming is that we’re very bad at it. While there are significant resources out there, they all presume those “tech literacy” skills. I think the thing that frustrates me the most is that so many introductory course on programming assumes from the outset that students are at a level that is neither introductory nor would be in the course.

While this seems obvious, it is a frustrating blind spot for faculty who have been engaged in computation at high levels for so long that they cannot remember how they even began to get there. I am no exception to this despite not being a professional coder.

While I tried to approach this space as though the student had never considered programming at all, there were some things that I did not consider. I also did not anticipate outside influences.

### Anti-virus software

PICO-8 is an extremely small program that requires very few resources. It is so small and light and simple that it is only 11.4 megabytes. It can be loaded on all sorts of devices and have even started to see folks try to export it all to floppy discs and Commodore 64. But it is this lightness that can provide something difficult for folks who are not used to working with computers.

Throughout the semester, around a quarter of the students emailed me in a panic about PICO-8 getting uninstalled and quarantined by their anti-virus software. There isn’t much that I can do about this other than to tell them to either add an exception or uninstall the anti-virus software itself. Interestingly, those same students did not know how to do either of these things.

This has lead me to start trying to outline a video on common problems and ways to solve them.

![How to deal with this in a course not about this without being able to see the machine, the student, or the issue. How to triage a student’s problem with a computer when the computer is needed to communicate?](https://cdn-images-1.medium.com/max/2000/1*TXS7PQGiLvOQi7UTnj9cIA.gif)
*How to deal with this in a course not about this without being able to see the machine, the student, or the issue. How to triage a student’s problem with a computer when the computer is needed to communicate?*

### Collisions

The most difficult aspect of coding is getting two objects to interact with one another. In Krystian’s tutorials, he spreads this out amongst 3 obtuse and difficult videos that cover nearly 2 hours of video. If you dig in to other video tutorials, they glaze over this point saying things like, “Just do this, simple!” And it makes sense because this is the single most difficult aspect of coding like this that I can think of.

When I sat down to do record my own version of this, I started to outline the code and video I was going to make and it was probably going to be over an hour. I tried to make many of the tutorial aspects of my videos less than 30 minutes each. So, when I started to record these videos it took me probably more than 3 or 4 hours to really get it all right.

I ended up adjusting the entire structure of the course so that I could spread collisions out between 2 different weeks. This resulted in pushing “game states” into a seemingly throw away video which then started to cascade failures across almost every student’s game.

The correction for this is simple though as I changed the content in a live course. Future students will not see those changes. Instead, the content will be set up that way and shouldn’t provide any issues.

### The Problem of Growing Programs

The general path of this course is to:

1. introduce variables,

1. create a ball,

1. move the ball,

1. create edges to bounce the ball off of,

1. create a paddle,

1. move the paddle,

1. get the paddle and ball to react to one another,

1. get the paddle and ball to bounce off each other,

1. add game states like victory and loss,

1. add sound,

1. add levels,

1. Juice it up!

1. Polish and submit.

By around the introduction of game states, it is no longer possible for students to ask the question, “This doesn’t work, can you help me?” The games are now so long that it will take a lot longer to debug the game than the time any professor will have.

This results in a bit of frustration when those students ask for help by saying, “It’s broken” but not getting any help because no person, no matter how helpful they are, can actually help them. It is such a frustrating problem that I have been considering altering the “juicing” content to “how to ask technical questions” or something like that.

### What to Change?

There is a lot to change. Generally, I want to add 3 distinct modes for students to declare at the start of the course:

1. **Normal Mode: **An introductory path where students take the code of the course and comment each line so they get used to reading code.

1. **Difficult Mode: **The way the course is now where students make Breakout! and then are given a choice to make something else.

1. **Expert Mode: **An expert path where students make their own content with high stakes grading.

But I am hesitant about this. My hesitation stems from putting folks who have had previous programming training on display. What might work there then is asking **Expert Mode **students to submit their content to the faculty member directly.

This has the benefit of keeping the expert content away from the new students while also making the **Expert Mode **students feel like they have a more direct line to faculty of record. For **Normal** and **Difficult **mode students, I think there shouldn’t be too much difficulty with those humans to interact with each other. Additionally, I think i’d offer that while students cannot move down in difficulty, they can decide to move up.

But ultimately, I wonder if it’s worth the hassle. I think I need more data. There is always a need for more data!

Given all of this, I wonder about what the next course could be. I have found myself wondering about:

* Teaching game design concepts.

* Teaching game design philosophies.

* Teaching more advanced programming methods.

* Ultimately merging those concepts in some way.

To date, I don’t know that i’ve seen a curriculum that does this. Instead, I see some interesting intro courses that eventually get impatient or need to catch up to some sort of programmer’s ability later in the program and so that careful scaffolding is suddenly moved away by an Angry Bird with little to no empathy about how precarious the situation truly is.
