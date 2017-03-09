---
layout: post
title: "remote adventures"
date: 2014-02-10
published: true
comments: true

---

## bash

I've been using my iPad to ssh into my home server a lot lately. I have it tethered to an Apple Bluetooth wireless keyboard. I also picked up an [incase Origami Workstation](http://goincase.com/shop/incase-origami-workstation-for-ipad-2), which I love. Here's something I learned: In bash when you type a long command (which takes time if you DON'T have a keyboard) and notice you made a typo in the first word, you can type `C-a` to go to the beginning of the line and `C-e` to go to the end. If you run [screen](http://www.gnu.org/software/screen/), you'd have to do a `C-a C-a` (tmux you're fine since your escape is `C-b` by default). Take a look at the readline section of the bash man page.

## tmux

I discovered [tmux](http://tmux.sourceforge.net/). I'm not sure how I feel about it yet. Seems a lot of the common commands are the same as screen, so that's good.

## RealVNC

OS X screen sharing is good if you have a fast connection. But if you're tethered to a 3G connection and your home broadband only has 400kb/s upstream, it is VERY slow. [RealVNC](http://www.realvnc.com/) has a server for OS X, I'm surprised it took me this long to notice. The free license allows 5 machines. I love the RealVNC app on iOS, now I just VPN to home and use the iOS app. The connection auto-figures-out the speed and adjusts the quality accordingly.
