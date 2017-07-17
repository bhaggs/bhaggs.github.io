---
id: 37
title: A Look at Google Maps
date: 2005-02-27T16:03:36+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2005/02/a_look_at_google_maps.php
permalink: /2005/02/google_maps/
categories:
  - Technology
---
Google&#8217;s recently released Maps beta is likely to be considered more innovative than their GMail product. Especially when looking at the markets for each product. While GMail provided an unheard of, at the time, 1gb of storage, the competition quickly responded. This isn&#8217;t to say that GMail didn&#8217;t have an assortment of other great features, but with [Google Maps](http://maps.google.com) they have completely changed the online map paradigm.

<p class="figure-centered">
  <img src="http://www.losingcontext.com/blog/wp-content/uploads/legacy/gmaps-overview.jpg" alt="Google Maps Overview" height="210" width="450" /><br /> Figure 1. The new Google Maps.
</p>

One of the major drawbacks of map services such as [MSN Maps](http://maps.msn.com) and [Mapblast](http://www.mapblast.com) is merely due to the nature of how the web works, a lack of continuous communication between client and server. Using typical online maps is like using a real map that you are not allowed to completely unfold, requiring requests to the server to unfold another piece of the map. Through technologies such as _Ajax_ (XMLHttpRequest) Google Maps are draggable and easy to work with, without the need for page reloads. You could scroll from the East Coast to the West Coast if you so desired. When page reloads occur it is not uncommon for users to lose their location focus, requiring users to have to waste cognitive resources to reorient themselves.

#### Some Hidden Features

A feature that will probably go unnoticed by many is the dynamic resizing of the map area. Upon resizing the browser window the map view changes accordingly to fit the space. This is a great feature if you are a person with a high display resolution, as you will be presented with a large map automatically. This eliminates the need for _Map Size_ buttons.

Just like in GMail, Google has added keyboard shortcuts for Google Maps. This is especially nice for scrolling around a map, by way of the keyboard&#8217;s arrow keys.

<p class="figure-right">
  <img src="http://www.losingcontext.com/blog/wp-content/uploads/legacy/gmaps-local-search.jpg" alt="Google Maps Local Search Bubble" height="237" width="212" /><br /> Figure 2. Local Search Bubble.
</p>

Location bubbles provide the user with a direct one to one connection between possible actions and the object which they will be applied to. This is currently only used for directions but could easily include _Local Search_ features. For example as shown in Figure 2, _Find great sushi near this location_

#### Areas of Improvement

There are still a few quirks in need of fixing though. The fact that a user is forced to click a link to get a URL for the map is a bit of a hassle. Especially since most users are accustomed to being able to just copy the URL from the browser&#8217;s location bar. Additionally, it is always a bad idea to ask users for information which the system already knows. When a user has searched for a particular address and is now looking for directions to it, the application should employ some basic assumptions. The user is likely to be traveling from a fairly local location, (i.e., do not force the user to have to enter the city and state again for the origin location). This is not a problem exclusive to Google Maps, but an annoyance I have with all the map services.

Google is definitely hard at work on this product. In a short period of time I&#8217;ve noticed a fair amount of tweaks such as the altering of the _Example Searches_ and better support for Apple&#8217;s [Safari](http://www.apple.com/safari/) browser. What will be more interesting is how the competition responds to Google Maps, since it seems there is already a lot to catch up to.

<p id="related-links">
  <strong>Related Links</strong>
</p>

  * [Augmenting Google Maps with Landmarks](/blog/2005/03/augmenting_goog.php)

<p id="update">
  <strong>Update:</strong> It seems there is some discrepancy as to whether Google Maps uses Ajax or a method which uses a hidden iframe. According to other sources the hidden iframe method appears to be the most likely answer. This method seems to be similar to a technique which we used at Harvard called <em>JSRS</em> from <a href="http://www.ashleyit.com/rs/" title="Learn more about JSRS">Ashley IT</a>.
</p>