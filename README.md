# Windows To Linux
## Current State - Testing

| Item | Type | Status | Workaround |
|------|------|--------| ---------- |
| Heros Of the Storm | Game | Passed | N/A |
| Factorio | Game | Passed | N/A |
| Satisfactory | Game | Passed | N/A |
| Steam | App | Passed | N/A |
| Battle.net | App | Passed | N/A |
| OpenRGB | App | Partial | N/A |
| K70 RGB Pro V2 | Hardware RGB | Fail | Yes |
| Asus / Corsair Fans | Hardware Control | Testing | Unknown |


## Overview

I have made the decision to not upgrade to Windows 11 (for my own reasons) and will be left with few options. I want to document all the things that I am doing to migrate over to Linux with any potential gotchas, hardware issues and workarounds so that someone else may benefit from this. I will do my best to document as I go but a few things may get lost.

## Use Case
On my main machine I use it for light MS Office bits, development, gaming and music production.

## Hardware

|Type|Manufacturer| Model |
|----|------------|-------|
| CPU | AMD| Ryzen 5800 X |
| Motherboard | Asus | B550-F Gaming |
| GPU | Nvidia | RTX 3070 |
| Keyboard | Corsair | K70 RGB PRO V2 |
| Mouse | Logitech | G502 Hero |
| RAM | - | 32GB |

## Dual Boot
To make sure that I give Linux a decent chance, I will dual boot Linux onto a new 2TB SSD away from my Windows partition and drive. This way if anything goes wrong I don't risk my Windows install and I can always go back to it when / if i need to.

## Distribution Chosen
### Original Choice - Mint
I originally chose Linux Mint for the distro of choice purely because I had used it in the past and it felt relatively user friendly.
Having booted into the "Live CD" I had to choose "Something else" as the other two options would have either wiped my Windows drive OR resized my Windows partition. In this mode I was faced with creating partitions manually for the dual boot and there were several posts saying that the installer had a bug and would actually modify my Windows Boot Loader.
So for me, this was a non starter.

### Kubuntu
A friend recommended Kubuntu to me having used it for a considerable time and had few issues with it. This seemed like a reasonable suggestion and as I was able to select the drive I wanted to install to, this seemed easiest.
Kubuntu was installed in no time at all and I now have a fresh new Linux install to call home for a couple of months whilst I trial it.

## Snap
I don't want snap, end of. My reasons are my own but nothing I read has anything good to say about it. So it needs to go. Following instructions [here](https://www.kubuntuforums.net/forum/general/miscellaneous/coding-scripting/669539-script-to-get-rid-of-snap), I removed snap before doing anything.

## Chromium
Well, I looked everywhere for a decent tutorial on installing Chromium but in the end settled for going with Firefox.

## Firefox - Without Snap
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
I could then simply run `sudo apt install firefox`

## More TO Come
TBD

