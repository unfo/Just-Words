---
layout: post
title: "Caring and vested interests"
date: 2012-07-31 21:45
comments: true
categories: 
published: false
---

# Caring and vested interests

**Caveat:** Most of my experience and my close friends' experiences are from small-medium companies, not giant corporations that can just throw >resources> at problems.

One of the most difficult things in all of software development is task management when $number_of_people > 1.

We have people whose only job is to babysit other people's tasks and making sure they get done in the right order even if today's right might be tomorrow's left.

The main reason this is a big problem in our industry is that tasks are almost exclusively wholly virtual: written atop a 30 email long FWD:RE:RE:RE:FWD:RE thread, input into a specific app made for tracking tasks like Trac or JIRA, or - worst case scenario - present only in the minds of the tasker and taskee.

<!-- more -->

If you go to a shoemaker and just keep piling pairs of shoes upon another it has a concrete effect on the real world. You run out of either space or common decency.. And there is no chance that either the shoemaker or his manager and/or front-of-house will ever forget or misinterpret the amount of work still left undone.

On the other hand if you are a local musician’s manager and keep getting people coming into your shop requesting "I want you to compose me song to cheer me up" who are willing to pay for that you might end up with an ever increasing queue of songs to compose without any sort of physical manifestation of whether this request is a bigger than that.

As the musician's manager you might start to develop a good sense that 'a happy song' takes 5 days and 'fusion jazz with a mix of reggae and trip-hop' takes 3 weeks and up and thus you can start giving clients some sort of estimations on when they could perhaps start expecting their song to be done.

For most of the time I've been involved with most of the people, myself included, have had a kind of a mass delusion that software engineering &mdash; with emphasis on **engineering** &mdash; is more akin to the former job instead of the hap-hazard, messy, touchy-feely world of creative art.

I would venture to postulate that this might have something to do with the ancestry of our field where the highly educated and very smart mathematicians and physicists were the pioneers of using computers for, well, computing equations and such with very, very strict time limits and requirements. And so we, the grandson of the Grand Duke of Hyperion (only 14 generations down and four times removed, and nevermind that thing with the cousins) believe that the blood of the Ancient Royalty still beats coldly in our veins.

It does not.

We are that musician and his manager. Our manager has two options with regards to payment: a set fee upon completion or an hourly price. Well how long will any given song take? No idea. Well a fixed price then. Fixed at what price? No idea. Make something up?

When the manager finally sets a price it is up to the musician to make it profitable &mdash; only you cannot push creativity.

And now to stop pushing my analogy till it breaks totally.

## What you asked for, when you wanted it and a low price!

Cake: ( ) Have it, ( ) Eat it.

So back to the subject of tasks and how they are so darned stealthy lil' critters! When you have a straight R&D house building a single project and nothing else things might stay reasonably well within parameters for sanity. But when that single project is first released to the wild and is found lacking you find that developers start to have divided priorities: make new stuff vs fix old stuff.

Add to this the troubles you face when you start writing (custom) features based on a single client just because of their impact on your bottom line. This will lead to some people having more in-depth knowledge of this feature than others and, voilá, you just added another divided priority.

Continue this for a few moments and you will have people with very hazy priorities that are mostly colored by their own motivation which might not align with the Correct priorities set by a manager. And those Correct priorities might not align with the **other** manager's view of Correct.

Skip a few iterations of Where's My To-do stickers and Wheel of Misfortune and this will end up in "let's make/buy an app for this".

> Q: What's the most important part of a to-do app apart from being able to tell who's ticket this is?
> A: **Priority**

Fast-forward a few months and you will have 80 tickets in High, 30 in Normal and 5 in Low - and 5 out of those 5 were the devs' own tickets.

Is 80 tickets much? It depends.

Maybe you've agreed that anything more complex than a few hours' work should be split into simpler tickets.

Well phew, that's just math and I have a calculator in my phone!

$ 80 x 2 = 8 x 20

