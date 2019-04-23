Role Name
=========

Installing Zabbix agent.

Requirements
------------

None requirements

Role Variables
--------------
| Variable       | Description |
|--------------- | ----------- |
| zabbix_version | zabbix package version|
| zbx_srv | zabbix server variable|
| zbx_proxy | zabbix proxy server |

Example Inventory
------------

    [public:vars]
    zbx_srv=8.8.8.8
    zbx_proxy="zproxy.domain.kz"

    [private:vars]
    zbx_srv=192.168.0.1
    zbx_proxy="zproxy.domain.kz"

    [public]
    8.8.1.1
    ...

    [private]
    192.168.0.2
    ...

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables
passed in as parameters) is always nice for users too:

    - hosts: private
      roles:
        - zbx-agent

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a
website (HTML is not allowed).
