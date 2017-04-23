# Ansible Role: packer

An Ansible role for managing HashiCorp [Packer](https://packer.io/)


## Requirements

64bit Linux


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
