Windows Network Share status Prometheus Exporter
=========
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-iquzart.win_check_network_drive-blue)](https://galaxy.ansible.com/iquzart/win_check_network_drive)
![Molecule Test](https://github.com/iquzart/ansible-win-check-network-drive/workflows/Molecule%20Test/badge.svg?) 
[![License](https://img.shields.io/:license-mit-blue.svg)](https://badges.mit-license.org)
[![Platforms](http://img.shields.io/badge/platforms-windows-lightgrey.svg?style=flat)](#)
![Release](https://img.shields.io/github/v/release/iquzart/ansible-win-check-network-drive?style=plastic)

Prometheus custom metrics for windows network share status 

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
