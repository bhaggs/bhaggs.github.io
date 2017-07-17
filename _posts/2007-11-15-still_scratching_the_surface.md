---
id: 117
title: Still Scratching the Surface
date: 2007-11-15T14:22:34+00:00
author: bryan.haggerty
layout: post
guid: http://losingcontext.com/blog/2007/11/still_scratching_the_surface.php
permalink: /2007/11/still_scratching_the_surface/
categories:
  - User Experience
  - Work
---
Earlier I had discussed the topic of only [solving the surface problem](http://bryanhaggerty.com/blog/2007/10/the_surface_problem.php) instead of digging deeper into the real problem. The &#8220;Reply to All&#8221; solution has now been accompanied with other surface solutions to &#8216;solve&#8217; more email problems.

As an organization that deals with sensitive information, the leaking of such information even if accidental is a major concern. And one of the possible ways this information can be leaked is via email to external addresses. In an effort to thwart this issue, a design change has been made to the email software (shown below), which requires users to specify whether their email is being sent to internal recipients or internal and external recipients. If the user fails to select that his email is being sent to external recipients, he will not receive any indication that the email was not delivered.

<img src='http://bryanhaggerty.com/blog/wp-content/uploads/2007/11/email-internal-external-recipients.gif' alt='Email settings for Internal or External recipients' class="image-centered" />

I cannot ascertain whether additional screening measures are performed on emails which are defined as being for external recipients, but based on communications about the changes, it appears they exist as a means of reinforcing how to properly handle sensitive information (i.e., it most likely shouldn&#8217;t be sent to external people). Certainly an odd way of communicating of this though, as users can simply always just select _internal / external e-mail_ just to feel safe that their email will be sent. This is especially due to that by default users will be given the impression their email is being sent when in fact it essentially may have never made it past their outbox.

As an aside, the changes are having an interesting side-effect: as emailing becomes more of a pain to do, alternatives such as IM are becoming a seemingly easier option.