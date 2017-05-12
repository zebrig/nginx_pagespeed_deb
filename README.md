# nginx_pagespeed_deb
Script that creates deb files for Ubuntu of nginx with pagespeed module compiled

## Why is this script created?
Mostly, all instructions of how to make nginx with pagespeed require a lot of manual work to do. I have decided to make it unattended and automated. 

Another thing is, I don't really like compiling and running compiled binaries on debian/ubuntu. I prefer creating deb files. Thus, installing and deleting packages is far more predictable.

So, this script downloads the current stable version of nginx and mod_pagespeed, compiles it together and creates a .deb file for comfortable installation. After it, you can simply install nginx with mod_pagespeed by:
`dpkg -i <generated file>.deb`

I successfully use it on Ubuntu 16.04. But it runs on any ubuntu, all you need is to change the version name of Ubuntu in the line
`UBUNTU_VERSION="xenial"`
