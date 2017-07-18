---
id: 35
title: 'An Example of Inconsistent &amp; Poor Form Design'
date: 2005-01-05T20:32:30+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2005/01/an_example_of_inconsistent_poor_form_design.php
permalink: /2005/01/effects_of_inco/
categories:
  - User Experience
---
Web applications are becoming more and more prominent, as are the html forms which comprise the method of interaction for these applications. Through the use of a simple example, I&#8217;ll discuss some of the good and bad points behind this example&#8217;s form design in terms of instructions and form actions. Additionally I&#8217;ll cover some tips on how to identify and avoid these problems.

I recently came across a simple example of inconsistent form design at the [SallieMae](http://www.salliemae.com/ "See the example for yourself") website. Due to that I rarely login to this particular website I needed to find out what my _user ID_ and _password_ were. To attain this information it is necessary to access both their _Forgot user ID_ and _Forgot password_ forms. Two very simple forms, let&#8217;s take a closer look into the components of the forms.

### What They Got Right

The forgot user ID tool, shown below in Figure 1, is extremely straight forward. Clear instructions are provided to the user conveying what is needed from them and what will occur upon completing the form. The form&#8217;s action buttons located to the lower right give the user not only the ability to commit the request for retreiving his user ID by pressing _Submit_ but also an exit strategy with the _Cancel_ button.

<p class="figure-centered">
  <img src="/blog/wp-content/uploads/legacy/salliemae-figure1.gif" alt="SallieMae Figure 1" height="237" width="450" /><br /> Figure 1
</p>

### What They Got Wrong

The forgot password form, shown below in Figure 2, unfortunately fails to follow the precedent set by the forgot user ID form. One of the main problems with the form is that it does not provide the user with instructions or information about what will occur upon submitting the form. Will the password be emailed? Will the user be asked to enter a new password?

The user is then presented with two possible form actions, both of which do not correspond to those presented in the forgot user ID form, _Clear_ and _Next_. Upon pressing the clear button the contents of the form&#8217;s text field will be erased. This would be considered an extremely weak exit strategy as the user is still positioned at the form. Typically clear buttons are frowned upon as it is not likely that a user will fill out an entire form only seeking to erase it all, at least in this form there is only one field. In the case of using a clear button, even a cancel button for that matter, the user should be prompted to confirm the action. Additionally, on a broader note, the page offers no link back to the home page, not even the _SallieMae_ logo, which could have been seen as an exit.

The use of Next as a form action is usually reserved for forms which have multiple form pages. While that may be the case for this form the user has no knowledge of that. If multiple form pages are going to be used, the user should be provided with such information. This can be in the form of stating that the form process has, for example, three steps.

<p class="figure-centered">
  <img src="/blog/wp-content/uploads/legacy/salliemae-figure2.gif" alt="SallieMae Figure 2" height="209" width="450" /><br /> Figure 2
</p>

### What This Can Lead To

The user not knowing what is required of them can lead to frustration and form drop outs. As for this example, a user could possibly end up calling SallieMae&#8217;s phone support, which ultimately can lead to increased costs.

### Lessons Learned

The best way to minimize these types of problems is sticking to the conventions which are used by countless developers. At the least, stick to your own conventions. That was the problem with SallieMae, they got some things right but failed to implement those methods across their other forms.

Another thing to consider is that whether you use _submit_, _enter_, or _send_ be consistent throughout your forms. As users become more familiar with your site they will become more comfortable if there is a coherent voice. You don&#8217;t want users second guessing the meaning of your form buttons.

Most importantly, provide users with clear and proper instructions. As the developer, a form&#8217;s use seems idiotically clear but that is a horrible assumption to make. If possible test the form with users, even if they are just co-workers or friends.