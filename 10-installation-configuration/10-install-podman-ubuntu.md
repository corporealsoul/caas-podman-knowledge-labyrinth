### APT Installation

https://podman.io/docs/installation

`anup@ubuntu-22042-108:~$ sudo apt-get -y install podman`

`anup@ubuntu-22042-108:~$ docker --version`

`anup@ubuntu-22042-108:~$ podman --version`

`anup@ubuntu-22042-108:~$ podman info`

<br>

### Ansible Installation

`[anup@rhel-92-104 ~]$ ansible -m ping all`

`[anup@rhel-92-104 playbook]$ ansible-inventory --list`

<br>

`[anup@rhel-92-104 ~]$ cd /etc/ansible/roles`

`[anup@rhel-92-104 roles]$ sudo ansible-galaxy init podman-installation-ubuntu`

<br>

`[anup@rhel-92-104 ~]$ cd /etc/ansible/playbook/`

<br>

`[anup@rhel-92-104 playbook]$ ansible-playbook podman-installation-ubuntu-site.yml --syntax-check`

`[anup@rhel-92-104 playbook]$ ansible-playbook podman-installation-ubuntu-site.yml --ask-become-pass`

<br>

`anup@ubuntu-22042-108:~$ docker --version`

<br>
