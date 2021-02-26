FortiVPN
=========

Install & configure fortinet-vpn

Requirements
------------

None.

Role Variables
--------------

```
fortivpn_resolved: false
fortivpn_gateway: 'vpn.gateway.com'
fortivpn_trustedcert: 'trusted0certifcate1'
fortivpn_user: 'name@email.com'
fortivpn_password: 'KaZoom666'
fortivpn_dns: '127.0.0.1;127.0.1.1;'
fortivpn_routes:
  - { name: route1, value: '1.1.0.0/16' }
  - { name: route2, value: '1.2.0.0/16' }
  - { name: route3, value: '1.3.0.0/16' }
  - { name: route4, value: '1.4.0.0/16' }
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: damienlagae.fortivpn, fortivpn_resolved: false }
