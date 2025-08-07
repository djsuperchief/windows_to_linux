---
layout: page
title: Getting Started
permalink: /gettingstarted
nav_order: 10
---

# Getting Started
{: .no_toc }
- TOC
{:toc}

## Choosing Your Linux Distribution
The first step in your journey is choosing your Linux distribution and there are A LOT to choose from.
I can only speak from personal experience but Debian, Mint and Ubuntu are the core ones that I have used. Mint is very user friendly and is an ideal place to start if you're considering a move to Linux. You could also potentially use something like `Bazzite` but it is also worth noting that this is a fairly new distribution and may have specific quirks (one of them being it is an immutable OS meaning you are limited in what you can change).
I can only advise that you do your research before ultimately choosing a distribution to try. You also don't have to stick to the original one you choose, you can decide that to try another. You can even change the desktop environment you end up with (there are a few KDE, Gnome etc) so your choices are endless on what to choose.

I personally chose Kubuntu for a very specific reason; dual booting to a separate drive in Mint was not simple.

### Why I Chose Kubuntu
I initially chose Mint as I had used it before, it didn't use Snap (more on that later) and I thought it would be a great option for me to try. The thing that ultimately stopped me was when I tried to do a dual boot installation as setting it up on a separate drive was not simple and I had to specify the space required for different partitions. Now this is something I really should get to know and understand but at this point I am just trialing Linux and I want the process to be as simple as possible. This made me choose a different distribution, one that would give me a much easier and more simple path to actually testing Linux.

A friend who has been using Kubuntu for a long enough time told me about it, about how you could disable Snap and showed me the dual boot process. This was enough for me to move it to the top of my list. I didn't want the Gnome desktop environment and preferred Cinnamon (Mint's desktop environment) or KDE and Kubuntu is Ubuntu but with KDE (hence Kubuntu).
A personal recommendation is good enough for me because it is someone with experience using the system "in anger".

## Dual Booting
So if you are just looking to try Linux as an alternative I would advise doing a dual boot. What this means is that you keep your existing Windows installation and also have Linux available. When you turn on your computer you will be presented with a menu that allows you to choose what you boot into and you can go into your chosen Linux install OR go into Windows (as well as a few other options but that's outside the scope of this).

In Kubuntu's case I was able to select the drive I wanted for the OS to live on and the rest was done for me.

### Separate Drive
Dual booting on an existing drive (the one Windows is currently installed on) is generally not advised. Windows can essentially erase the changes Linux makes to your boot loader and you could loose the ability to boot into Linux. Not only that, installing Linux on a separate drive isolates the two systems away from each other so you can test safe in the knowledge that you are not damaging either system. If you have a spare drive, great use that. If not, I can advise getting a 2TB SSD to give you enough space to install the OS and test. If you aren't confident in adding a new drive to your system ask your friendly neighborhood IT person (you all have that friend...you know you do).

#### Physically Remove Windows Disk?
I didn't remove my Windows drive when doing the dual boot installation but lots of guides advise you to do so. This is so that you don't accidentally erase your Windows install and it's sound advice. I, however, didn't as I knew which drive was being used. Whether you remove the Windows drive from your machine is up to you. I don't know if Grub (the Linux boot loader) will pick up your Windows installation afterwards if you add the drive back in, do your research.

## Hardware Support
Get a list of your hardware and go to the manufacturers website. They may provide Linux apps or drivers and it is worth confirming whether Linux will work for your hardware. For me, mine "just worked" out of the box with a few apps required to get some of the finer parts of my system working but you may have varying luck with yours. Chances are good that things will just work but do your research! I cannot stress that enough. Hardware will most likely be at the top of the reasons as to why you won't move to Linux (along with Anti-Cheat but that's later) and it is probably one to get out of the way early.

## Don't Be Afraid Of The Terminal
At some point you will need to go into the terminal to do something whether it is to install something, do an update or edit something on the system. If you are going through a tutorial or instructions make sure you follow them to the letter and read everything before writing or executing anything. Read peoples responses to what commands you have been instructed to run and try to understand as best you can what they are asking you to do.
Given what I just said sounds scary, going into the terminal is a normal thing in a Linux world and nothing to be scared of. A lot of what you will need to do won't involve the terminal but on the odd occasion, you will need to venture into it but do so with confidence. After all, you are trialing this setup and you can't mess up your Windows installation. If something goes wrong it is just a learning experience and you can always try again.

## The First Solution Isn't Always The Right One
You may come across something that works for you but not quite. For instance, I used OpenRGB to control the RGB on my system but all I was really bothered about was my K70 keyboard not being a flashy mess all the time. I used OpenRGB for a few days and then found something that worked a lot better and was more geared to Corsair hardware specifically. I stopped using OpenRGB and went with what I had found because it was a better solution so the key message here is sometimes the first thing you find is not always the last thing you'll use. Keep looking for better alternatives and don't be afraid to try open source things.

## Note On My TLDR Edition
I will summarize the steps I took to do something in a "TLDR" on the page. I do advise that where I have provided a link to an article or resource, go to it first and read it thoroughly. If it is a forum post, read the responses. If it is a github / source repository, read the issues associated with it before executing anything.
Most things on Linux you do so at your own risk and what works for one person might not work for you.

## Personal Opinion
Throughout this site I will label things up with "Personal Opinion". What I mean by this is it is entirely optional and whether you follow what I do is up to you. Everything is down to personal taste and for things like removing Snap, that's up to you. I don't want it on my system so i've removed it but you might not be bothered.

---
I'll add things to this as they come along but this is as good a place to get started.