rpi_wifi_usb_smb
================
[![Ansible Lint](https://github.com/oxivanisher/role-rpi_wifi_usb_smb/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-rpi_wifi_usb_smb/actions/workflows/ansible-lint.yml)

This role configures a SMB/CIFS share path. It is intended to be used with the [rpi_wifi_usb](https://github.com/oxivanisher/role-rpi_wifi_usb.git) role.

As always: Use at your own risk!

Role Variables
--------------

| Name                             | Comment                                             | Default value                |
|----------------------------------|-----------------------------------------------------|------------------------------|
| rpi_wifi_usb_smb_share_path      | Mount point to be shared via SMB/CIFS               | `/mnt/wifi_usb_share`        |

Example Playbook
----------------
```yaml
- name: Raspberry Pi Wifi USB stick
  hosts: wifi_usb
  roles:
    - role: oxivanisher.raspberry_pi.rpi_wifi_usb_smb                 # configure rpi wifi usb smb share
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.raspberry_pi](https://galaxy.ansible.com/ui/repo/published/oxivanisher/raspberry_pi/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-raspberry_pi).
