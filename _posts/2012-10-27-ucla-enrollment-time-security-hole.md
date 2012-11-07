---
layout: post
title: "UCLA Enrollment Time Security Hole"
description: ""
category:
tags: [UCLA]
---

It’s the end of week 4, fall 2012 at UCLA. According to the registrar [calendar](http://registrar.ucla.edu/calendar/calf12.htm), the schedule of classes for Winter 2013 will be posted on October 29 and our enrollment appointment times will be available on URSA on October 31.

If you logon to URSA to view your enrollment appointment times, you’ll see that 2012 is the highest year available:

![URSA enrollment time menu](/images/URSA.png)

So I hit Apple + Option + I to view the Inspect Element pane in Chrome, and changed the dropdown entry’s value from 2012 to 2013 and submit the form.

![URSA inspect element](/images/inspect.png)

UCLA didn’t implement a check to make sure that form values I submitted matched against their enrollment appointment announcement times, so I was able to get my enrollment times:

![URSA times](/images/times.png)

Try it if you’re as impatient as I am.

{% include JB/setup %}
