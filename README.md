NTP
========

Install and configure NTP
This role enables users to install and configure ntp on their hosts.

Fixed error in vars that caused ntp to fail

Requirements
------------

This role requires Ansible 1.4 or higher, and platform requirements are listed
in the metadata file.

Examples
--------

1) Install ntp and set the default settings.

	- hosts: all
	  roles:
	    - role: ntp

2) Install ntp and set some custom servers.

	- hosts: all
	  roles:
	    - role: ntp
	      ntp_config_server: [2.ubuntu.pool.ntp.org, 1.ubuntu.pool.ntp.org]


License
-------

BSD

Author Information
------------------
Forked from https://github.com/resmo/ansible-role-ntp
with bits from https://github.com/geerlingguy/ansible-role-ntp
and
https://github.com/knopki/ansible-timezone

