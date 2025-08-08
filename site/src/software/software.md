---
layout: page
title: Software
permalink: /software
nav_order: 40
has_children: true
---

# Software

I am detailing some common software unrelated to hardware specific requirements that might be useful such as Discord, Steam, Lutris etc. I'll expand on these as I go along and find bits and pieces.

# Debian Package Installs (or equivalent)

When downloading `.deb` packages you may find that the default option to install through the UI sometimes fails with "unresolved dependencies". Well this is one of those moments that diving into the terminal will help you.

Open up a terminal and use the `cd` command to navigate to where you downloaded the file to (usually `~/Downloads`).
Then run the following command

```
sudo dpkg -i <package>.deb
```

This might end up in an error about dependencies as well, this is fine. Next run:

```
sudo apt-get -f install
```

This should now install the dependencies and finish off the package you were trying to install.

{: .fs-6 .fw-300 }