Windows Network Share status Prometheus Exporter
=========
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-iquzart.win_check_network_drive-blue)](https://galaxy.ansible.com/iquzart/win_check_network_drive)
[![License](https://img.shields.io/:license-mit-blue.svg)](https://badges.mit-license.org)
![Platforms](http://img.shields.io/badge/platforms-windows-green.svg?style=flat)
![Release](https://img.shields.io/github/v/release/iquzart/ansible-win-check-network-drive?style=flat)

Prometheus custom metrics for windows network share status 

```
# HELP windows_network_share_up windows network share status. 
# TYPE windows_network_share_up gauge
windows_network_share_up{mountpoint="//example-a.file.core.windows.net/share-name-x"} 1
windows_network_share_up{mountpoint="//example-b.file.core.windows.net/share-name-y"} 1
```

Requirements
------------

windows exporter installed and configured to scrap text file from C:\Prometheus\custom_metrics\promfiles\*.prom

Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: iquzart.win-check-network-drive, network_drives: 'Z:\' }

License
-------

MIT

Author Information
------------------

Muhammed Iqbal <iquzart@hotmail.com>
