papertrail
=========

Setup PapertrailApp remote logging on server.

Currently, supports only `rsyslog` service.

Includes offical recommendations for better stability.

Requirements
------------

This role is known-to-work on Ubuntu/Debian-based systems.
You need to have account at PapertrailApp, and know your host and port.

Role Variables
--------------

* `papertrail_destination` -  papertrail destination with port i.e. logs1234.papertrailapp.com:1234
* `papertrail_loglevel`: rsyslog loglevel. Default: *.*

Dependencies
------------

No dependencies

Example Playbook
----------------

Just include this role as in example:

    - hosts: all
      roles:
         - role: matic-insurance.papertrail
           papertrail_destination: logs1234.papertrailapp.com:1234

License
-------

MIT

Author Information
------------------

Matic is a communication platform that connects lenders and borrowers originating a new home loan. A borrower now knows where they are in the loan process and what they need to do to complete the loan.
