[![Build Status](https://travis-ci.org/wtanaka/ansible-role-hardlink.svg?branch=master)](https://travis-ci.org/wtanaka/ansible-role-hardlink)
[![CircleCI](https://circleci.com/gh/wtanaka/ansible-role-hardlink.svg?style=svg)](https://circleci.com/gh/wtanaka/ansible-role-hardlink)

wtanaka.hardlink
================

hardlink is a tool which replaces multiple copies of a file with
hardlinks. Inspiration came from http://code.google.com/p/hardlinkpy/,
but no code has been used. It was rewritten from scratch because
hardlinkpy code was not very readable and written against old Python
versions. The program requires Python 2.5 or newer, and should work
with Python 3 after running 2to3 on it.

Example Playbook
----------------

    - hosts: all
      roles:
         - wtanaka.hardlink

### `hardlink_should_shortcircuit`

Default: True

when True, the role short-circuits itself if hardlink is already installed

### All variables

The full set of configuration options available are visible in
[defaults/main.yml](defaults/main.yml)

License
-------

GPLv2

Author Information
------------------

http://wtanaka.com/
