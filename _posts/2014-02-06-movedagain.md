---
layout: post
title: "well that was fast"
date: 2014-02-06 12:00:00
published: true
comments: true

---

[calepin](http://calepin.co/) is nice, but it seems it's not really supported anymore.

So I ventured to run [pelican][1] myself on [sdf](http://sdf.org/). Alas the VHOST and DNS memberships don't offer much in the flexibility department. Reading on the webs looks like most people (markdown bloggers) gravitate towards [jekyll](jekyllrb.com) and even [octopress](octopress.org). So here I am. I had to convert my posts from [scriptog.am](http://scriptogr.am) / [calepin](http://calepin.co/) / [pelican][1] format to something with a YAML front matter.

This worked:

{% highlight bash %}
#!/bin/bash
# Mac OS X .. ymmv
for i in $1/*.md; do
    sed -i '' -e 's/Tags:/tags:/' \
    -e 's/Title:/title:/' \
    -e 's/Date:/date:/' \
    -e '/title:/i\'$'\n''---' \
    -e '/title:/i\'$'\n''layout: post' \
    -e '/tags:/a\'$'\n''---' "$i"
done
{% endhighlight %}

[1]: http://pelican.readthedocs.org/
