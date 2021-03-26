ansible-role-openldap
=========

Configure an openldap server.

Requirements
------------

certificates are required if openldap_server_tls: True


Role Variables
--------------

openldap_server_tls: True

See the defaults/main.yml , do change passwords!

Dependencies
------------

EL7


Example Playbook
----------------

Including an example of how to use your role. configurables parameter is optional. If you define it, will expect certificates to be found in ansible vault. If you omit it, OpenLDAP will used defatul installation selfsigned certificates

    - hosts: servers
      roles:
         - { role: ansible-role-openldap, configurables: ['certs'] }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).

Inspiration from:
 - https://github.com/kbrebanov/ansible-openldap
 - http://www.server-world.info/en/note?os=CentOS_7&p=openldap
