---
id: 20
title: Dating File Relaunch
date: 2004-07-30T16:46:58+00:00
author: bryan.haggerty
layout: post
guid: http://beta.losingcontext.com/blog/2004/07/dating_file_relaunch.php
permalink: /2004/07/dating_file_rel/
categories:
  - Work
---
[<img src="/blog/images/new-tdf.jpg" alt="The Dating File Revamped" class="image-right" border="0" height="177" width="200" />](http://www.thedatingfile.com "Visit The Dating File.com") [FourSedgewick Interactive](http://www.foursedgewick.com "Visit the FourSedgewick Interactive web site") has been hard at work revamping [The Dating File](http://www.thedatingfile.com "Visit The Dating File.com") and bringing it back to life. After a long hiatus we&#8217;re ready to bring the site back with a souped up engine.

The release brings along a new standards compliant design featuring XHTML 1.0 Transitional and CSS 2. As well as prominent use of <acronym title="Portable Network Graphics">PNGs</acronym> and alpha-transparencies. In order to discuss the benefits of standards compliant design I&#8217;ve provided a bit of analysis between the version 4 site and the newly released version 5.

#### The Challenges

Being an aggregator site visitors will only spend a short period of time at the site, they may even leave before it finishes loading. That was why we needed to trim down the download time but still keep the same look and feel.

_The Dating File_ previously sported a table based layout for presentation. Which required a lot of slicing of images to get the desired look, which left us with severe image bloat. Not to mention wasted bits on non-structure tags used for presentation.

The previous version featured unique _rank_, _star on_, _star off_, and _join_ images. In order to get our color fade this was the only way possible since transparent gifs would suffer from rough edges.

#### The Solution

The use of valid valid XHTML markup and CSS helped reduce the tag overload induced by using a totally table based layout. Separating presentation markup from structural markup also aided heavily in terms of <acronym title="Search Engine Optimization">SEO</acronym>. By presenting search engine spiders only with structurally marked upped content the site gets a better rating in terms of semantics. For instance our logo is actually an `h1` tag which has a higher ranking than say an `img` tag.

In response to the excessive image use we capitalized on the features of the PNG format and its alpha-transparencies. The use of PNGs allowed us to trim 20 unique images down to just 4. Unfortunately our user base is primarily Win/IE users and alpha transparency images and Win/IE do not play well together. Fortunately Justin Koivisto&#8217;s [IE PNG Hack](http://www.koivi.com/ie-png-transparency/ "Learn more about the IE PNG hack") provided a nice workaround which did not affect other browsers which do display PNGs correctly.

#### The Results

Below is a comparison between the previous version and the current version in terms of download metrics.

<table border="0" cellspacing="0">
  <th>
  </th>
  
  <th>
    Version 4
  </th>
  
  <th>
    Version 5
  </th>
  
  <tr>
    <td>
      Size of webpage
    </td>
    
    <td>
      19.3K
    </td>
    
    <td>
      9.1K
    </td>
  </tr>
  
  <tr>
    <td>
      Visible text size
    </td>
    
    <td>
      2.1K
    </td>
    
    <td>
      1.2K
    </td>
  </tr>
  
  <tr>
    <td>
      Size of html tags
    </td>
    
    <td>
      17.2K
    </td>
    
    <td>
      7.8K
    </td>
  </tr>
  
  <tr>
    <td>
      Number of images
    </td>
    
    <td>
      58
    </td>
    
    <td>
      33
    </td>
  </tr>
  
  <tr>
    <td>
      Unique images
    </td>
    
    <td>
      45
    </td>
    
    <td>
      10
    </td>
  </tr>
  
  <tr>
    <td>
      Size of all images
    </td>
    
    <td>
      27K
    </td>
    
    <td>
      12K
    </td>
  </tr>
  
  <tr>
    <td>
      Grand total
    </td>
    
    <td>
      46.4K
    </td>
    
    <td>
      21.2K
    </td>
  </tr>
</table>

As can be seen from the grand total we&#8217;ve optimized the site by about **46%**! We&#8217;ve cut the download size almost in half, without compromising the visual display.

<p id="related-links">
  <strong>Related Links</strong>
</p>

  * [The Dating File portfolio entry](http://www.losingcontext.com/portfolio/thedatingfile/)
  * [Creating User-Friendly URLs](http://www.losingcontext.com/blog/2004/08/creating_userfr.php)
  * [Taking On CSS](http://www.losingcontext.com/blog/2004/08/taking_on_css.php)