---
layout: post
title: "post rss to Twitter with a custom URL shortener"
date: 2011-9-23 16:40:0
tags: 
---

I've been doing some experimenting and I believe I've figured how to do this with tools already out there (without building your own solution and hosting it). All you need is an RSS feed, a domain you control and a twitter account.



  1. Start with logging in to [bitly.com][1] with your twitter (or create a new account)
  2. Setup your custom domain (this is where you need access to your DNS records)
  3. Get your API login and API password [here][2], you'll need these later.
  4. Log in to [twitterfeed.com][3], I used my Blogger openID.
  5. Create a new feed using the rss URL of your choice. I used my Blogger blog.
  6. In the advanced settings, setup bitly as your shortener and use the API credentials.
  7. Done

Then you write a blog post about how you did it and see if it worked. The one thing I don't like is when you have twitter connected to Facebook, your custom link gets converted to a t.co address. They must do it for safety, but it still sucks. Brand is important.

Update: Only issue I find is that the root of your domain gets taken over by bitly; you have to pay them a little less than 1000$ per month to get the ability to redirect it.

Update 2: Forget everything I said and use [yourls][4]

   [1]: http://bitly.com/
   [2]: http://bit.ly/account/your_api_key
   [3]: http://twitterfeed.com/
   [4]: http://greener.ca/yourls
