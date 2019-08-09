---
layout: post
title: Automating Maxmind GeoIP downloads on Windows
date: 2015-08-20 18:05:51.000000000 +08:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- sysadmin

---
Sure - there’s lots of snippets for automating the GeoIP database downloads (with your Maxmind subscription) for your \*nix boxes, but not many for Windows.

&nbsp;

Here’s a simple PowerShell script that you can pop into your favourite job scheduler application (Batch Job Server, JAMS Scheduler, or \*ugh\* Windows Task Scheduler)

&nbsp;

It’s pretty rough and not much error handling (I wrote it quickly) but it does the job to;

&nbsp;

1. Download the latest GeoIP file

2. Unextract the double-zipped tar.gz file

3. Copy the unextracted .dat file to a location for you to use

&nbsp;

(We use this in a webfarm environment, which is replicated to each web server via Microsoft’s DFSR)

&nbsp;

It’s posted here on GitHub, so feel free to make improvements and collaborate :)


<script src="https://gist.github.com/IX9/cd1fa5bde12de3f917dc.js"></script>
