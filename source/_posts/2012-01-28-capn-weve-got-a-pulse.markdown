---
layout: post
title: "Cap'n we've got a pulse"
date: 2012-03-15 20:00
comments: true
categories: self webdev
---
```
$ sudo make me a blog
```
Here's a medium-sized recap of where I've been and what I've done to set the stage for future blog posts.


# &lt;HTML>, PHP - summary of acronym abuse.

Having written my first snippet of HTML 3.2 back in '96 and then after a few years of hand-written html/css and some quirky js I was learned some php and mysql from [Sami Honkonen](http://www.samihonkonen.fi/) and thenceforth I have been programming almost exclusively for the web. I've done php, python, c#/asp.net, ruby/rails, java, javascript/backbone.js/node.js and groovy/grails. A lot of different experiences and ways to build a wheel - but I've invented that wheel quite a few times now.

I am now taking a step away from web development, even tho' the field is full of potential and it is changing at such a rapid pace it would probably be prudent to stick with it and especially master javascript as it is surfacing as the generalist language with which you can do almost anything.

Regardless of the fruit that could be reaped in this field, I feel as though I need to try something new. This is just a matter of personal development and finding interesting challenges.

## e21

I already felt the urge to move onwards from a full-time web development job 2,5 years ago when I was the head tech honcho at [e21](http://e21.fi/) and I told my boss that I felt like I wanted to do something more challenging and new - integrations was one thing I mentioned I had an interest in after I had done some Active Directory and other backend service integrations for [our product](http://www.solubs.fi/). 

During my 5 year stay at e21 I used my rare xslt skills to do some mind-bending functional programming, upgraded the entire IT infrastructure, learned quite a lot of the innards of Windows servers, learned a new language, did a *successful* [Big Rewrite](http://www.joelonsoftware.com/articles/fog0000000069.html) with [Juhani Markkula](http://jums.fi/), helped build a "Adobe Acrobat clone" with Javascript/iText and at one point was, probably, Finland's leading developer in Microsoft's in-house XML/XSLT-based templating system used for a short period on their national site.

I also conducted my first tech job interview at e21, altho' it was a bachelor party gag my friends pulled on me, which did make me wary on the first few actual interviews I held.


## DoDreams

I left the e21 to join [DoDreams](http://www.dodreams.com/) to do a hybrid role of Ruby on Rails/Python/C# developer and sysadmin. I took on new tech in the form of learning about Xen virtualization, integrating our Rails frontend to some propertiery backend game services, administering and troubleshooting our Python multithreaded game hubs. There was a lot to learn and I thrived on the experience and was glad of the challenges.


## Conmio
After a quick break outside of web dev (my role at DoDreams did not include that much Rails frontend work) I joined forces with [Lauri Piispanen](http://www.sunky.org/) at [Conmio](http://www.conmio.com/) where I started my venture into the world of mobile web development. Working with Lauri was a great pleasure since for the first time in very many years I had a stable environment where I had a colleague that was vastly more experienced in the domain than I was. I had never worked with media companies and had done absolutely zero mobile web dev.

I quickly learned that BlackBerry was a four-letter word and that what I had endured in the world of the big pixels with Internet Explorer was not as atrocious a situation as I had previously thought. It was pretty clear that if we could solve our cross-browser problems with a single iefix.css and a hacked in &lt;link/> tag then we would've been on cloud nine. But no. Oh no. Quite far from it. The world of mobile browsers is staggeringly overpopulated with different versions of the same browser, propertiary browsers, applications pretending to be browsers and, lastly and leastly, Opera Mini.

### Webkit != Webkit != Webkit.
**TODO:** Anecdote aboute Android vs Android

### But does it scale?!

One the things that first caught me off-guard was the size of Conmio's clientele. Previously I had done small hobby projects (random visitors/month), small band projects pro bono (100-2000/month), small-medium companies at work (~1k-50k/month) and now I was thrown feet first into the deep-end with the mobile sites of [New York Times](http://m.nyt.com), [USAToday](http://m.usatoday.com) and [Bloomberg](http://mobile.bloomberg.com) - the two latter ones I helped build. I cannot disclose visitor stats, since I named those sites, but I can tell you they are in another ballpark to everything I've worked with so far.

This of course meant getting familiar with high availability setups, sticky sessions, not using sessions if possible, caching (a *lot* of caching) and all that fun stuff you really can't practice for at home or on hobby projects you host on your EC2-small instance.

### Mobile design / UX

One thing that became apparent during the last 12 months of my stay at Conmio was that tablets and higher-end phones deserved and demanded special attention. You could basically do almost anything tech-wise with them as you could do on a desktop browser, but you of course had to take the input and size constraints into consideration when designing the user experience to fit non-desktop use.

One thing that has and is currently breaking through on the UI front is javascript-driven UIs -- using the likes of [Backbone.js](http://backbonejs.com) or [Ember.js](http://emberjs.com). Lauri and I used Backbone quite successfully on a very rapidly developed site where we first did the tablet app from scratch and the iPhone/Android version was basically just configuring the layout while all of the application logic in javascript and backend could stay exactly as-is. I see great promise in this technology.

A technique has also started to stir the design circuits quite a lot and is heavily influenced by people's general lack of mobile design skills: responsive design. I feel that responsive design is nothing new, we've had [fluid layouts](http://forums.devarticles.com/programming-tools-11/what-is-a-fluid-layout-99.html) for ten years now and that "responsive design" is just fluid layouts + having blocks that fall underneath each other or go side-by-side depending on the screen real-estate available. And so far all the examples I've seen of responsive design make it apparent that most people doing it are just trying to make the sites somewhat more usable for smaller screens, but I feel that responsive design cannot beat proper mobile-targeted design. If you are only aiming to serve the iOS/Android market then you can get by with a responsive design, but "just ok" won't [win you awards](http://www.eppyawards.com/Content/Past_2011_Winners-28-.aspx).

## Been there, done that, have the t-shirt

During the latter part of 2011 realized that I had grown quite saturated with web development and the repeating problems I've had to tackle on so many web platforms - pagination, making things line up perfectly, dealing with xbrowser issues, browser quirks, xss, xsrf, sql injection and so on. I decided to look around and see what's available. I looked at openings for project management, team leader, programming, sysadmin, business intelligence, data mining and what have you. I went to job interviews and had some over the phone for in Finland, remote and out of the country work and so forth. But nothing seemed to match. Either the companies seemed fishy or I was not a match to what they were looking or the actual job activies described during the interview did not match what had been written on the job opening, &mdash; _ad nauseam_.

## Relex

Then during a session of Battlestar Galatica Board Game two ex-colleagues from Dodreams (Matias Käkelä and [Iikka Niinivaara](http://www.linkedin.com/in/niinivaara)) told me about their new employer [Relex](http://www.relex.fi/) and what nice a place it is. And after a few weeks of scanning LinkedIn's "jobs you might be interested in" listings to no avail I noticed that one job that it suggested was an open position at Relex. I had a quick chat with Iikka and decided that based on the information I had it was worth a shot.

I sent my application via LinkedIn at around quarter to midnight and at seven AM I had an invitation to an interview and a few weeks later I had a job offer I was willing to sign on. The most important factor was the very versatile role described to me as what I could be and evolve as. A short version of it is "we have to make sure everything continues run - debug hardware, network, database and programming issues".

After two weeks at Relex I am really happy that the job description holds true and I've yet to have a boring day.

So that's my related professional career brought up-to-date.


# Now for something completely different

## StackOverflow

**TODO**

## Anti-piracy vs better service

**TODO**

## BRCM & Silo404

**TODO**
















