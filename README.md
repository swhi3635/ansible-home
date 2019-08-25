# Overview
This is just a pet project of mine, with the primary goal of familiarizing myself with Ansible, and a few other tools.  I spent a few years working with Salt, and I've often wondered how it compared to Ansible.  

In my experience, working on technical projects for the sole purpose of learning a new language, software tool, etc. can be difficult.  Thus, it is important to come up with a deliverable that provides some value to me, while tying the new piece of technology into the requirements of the project.

In the case of this project, I've decided to migrate my media streaming server from a rented dedicated server into my home.  I'm doing this for a few reasons:

 - The dedicated server is running Ubuntu 14.04, which is essentially EOL
 - I did not use configuration management when I first set up the old server almost 5 years ago.  Thus, it has been difficult to maintain over time.
 - The home server is on better hardware with full virtualization support
 - I have gigabit fiber at home, which is 10x faster than the rented machine
 - I _might_ save money in the long run, since the ongoing cost of keeping the new machine online is less than the cost of the dedicated server.
 - Most importantly, it will be fun!

# Technical details

## Goals
 - Ensure a positive user experience for anyone using the services provided by this system (friends/family using my media library, etc.)
 - Utilize Ansible to allow me to fully configure the baremetal machine, guest VMs, and any containers from scratch with minimal manual effort
 - Use containers to create logical separation between each distinct service/application in the system

## Hardware
I found an old HP business-grade desktop on Craigslist for $80.  It should have more than enough horsepower for my needs.

**HP Compaq Elite 8300**
- CPU: Intel Core i7 3770 ([ARK](https://ark.intel.com/content/www/us/en/ark/products/65719/intel-core-i7-3770-processor-8m-cache-up-to-3-90-ghz.html))
- Memory: 16 GB DDR3
- Disk: 2x SanDisk 128 GB SSD

**Upgrades**
- 2x WD Red 4TB hard drives
