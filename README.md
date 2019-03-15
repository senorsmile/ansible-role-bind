ansible-role-bind
=========

ansible role to manage bind server


Requirements
------------

ansible >= 2.5

Role Variables
--------------

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }


Inventory vars:

    bind_dns_records_example:
      - name: example.com
        addr: "1.2.3.4"
        records:
          - type: A
            name: subdomain 
            addr: "1.2.3.5"
    ... # similar for example2 and example3

    bind_dns_records:
      - "{{ bind_dns_records_example }}"
      - "{{ bind_dns_records_example2 }}"
      - "{{ bind_dns_records_example3 }}"

License
-------

MIT

Author Information
------------------

- Shaun Smiley
