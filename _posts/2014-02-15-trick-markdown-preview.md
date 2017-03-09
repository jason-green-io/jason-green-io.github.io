---
layout: post
title: "Trick markdown preview"
published: true
date: 2014-02-15 13:29
comments: true

---

You can trick your markdown preview into correctly rendering the front matter from octopress (depending on the flavor of markdown your app uses). This works with 1Writer, not so much in Byword.

Just leave a space before the last `---`. Like so.

    ---
    layout: post
    title: "Title"
    published: true
    date: 2014-01-01
    comments: true
    
    ---

And voila!
