raspi-ntpd-not-timesyncd
=========

timesyncd (a component of systemd) is not "real" NTP with its gentle failure characteristics.
It is an implementation of SNTP; the outcome is indistinguishable from running ntpdate
out of cron.

This role disables timesyncd, installs the reference ntp implementation, and
installs an ntp.conf with an appropriate selection of ntp servers


Requirements
------------

none

Role Variables
--------------

none - will be some in the next iteration or three

for your requirements.yml:

- src: https://github.com/res3066/ansiblerole-raspi-ntpd-not-timesyncd
  name: raspi-ntpd-not-timesyncd
  scm: git


Dependencies
------------

none

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - raspi-ntpd-not-timesyncd

License
-------

MIT

Author Information
------------------

Rob Seastrom <rs@seastrom.com>

