---
title: Syndication Between WP Sites
date: "2018-03-26"
categories:
  - IndieWeb
  - Syndication
  - Teaching
tags:
  - dyerlab
---
<div class='e-content'>
  <p>
    Syndication is a process whereby you can post something to your site and other locations will detect that you have posted something and then pull in the content to their site, making it look like you wrote it and posted it on their site.  Is that clear?  Here is my use-case:
  </p>
  
  <p>
    <span id="more-459"></span>
  </p>
  
  <ol>
    <li>
      I post everything I do to rodneydyer.com.
    </li>
    <li>
      For things that I want to be shown on my work page (https://dyerlab.org), I select a particular Category or Tag for the post.
    </li>
    <li>
      My work site monitors and any time something at rodneydyer.com comes up with the key Category and/or Tag, dyerlab.org pulls the content of the post in and formats it to look just like I wrote it for that site.
    </li>
  </ol>
  
  <p>
    This is particularly interesting for teaching and other uses.  If a class uses WordPress for its webpage, students can provide content for that class page by publishing on their own site.  This allows each student to create a "Digital Portfolio" of work that they maintain (see my thing on <a href="">Content Silos</a> for more on this).
  </p>
  
  <h2>
    FeedWordPress Plugin
  </h2>
  
  <p>
    I'm going to use the FeedWordPress Plugin for this because it was the one that my university uses and I want to standardize the approaches.
  </p>
  
  <p>
    To install it, go to Plugins->Add New and search for it.  Install & Activate  .I'm going to use a new Category, named <em>Dyerlab</em>, to trigger the syndication.  So I add a new one.
  </p><figure class="wp-block-image aligncenter">
  
  <img src="" alt="" class="wp-image-438" srcset="https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-10.29.53-AM.png 2118w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-10.29.53-AM-300x204.png 300w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-10.29.53-AM-768x521.png 768w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-10.29.53-AM-1024x695.png 1024w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-10.29.53-AM-1070x726.png 1070w" sizes="(max-width: 2118px) 100vw, 2118px" /><figcaption>A new top-level category to handle the syndication.</figcaption></figure> 
  
  <h2>
    Configuration
  </h2>
  
  <p>
    OK, now on my personal page, I have a category "Dyerlab" that I will attach to things that I want to show up on my Dyerlab WordPress site.  To make the connection, we need to get the category feed address.  Unless you are changing something drastic it has the following structure:
  </p>
  
  <pre class="crayon-plain-tag">https://yoursiteurl/category/categoryname</pre>
  
  <p>
    which in my case is:
  </p>
  
  <pre class="crayon-plain-tag">https://rodneydyer.com/category/Dyerlab/</pre>
  
  <p>
    You can try it out and you should see (if you have any posts with that category published) a list of just those posts.  If so, <em>perfect</em>﻿.  If not, then you either have not posted anything with that category or you have not set up the category correctly.  Go back and check.
  </p>
  
  <p>
    Now, I need to set up the other site, in this case my laboratory site, to monitor my personal site, and any time something is posted, grab it.  Go open your other site and make sure the plugin is installed.  This site will "Pull" the posts from the original site.  Click on Syndication in the bottom left panel and you will open the settings page.  
  </p><figure class="wp-block-image">
  
  <img src="" alt="" class="wp-image-451" srcset="https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.09.39-PM.png 1850w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.09.39-PM-300x116.png 300w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.09.39-PM-768x298.png 768w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.09.39-PM-1024x397.png 1024w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.09.39-PM-1070x415.png 1070w" sizes="(max-width: 1850px) 100vw, 1850px" /><figcaption>The syndication settings page.</figcaption></figure> 
  
  <p>
    In the "New Source" box, paste in the category address from your other site.  In my case I pasted in
  </p>
  
  <pre class="crayon-plain-tag">https://rodneydyer.com/category/dyerlab.</pre>
  
  <p>
    You will be taken to a verification screen where you can verify that things are working properly and select the correct feed type.  There is a 'verify' link that you can use to make sure it is providing good input.  After you select which kind of feed you want, you will be redirected back to the list, as above, but with your new feed in it.
  </p><figure class="wp-block-image">
  
  <img src="" alt="" class="wp-image-454" srcset="https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.07.39-PM.png 2156w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.07.39-PM-300x92.png 300w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.07.39-PM-768x235.png 768w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.07.39-PM-1024x313.png 1024w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.07.39-PM-1070x328.png 1070w" sizes="(max-width: 2156px) 100vw, 2156px" /></figure> 
  
  <p>
    Success
  </p>
  
  <p>
    Now, when I write something (like this post) on my site, it will automagically show up on my laboratory site as well. The Cool thing is that wherever it is displayed, it is reformatted to look as if it belonged at that location.  Here is this post on my personal site.
  </p><figure class="wp-block-image aligncenter" style="width:485px">
  
  <img src="" alt="" class="wp-image-466" width="485" height="624" srcset="https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.34.08-PM.png 1054w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.34.08-PM-233x300.png 233w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.34.08-PM-768x990.png 768w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.34.08-PM-795x1024.png 795w" sizes="(max-width: 485px) 100vw, 485px" /></figure> 
  
  <p>
    and on my laboratory site
  </p><figure class="wp-block-image aligncenter" style="width:474px">
  
  <img src="" alt="" class="wp-image-472" width="474" height="452" srcset="https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.52.30-PM.png 1236w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.52.30-PM-300x286.png 300w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.52.30-PM-768x732.png 768w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.52.30-PM-1024x976.png 1024w, https://rodneydyer.com/wp-content/uploads/2018/03/Screen-Shot-2018-03-26-at-12.52.30-PM-1070x1020.png 1070w" sizes="(max-width: 474px) 100vw, 474px" /></figure> 
  
  <p>
    are identical in content, though are individually styles.  Pretty cool!
  </p>
  
  <p style="font-size:12px">
    Featured image bytes <a href="https://www.flickr.com/photos/amattox/">amattox mattox</a> (CC BY-NC 2.0).
  </p>
</div>
