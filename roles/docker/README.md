# Docker Role
Currently, this role is responsible for the following:
 - Installing necessary packages to build, run, etc. docker containers and images
 - Create storage volumes using the available block devices on my host machine
   - If/when additional physical hosts are added to my lab, I will need to separate these and/or template them out, since I don't expect all of my hosts to have the same storage configurations.
 - Generate a templated docker-compose.yml file.  I'd like to move the docker-compose work to a separate repository at some point.

## Included roles:
- [geerlinguy/docker](https://galaxy.ansible.com/geerlingguy/docker)
- [geerlinguy/pip](https://galaxy.ansible.com/geerlingguy/pip)
- [mrlesmithjr/mdadm](https://galaxy.ansible.com/mrlesmithjr/mdadm)
