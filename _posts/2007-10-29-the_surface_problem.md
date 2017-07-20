---
id: 111
title: The Surface Problem
date: 2007-10-29T16:24:10+00:00
author: bryan.haggerty
layout: post
guid: http://losingcontext.com/blog/2007/10/the_surface_problem.php
permalink: /blog/2007/10/the_surface_problem/
categories:
  - User Experience
  - Work
---
Sweeping the dirt under the rug, putting a new coat of paint on an old car, opting for a diet coke and calling it healthy living are all solutions to surface problems that never truly solve anything. They&#8217;re the easy and quick things that we think can actually make a difference. Just like in any other space, in software design we see solutions to surface problems passed off as answers to greater issues.

#### Are You Sure&#8230;

My workplace has a culture of excessive email CCing, which I&#8217;m sure exists at many other people&#8217;s companies as well. As a result, many people complain of bloated inboxes with emails which may only indirectly involve them. The probelm is the culture of blindly CCing&#8211;a result of people wanting to cover their bases, an irrelevant email to someone is easier to deal with than a missed email to someone important. And as such, an email propagates, recipients &#8220;Reply to All&#8221;&#8211;resulting in an exponential increase in email that may be irrelevant to a fair amount of people. Often this fact is made apparent by the amount of people who reply to all, pleading to be removed from the email chain. Chain is probably a good word for this too, as users literally feel they become _chained_ to email.

So how does one solve this issue? For the IT staff it was by creating a new dialog box which prompts the user to confirm whether he truly wants to &#8220;Reply to All&#8221;. Sadly, this only attempts to solve the _surface problem_ [people simply replying to all], as opposed to delving into the true root of the problem; that of the email culture of CCing a swath of people without regard for taking into consideration if all people need to be included. Instead, users are now left with an additional step, that solves nothing, in order to reply to an email, even if replying to all consists of only two people.

<img src='http://bryanhaggerty.com/blog/wp-content/uploads/2007/10/reply-to-all-confirm.gif' alt='Confirm to Rely to All' class="image-centered" />

_[note: The email protocol as an effective collaboration tool can be debated as a greater root problem.]_

#### Forgot Your Password, Forget About Calling

The previous example is mostly a minor annoyance and for the most part, people will get on with their activities without much of a hiccup. A more pertinent example, which ultimately had greater consequences, involves the often challenging user authentication process. If a user who should have access can not get access, it is a major problem, one which as time elapses grows even greater. The issue at hand was that a &#8220;Forgot Password&#8221; function was taking an excessively long time to email the user the link to reset their password. As such, users, after waiting hours, assumed something was wrong and that they should call tech support. This resulted in an excessive amount of calls to the tech support call center.

What is interesting is that the call volume was perceived as the problem. First, they needed to figure out how to stop users from calling about forgotten passwords. The solution was a quick fix, a message was put in place next to the tech support telephone number:

> Not for forgotten passwords

It was a very out of sight, out of mind solution. It took care of the _surface problem_, calls reduced, but the true problem still persisted. Users now had little recourse in finding a way to get back on track. Worse still, was that now, the people who should care don&#8217;t even hear the users since they&#8217;ve turned off that avenue of communication. Luckily, many people refused to follow the directions provided and called anyways.

#### Digging Below the Surface

During a user interview, a user may describe what they don&#8217;t like or why they don&#8217;t think it works. And while observing a user in a usability test it can be easy to identify what they get caught up on. The natural instinct is to &#8220;ease the pain where it hurts&#8221;, but often in software or product usability the problem&#8217;s cause could come from an array of different areas.

This isn&#8217;t news, but when design decisions such as the ones I described keep occurring it is good to remind ourselves about spending that extra time to think deeper about what we are solving.