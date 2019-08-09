---
layout: post
title: AFP setup on CentOS 7
date: 2015-08-10 13:09:35.000000000 +08:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- sysadmin

---
Finding an accurate how-to for the minefield that is, open source software is sometimes terrible.

Documentation is hard to read, and often isn’t updated for point releases, which is often out of date.

&nbsp;

Thank god this blog post from Zit Seng explains exactly how to setup Netatalk on CentOS 7.

[https://zitseng.com/archives/6182](https://zitseng.com/archives/6182)

&nbsp;

Except for the afp.conf file, which sometimes needs a little more massaging to be usable as a bare minimum config.

&nbsp;

I found it needs the **uam list** property present in the file in order for AFP clients to connect successfully.

I’m using OSX 10.10.5 (Yosemite) and found without these config directives accessing the shares would fail.

&nbsp;

Here’s a working usable config you can use;

<script src="https://gist.github.com/IX9/45df69dec5d471b983d5.js"></script>



&nbsp;

