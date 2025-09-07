# pocketid ansible role

[![Actions Status - Main](https://github.com/juju4/ansible-pocketid/workflows/AnsibleCI/badge.svg)](https://github.com/juju4/ansible-pocketid/actions?query=branch%3Amain)
[![Actions Status - Devel](https://github.com/juju4/ansible-pocketid/workflows/AnsibleCI/badge.svg?branch=devel)](https://github.com/juju4/ansible-pocketid/actions?query=branch%3Adevel)

Setup [pocketid](https://github.com/pocket-id/pocket-id), A simple and easy-to-use OIDC provider that allows users to authenticate with their passkeys to your services.

See also
* https://pocket-id.org/
* https://docs.pocket-id.org/
* https://demo.pocket-id.org/

To sign up aka create account, go to <https://pocketid/setup>.
To sign in from secondary device with different passkeys, use "My Account > login code" option.

## Requirements & Dependencies

### Ansible

It was tested on the following versions:
 * 2.18

### Operating systems

Tested on Ubuntu 24.04, 22.04, Centos/Rockylinux 9.

## Example Playbook

Just include this role in your list.
For example

```yaml
- host: myhost
  roles:
    - juju4.pocketid
```

you probably want to review variables

## Variables

TBD

## Continuous integration

```
$ pip install molecule docker
$ molecule test
$ MOLECULE_DISTRO=ubuntu:24.04 molecule test --destroy=never
```

## Troubleshooting & Known issues

TBD

## License

BSD 2-clause
