fritzing_install
====================

This role downloads the latest version from Fritzing to the Ansible controller.
It does this by checking if the latest version on the Download page.
If the file for the latest version does exist, it does not attempt to download it.
In the installation process the file is uploaded to the targets, extracted and a
symlink is created in /usr/bin. It also does not upload and extract if the installed
version matches the latest version of the fritzing on the download page.

Requirements
---------------

TODO: Probably Kubuntu, Ubuntu, Debian ... 

Role Variables
------------------

| Variable                       | Description                                 | Default    |
| ------------------------------ | ------------------------------------------- | ---------- |
| fritzing_install_directory     | directory the fritzing folder will be place | /usr/share |

Dependencies
---------------

No role dependencies

Example Playbook
--------------------

    - hosts: desktops
      roles:
         - cyborg_x1.fritzing_install

License
---------

BSD

Author Information
-----------------------

Christian Holl: cyborgx1 [the at] gmail [the dot] com

