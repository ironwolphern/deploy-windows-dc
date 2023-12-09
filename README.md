:construction: ***DEVELOPING*** :construction:

**Ansible Playbook to deploy Active-Directoy and DNS**
======================================================

![Ansible](https://img.shields.io/badge/ansible-%231A1918.svg?style=flat&logo=ansible&logoColor=white)
![GitHub License](https://img.shields.io/github/license/ironwolphern/deploy-windows-dc)
![GitHub release (with filter)](https://img.shields.io/github/v/release/ironwolphern/deploy-windows-dc)
![GitHub pull requests](https://img.shields.io/github/issues-pr/ironwolphern/deploy-windows-dc)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/ironwolphern/deploy-windows-dc)
![GitHub issues](https://img.shields.io/github/issues/ironwolphern/deploy-windows-dc)
[![Ansible Lint](https://github.com/ironwolphern/deploy-windows-dc/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/ironwolphern/deploy-windows-dc/actions/workflows/ansible-lint.yml)
![Dependabot](https://badgen.net/github/dependabot/ironwolphern/deploy-windows-dc)

This is an Ansible playbook for deploy Active-Directoy and DNS server in a Windows Server virtual machine. When launch the playbook,  
asks for the following parameters to enter:

- Name of the new domain controller
- Name of domain
- Network CIDR of the new domain controller, not the ip address
- Administrator user
- Password user

*Playbook Features*
-------------------

- Rename of virtual machine
- Install and config Active Directory controller
- Install and config DNS server

*Usage/Example*
---------------

```bash
ansible-playbook -i inventories/inv.esx.vmware.yml deploy-ad.yml
```

*License*
---------

MIT

*Author Information*
--------------------

This playbook was created in 2023 by:

- Fernando Hernández San Felipe (ironwolphern@outlook.com)
