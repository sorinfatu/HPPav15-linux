##
This page is mostly for personal use but is being published in case others can benefir from the information here.
The main purpose of this is to facilitate instalation and configuration of Linux distros on  a HP Pavillion 15-ec00xxxx laptop.
##

# Personal configuration:
- AMD Ryzen™ 7 3750H
- NVIDIA® GeForce® GTX 1650 4GB
- 1TB HDD + 256GB NVME SSD
- 16GB RAM

# General considerations:  
Most Linux distros work out of the box on the laptop but there are considerations to take into account on some of them.
As a rule of thumb, as long as the kernel provided is at least version 5.4, the distro should be at least in a functioning state. This however does not guarantee everything will run smoothly.

# Required software (my personal options):
- browser - whatever (Firefox, Chromium/Chrome, Brave, Opera)
- password manager  - Bitwarden
- cloud storage - pCloud
- mail - using Protonmail (the only linux native client I managed to get working with it is Thunderbird but honestly I don't use it)
- office - OnlyOffice or WPS (I like the interface better for these two but whatever you need)
- music - Spotify
- video - SMPlayer
- gaming  - Lutris, Steam
- printing - I need printing to be able to handle on HP printer via a raspberry pi print server and another one with an inbuilt scanner  via USB connection
- extra stuff - gamemode, mangohud, goverlay

# Redundancy:
While btrfs is a nice option to have when installing, not all distributions have it out of the box so to make my life easier, my usual directories in /home/username/ are on the 1TB HDD and I just symlink them to my actual home. This way, I get to keep the files in them when switching distro. This has the disadvantage of not benefiting from the NVME speed so this stuff is optional. 

# Universal packages:
To have some consistency across distributions, I will use flatpak for some applications. This allows me install them and have them in a good working state no matter the platform.
