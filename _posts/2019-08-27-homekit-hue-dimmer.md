---
layout: post
title: Homekit and Hue dimmer with LivingWhites Plug
date: 2019-08-27 13:09:35.000000000 +08:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- homeautomation

---

As of firmware 1933144020 for the Philips Hue Bridge, it no longer allows dimming functionality on the LivingWhites dimmable plug.

Fortunately this can be negated in OpenHAB (assuming correct bindings in the items xml) with the following Node-RED flows.
[![homekit-nodered.png]({{ site.baseurl }}/assets/images/homekit-nodered.png)]

<script src="https://gist.github.com/IX9/14c92405d46aba096c5cd3bc39296e98.js"></script>