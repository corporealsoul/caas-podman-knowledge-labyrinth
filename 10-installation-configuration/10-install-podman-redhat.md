### YUM Installation

https://podman.io/docs/installation

**These tools—Podman, Buildah, and Skopeo—are lightweight, secure, and designed to manage containers directly on Red Hat Enterprise Linux.**

`[anup@rhel-92-104 ~]$ sudo dnf install container-tools`

`[anup@rhel-92-104 ~]$ docker --version`

`[anup@rhel-92-104 ~]$ podman --version`

**Optionally, you can also install the podman-docker package, which replaces the Docker command-line interface with matching Podman commands:**

`[anup@rhel-92-104 ~]$ sudo dnf install podman-docker`

`[anup@rhel-92-104 ~]$ podman info`


### Ansible Installation

`[anup@rhel-92-104 ~]$ ansible -m ping all`

`[anup@rhel-92-104 playbook]$ ansible-inventory --list`

<br>

`[anup@rhel-92-104 ~]$ cd /etc/ansible/roles`

`[anup@rhel-92-104 roles]$ sudo ansible-galaxy init podman-installation-redhat`

<br>

`[anup@rhel-92-104 ~]$ cd /etc/ansible/playbook/`

<br>

`[anup@rhel-92-104 playbook]$ ansible-playbook podman-installation-redhat-site.yml --syntax-check`

`[anup@rhel-92-104 playbook]$ ansible-playbook podman-installation-redhat-site.yml --ask-become-pass`

<br>

`anup@ubuntu-22042-108:~$ podman --version`

<br>