So that's 20 man-days and we just happen to have 10 __engineers__ so in two days everything is settled and done! Yay!

Right.

All developers I know have been faced with a bug report that at first seems like it's a typo somewhere but ends up needing a re-write of one of the core modules.

> Bug report: When I do X I get 3.13 as the result instead of 3.14.
> Original estimate: 0.5 hours
> Actual time: 0.5 hours
> Resolution: Changed the rounding options in file X.

It could've as easily have been:

> Actual time: 53 hours
> Resolution: The fourth level dependency of this library we use to do Y in our software has a problem with IEEE floating point numbers and it had to be recompiled against the production server's ancient headers by hand which failed because of Z and then we needed to reimplement some of the API because of a version mismatch.

The point is you can rarely truly know.

> Q: What the hell does caring have to do with any of this?
> A: **Quality**.

Caring leads to commitment and commitment can lead to either great quality or not caring anymore.

Not caring leads to lack of motivation, lack of motivation leads to either shitty quality or burn-out.

The key factor here is the whether the developer feels like he is getting as much commitment and good vibes from the company/managers as he is putting out there.

If you have a caring developer who commits and gets rewarded both in financial terms as with joys of the mind for his work it will lead to great quality work and a very healthy and, probably, long-lasting mutually respecting relationship. Yay.

If you have a caring developer who commits and just gets asked for 'a little more', 'just temporarily', 'just this once', 'until X happens' day after day it will lead to a plummet of personal motivation or &mdash; if the dev committed enough to weather any storm &mdash; to even more attempts to get rewarded which would eventually justify his spending so much of himself.

There is only so much a single person can give. If you are still burning your energy at full blast when you run out of fuel you will crash quite hard and end up in burn-out mode. If you happen to notice the blinking light on the dashboard and see your energy levels depleting it is possible to do an emergency jetting of commitment, caring and motivation - to cut loose - and it just might save you from having to recoup as heavily as a full blown burnout requires.

Regardless of how you got to the 404 page of motivation dot com, the quality of your work just took a big nose dive. Should your work ethic so suggest, it is still possible to do decent quality work if required, but it just takes vast amounts of energy.

The most common route to not caring is when your own interests do not align with the company's interests.
When you have vested interests it simply put means that whatever is the best thing for **yourself** to do is also the best thing for the company.

This boils down to: if what you do **directly** affects the company bottom line in a positive manner then you have vested interests.

Note the directly. If your work is indirect with regards to the bottom line then it is much easier to have misaligned agendas.

I can give you both a negative and positive example from my own work history.

Before the examples, I must point out that I am at heart very customer-oriented. And not in just as a CV filling positive adjective. I really do care that the people I am building stuff for get the best possible experience. 

When I was doing web dev the main beneficiary of my efforts was the client and they were thus more likely to stay with us and that affected the company's revenue stream. I had an indirect effect.
And because it was indirect, it was quite impossible to measure in any short-term manner and in the long-term there were so many confounding variables as to ruin any chance of being able to say "if we do this half-assed then there's an 1.5% increased risk of losing this client worth X EUR".
So it was not possible to compare getting a better margin for the billed hours **now** versus potential loss of sales in a year or two's time. So even though I would like to spend more time fine-tuning the UI or database stored procedures there just wasn't any money to be made.

As I mentioned in my first post since this blog's resurrection: I am no longer doing web dev. And seeing the above way of operating quite wide-spread was one motivator to try something different. (**Note:** Not all projects were like this, but an unfortunate amount encountered by myself and my friends in numerous companies across many countries.)

Today I am in a happy situation, that I can use as an alternative example:
Our company makes a product that directly generates savings to the client and a certain cut of those savings is what our company gets. Well that's the simplified version at least.

So at the core: any way that I am able to make the system better or run smoother will generate more savings to the client and thus more revenue for our company. Thus I have a vested interest with the company to do my best.

And **that** makes for a very opportune place to have high quantities of caring and commitment.
