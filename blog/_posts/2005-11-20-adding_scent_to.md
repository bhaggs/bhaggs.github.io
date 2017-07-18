---
id: 57
title: Adding Scent to Pagination
date: 2005-11-20T13:00:38+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2005/11/adding_scent_to_pagination.php
permalink: /blog/2005/11/adding_scent_to/
categories:
  - User Experience
---
Spanning search results or any other kind of list of information across pages has become standard fare on the Web. Unfortunately this information is now secretly locked behind mystery doors (links) 2 through 34. How can we give the user insight into what lies behind these doors instead of simply choosing at random in order to find they information they desire?

Pagination has helped in reducing the load of information a user has to take in or download for that matter, but the pagination navigation leaves a great deal to be desired. Typically the pagination navigation is simply a list of linked numbers which reference each page of results, sometimes truncated to reduce an overload of page links. The problem with this is that the user is essentially gambling with what he will be presented with when clicking on a page link. Which is why most users don&#8217;t actually randomly pick a page, they walk through the results with the _Next Page_ link.

[Jared Spool](http://www.uie.com/) has talked at great lengths about the idea of [information scent](http://www.uie.com/reports/scent_of_information/), basically giving the user an idea of what lies behind a link before they click it. Information scent can give a user a purpose to click a link. Pagination navigation does not provide the user with any scent as to what exists behind a link such as _4_. When looking at an alphabetically sorted list of results, wouldn&#8217;t it be nice to be able to know that a particular letter was on a certain page instead of excessively clicking around? Figure 1 showcases a pagination navigation scheme with scent for [Flickr](http://www.flickr.com). When the user mouses over a page link he is presented with a sample of the photos which exist on that page. Thus allowing the user to make a better informed decision about whether to proceed to that page or not.

<p class="figure-centered">
  <img src="/blog/wp-content/uploads/legacy/pagination-scent-flickr.jpg" alt="Flickr pagination with information scent" height="288" width="463" /><br /> Figure 1. <em>Flickr pagination with information scent</em>
</p>