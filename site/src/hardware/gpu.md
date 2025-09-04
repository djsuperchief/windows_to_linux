---
layout: page
title: GPU
parent: Hardware
---

# GPU - NVIDIA

{: .warning}
These are the steps I took, please do your own research before deciding to follow the article posted or this page.

## Drivers
So this one is an interesting one. NVIDIA do provide their own drivers and there is a download link for Linux specifically but I read varying reports on the success of those drivers. Following [this](https://documentation.ubuntu.com/server/how-to/graphics/install-nvidia-drivers/#the-recommended-way-ubuntu-drivers-tool) documentation, I was able to get the NVIDIA drivers installed with very little issue. What this does is essentially let the OS decide what is best for the system and I think in this case, i'll let it.

## Instructions - TLDR Edition
Open up a terminal and run the following:

```
sudo ubuntu-drivers list
```

You'll get a list of drivers and in there should be nvidia-driver and a number. Now run the following:

```
sudo ubuntu-drivers install
```

And this will install all the drivers your OS thinks it needs.

And that's it. You shouldn't need to do anything further.

# GPU - AMD

{: .warning}
These are the steps I took, please do your own research before deciding to follow the article posted or this page.

## Drivers
Built into the OS

## Fixes
None