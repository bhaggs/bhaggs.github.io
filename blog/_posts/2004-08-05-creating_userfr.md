---
id: 21
title: Creating User-Friendly URLs
date: 2004-08-05T10:59:12+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2004/08/creating_user-friendly_urls.php
permalink: /2004/08/creating_userfr/
categories:
  - User Experience
---
The web is rampant with crude looking URLs largely due to the increase of dynamically generated web pages. Not only do these URLs look poor visually they decrease a site&#8217;s usability and become less attractive to search engines for ranking.

I&#8217;ll take a look at why these URLs are a problem and how they can be fixed to present a friendlier user experience and improve your search rankings.

### Usability of URLs

Ever try to tell someone a URL over the phone or attempt to write down a specific URL? Aside from the domain name, things can get real hairy after that first trailing slash. Somewhere along the line, we as developers have seemed to forget what the URL is supposed to tell the user.

In basic terms, the URL is an address and we can learn a lot from comparing a URL to a street address. The street address has a structure which for the most part has been standardized and shows meaning in it&#8217;s presentation. I can read it off to a person over the phone and they too will understand it. I can also easily remember a street address as well.

I&#8217;m not saying that we need to standardized our URL structure across the board but to remember that there is meaning in structure. The URL presents a hierarchy which informs users about the information which they are viewing.

In working on [TheDatingFile.com](http://www.thedatingfile.com "Visit TheDatingFile.com") we had to deal with this very problem in particular. For example we used to have the URL shown below:

`http://www.thedatingfile.com/info.php?id=4&file=straight`

What does that mean? Not much to the user. Forget about attempting to type that in yourself from memory. Actually forget about even looking at it. Once the question marks and ampersands begin to appear it looks less like information and more like code.

After implementing web server features, which I&#8217;ll discuss later, here is the result:

`http://www.thedatingfile.com/straight/yahoo/`

This URL now actually provides the user with some information. The hierarchy is used to present the user with not only a simple overview of the content of the page but also their location in the web site.

**Further Reading:**

  * Jakob Nielsen&#8217;s Alertbox [URL as UI](http://www.useit.com/alertbox/990321.html)
  * Adam Baker&#8217;s Theory: [How to make URLs user-friendly](http://www.merges.net/theory/20010305.html)
  * IBM DevelopWorks: [Making URLs accessible](http://www-106.ibm.com/developerworks/web/library/us-cranky8.html?dwzone=web)

### Search Engines and Friendly URLs

Google says it best in their [Information For Webmasters](http://www.google.com/webmasters/2.html):

<blockquote cite="http://www.google.com/webmasters/2.html">
  <p>
    We are able to index dynamically generated pages. However, because our web crawler can easily overwhelm and crash sites serving dynamic content, we limit the amount of dynamic pages we index.
  </p>
</blockquote>

Many search bots see dynamic pages as endless loops of links or blind alleys. Which many times is not the case. From a developer&#8217;s stand point, making dynamic pages can save tons of time but unfortunately search engines impose a penalty for that. Luckily there is a solution, Apache&#8217;s [mod_rewrite](http://httpd.apache.org/docs/mod/mod_rewrite.html "Learn more about mod_rewrite from Apache").

### Make Your URLs Friendly

Mod_rewrite has a lot of features ranging from easy to implement to the more complex. Shown below is how we made our URLs for [TheDatingFile.com](http://www.thedatingfile.com "Visit TheDatingFile.com") more user-friendly and optimized for search engines.

The following code is contained In our `.htaccess` file stored at the root level of the site:

`RewriteEngine On<br />
RewriteRule ^(.*)/(.*)/$ /info.php?file=$1&shortname=$2 [L]`

A brief explanation of what is actually going on here. We start off by telling the Apache web server to turn on mod_rewrite. The `RewriteRule` is what will do all the work in transforming our URLs. &#8220;`^(.*)/(.*)/$`&#8221; is the format in which we wish to have our URLs displayed. &#8220;`(.*)`&#8221; will match anything and put the contents, starting with `$1`, into the variable (`file=$1`) of our real dynamically generated page.

**Further Reading:**

  * DevShed: [Make Dynamic URLs Search Engine Friendly](http://www.devarticles.com/c/a/Web-Services/Make-Dynamic-URLs-Search-Engine-Friendly/) 
  * Webmaster Toolkit: [mod_rewrite RewriteRule Generator](http://www.webmaster-toolkit.com/mod_rewrite-rewriterule-generator.shtml)