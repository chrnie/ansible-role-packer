# Ansible Role: packer

An Ansible role for managing HashiCorp [Packer](https://packer.io/)

## How To?

When configured connect to your machine and create the base Images. 
We use xAuth to tunnel the VNC screen automagically to you workstation.

```sh
$ ssh -X root@srvXY
root@srvXY /opt/packer/distros/centos7 # packer build centos7-base.json 
[...]
==> Builds finished. The artifacts of successful builds are:
--> qemu: VM files in directory: centos7-base-img
```

## Requirements

- 64bit Linux
- virt-manager on your workstation


## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    packer_version: "1.0.0"

define packer version


## Dependencies

chrnie.unzip


## Example Playbook

    - hosts: all
      roles:
        - chrnie.packer


## License

Apache License 2.0

## Author Information

Created in 2017 by Christoph Niemann, https://github.com/chrnie
