# Role Name

Installs iptables and ensure that it's running

## Installation

To install the role:

```
ansible-galaxy role install chrissayon.iptables
```

## Role Variables

| Variable                  | Description                                                                                                                                                     |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| hardening_type            | How to harden the server depending on your application                                                                                                          |
| remove_existing_firewalls | Whether the existing firewalls on the OS should be removed (If you're setting up iptables, you should remove any other applications that also interact with it) |

## Example Playbook

```
- hosts: all
  roles:
      - chrissayon.iptables
```
