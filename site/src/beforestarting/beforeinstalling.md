---
layout: page
title: Before Installing Software
permalink: /beforeinstalling
nav_order: 15
has_children: true
---

# STOP - Before Installing Anything

Assuming you are now at a point where you have installed, booted and logged into your chosen Linux distribution I want to quickly stop you here.
On Linux there are multiple ways of installing software:

- OS specific packages (.deb etc)
- Flatpack
- AppImage
- Snap
- Apt repository (or similar RPM)

All of the above provide an executable file or binary that your system uses to run the software you have requested. There is one of these though that I can't recommend and if you happen to have installed an Ubuntu flavour of OS (like Ubuntu or Kubuntu) it is likely that `Snap` has been installed as the default.

# Snap

{: .note-title}
> Personal Opinion
>
> Removing Snap is a personal preference and you should come to your own conclusion.

Snap is a way of delivering software to your system and there is nothing inherently wrong with it. My issue is that Snaps start slightly slower than any other method, they increase disk space usage (the packages you download tend to be larger than the alternatives), they can only be installed from a single source and they go against open source nature (you're running Linux....that's open source).
I personally don't want packages from Snap so I will disable Snap before doing anything but this is an entirely optional step.

## Mint
If you have chosen Mint as your distribution then Snap is disabled by default. You can turn it on but they advise against this.

# Flathub

{: .note-title}
> Personal Opinion
>
> The order in which to install things from is a personal preference and you should come to your own conclusion.


As I mentioned before, Flatpacks are one of the methods of installing software and you may find that some software is only available as a Flatpack. You may also find that software is available from multiple sources so you get to choose how to install it and from where. My personal choice of what order to install things from is:

- Apt
- Flathub
- AppImage

Another thing to consider is what versions are available from which repository. For instance, in Apt the version of Lutris (game management software) is 0.5.14-2 (at the time of writing) where as the version available in Flathub is 0.5.18. This makes a real difference because the version in Apt is 2 years out of date and many fixes or customisations you'll find rely on you using the latest version.
I'll detail how to get Flathub as a repository in your system and show you how to select it as a source.