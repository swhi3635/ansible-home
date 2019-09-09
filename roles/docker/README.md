# Docker Role
Currently, this role is responsible for the following:
 - Installing necessary packages to build, run, etc. docker containers and images
 - Create a storage volume using an available block device on my host machine
   - If/when additional physical hosts are added to my lab, I will need to separate these and/or template them out, since I don't expect all of my host machines to have identical storage configurations.

## Included roles:
- [geerlinguy/docker](https://galaxy.ansible.com/geerlingguy/docker)
- [geerlinguy/pip](https://galaxy.ansible.com/geerlingguy/pip)
