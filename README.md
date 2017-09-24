Binkd FTN Mailer [![Build Status](https://travis-ci.org/davestephens/ansible-role-binkd.svg?branch=master)](https://travis-ci.org/davestephens/ansible-role-binkd) 
===========
Installs [Binkd FTN mailer](https://github.com/pgul/binkd). 

Requirements
------------

Ubuntu or Debian based Linux distribution. A Raspberry Pi with Raspbian installed is a great candidate!

Role Variables
--------------

````yaml
binkd:
  home: "/bbs/binkd" # where to install Binkd
  repo: https://github.com/pgul/binkd.git # Binkd repo to use
````
Dependencies
------------

    - Binkd source - defaults to pulling from https://github.com/pgul/binkd.git 

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: davestephens.binkd }

Testing
-------
The role is tested against Debian and Ubuntu with [Travis CI](https://travis-ci.org/davestephens/ansible-role-binkd).

License
-------

MIT

Author Information
------------------
[David Stephens](http://www.davidstephens.uk) - a DevOps and platform engineer from London, UK.
