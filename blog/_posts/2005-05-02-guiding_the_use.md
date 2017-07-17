---
id: 48
title: Guiding the User with Contextual Help
date: 2005-05-02T13:49:01+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2005/05/guiding_the_user_with_contextual_help.php
permalink: /2005/05/guiding_the_use/
categories:
  - User Experience
---
As a [PayPal](http://www.paypal.com) user I frequently use it to pay for products or services when available, as it is easier than pulling out the credit card. Recently, while renewing a domain name at [GoDaddy](http://www.godaddy.com) using _PayPal_ I ran into an unfamiliar form request. Unfortunately _GoDaddy_ does not provide easily accessible explanations to such requests. Situations such as these are ideal for contextual help.

The form request in question is displayed below in Figure 1.

<p class="figure-centered">
  <img src="/blog/images/godaddy-original.gif" alt="An ambiguous form request" height="63" width="538" /><br /> Figure 1. <em>Ambiguous form request at GoDaddy</em>
</p>

My first inclination about this form request was that the system needed a name which they would use to identify my _PayPal_ account&#8211;and it wanted it to be friendly! Unsure of what exactly this meant, I simply re-entered my name.

Upon further research, the form request is asking the user to give the _PayPal_ account a name which the user can use later to identify it (e.g., My Personal PayPal account). Such form requests are of a different nature than the typical Name, Phone, and Email Address which users are already familiar with, they are used frequently, and are self-explanatory. Additionally, the typical mode of interaction for the user is to provide the system with the necessary information for it to process the transaction. But in this case the system is asking the user to provide information for the user to use. Thus, such a request can appear somewhat ambiguous to the user. Contextual help could have easily provided me with the basic information about what the request was truly seeking.

Contextual help the is simplest and quickest way to assist users when they are unsure about something. Using contextual help provides the user with specific and concise information about the request in question. Displayed below in Figures 2 and 3 are two simple contextual help implementations for the _GoDaddy_ order form.

<p class="figure-centered">
  <img src="/blog/images/godaddy-example.gif" alt="Form request with example contextual help" height="63" width="538" /><br /> Figure 2. <em>Example contextual help</em>
</p>

In Figure 2 the user is guided by the presentation of example responses. This method utilizes a limited amount of screen real estate and conveys the intended meaning of the request concisely. The downside of this method is that it cannot provide a more in depth description, which depending on the ambiguity of the request, some users may require.

<p class="figure-centered">
  <img src="/blog/images/godaddy-what.gif" alt="Form request with 'What's This' contextual help link" height="63" width="538" /><br /> Figure 3. <em>Contextual help through &#8220;What&#8217;s This&#8221; link</em>
</p>

Figure 3 provides a method which handles the shortcoming of the example method by offering a &#8220;What&#8217;s This&#8221; link, which provides a supplementary page containing additional information unconstrained by screen real estate. Typically upon pressing the link the user is presented with a new window featuring a deeper explanation of the request. One of the drawbacks of this method is that the user is required to manage multiple windows, which can hinder the intended goal by increasing the cognitive load.

Both methods are significant improvements over providing nothing at all, especially for an e-commerce site like _GoDaddy_ who seeks to get your business. As a designer you need to determine what contextual help methods are most ideal for each particular situation&#8211;what will make the user feel comfortable and allow them to achieve their goal quickly.