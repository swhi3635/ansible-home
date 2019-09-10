# pi-bootstrap Role
This role simply makes the necessary changes for the first-run of Ansible against a new Raspberry Pi.  The machine must have Raspbian installed, SSH enabled, and my SSH keys installed for the `pi` user.  This role is meant to be run immediately before running the `common` [role](https://github.com/swhi3635/ansible-home/tree/master/roles/common).

## Credits
The SSH username configs were taken from [Tom Bull's answer on Server Fault](https://serverfault.com/a/755006), with minor modifications.
