---
layout: post
title: Using a Logitech K750 PC Version on a Mac
date: 2015-09-02 14:58:39.000000000 +08:00
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories: []

---
Probably one of the nicest full-sized wireless chiclet keyboards for PC (which used to come in a Mac version, however Logitech stopped selling them)

So I'm forced to use the PC version on a Mac, which comes with a few gotcha's. For one, the PC version has a hardware-based FN key (the OS doesn't know you've pressed it until you press the corresponding blue-text key as well)

Oh and the Vol Up/Down/Mute keys are one position left on the keyboard than the Mac equivalent.

Mac: F10 = Mute, F11 = Down, F12 = Up.  
PC: F9 = Mute, F10 = Down, F11 = Up.

![apple_web]({{ site.baseurl }}/assets/images/apple_web.jpg) [![k750_web]({{ site.baseurl }}/assets/images/k750_web.jpg?w=300)](https://xrwtech.files.wordpress.com/2015/09/k750_web.jpg)

Ugh....  
Enter [Karabiner](https://pqrs.org/osx/karabiner/)

![Screenshot 2015-09-02 14.30.27]({{ site.baseurl }}/assets/images/screenshot-2015-09-02-14-30-27.png)

With it, you can remap your keys and make customisations more relevant to the Mac world.

I find the Home/End re-mapping great.

![Screenshot 2015-09-02 14.44.53]({{ site.baseurl }}/assets/images/screenshot-2015-09-02-14-44-53.png)

There are some exceptions where this shouldn't be remapped of course, and that's Remote Desktop sessions (which I use [RoyalTSX](http://blog.xrw.tech/2015/08/20/using-royal-tsx-to-administer-your-windows-network-from-your-mac/) for - see my previous blog post)  
So we had to add an exception into the XML file - easy!

![Screenshot 2015-09-02 14.46.58]({{ site.baseurl }}/assets/images/screenshot-2015-09-02-14-46-58.png)

In the following example I've remapped the following;

F3 = Spotlight  
F4 = Launch Calculator.app (always found that handy in Windows)  
F9/10/11 = Mute, Vol Down, Vol Up  
PrtScr = OSX Screenshot to Clipboard  
FN+PrtScr = OSX Screenshot to File

Put this code in your private.xml file;  

<script src="https://gist.github.com/IX9/660c276addcaf983207a.js"></script>

Hit the Reload XML button and enable the "K750" options to suit you.

![Screenshot 2015-09-02 14.48.40]({{ site.baseurl }}/assets/images/screenshot-2015-09-02-14-48-40.png)

