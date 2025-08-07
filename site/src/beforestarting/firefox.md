---
layout: page
title: Firefox Without Snap
parent: Before Installing Software
---
# Firefox Without Snap

{: .warning}
OPTIONAL - Only needed if you decided to disable Snap.

## Why Firefox
Well I couldn't find a reliable way of installing chrome and firefox was much easier to install and get running. If you happen to have removed Snap then you will not be able to find it in Apt or your software manager.

# Enabling Firefox Repository
Running the following:
```sudo add-apt-repository ppa:mozillateam/ppa```

And then pasting this below into terminal:

```
echo '
Package: *
Pin: release o=LP-PPA-mozillateam
Pin-Priority: 1001

Package: firefox
Pin: version 1:1snap*
Pin-Priority: -1
' | sudo tee /etc/apt/preferences.d/mozilla-firefox
```

From here you can either go to your software manager to install Firefox or run:

```
sudo apt install firefox
```

And the same goes for any Mozilla software.