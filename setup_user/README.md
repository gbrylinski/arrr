### What is it for?

Setups a *user*. It creates an OS account if necessary, disables password and adds SSH keys allowed to login. 

### Variables

it's configured via a base hash named `setup_user` after a role name.

#### setup_user.name `string`

specifies a name of the user to create.

#### setup_user.allowed_ssh_keys `array`

lists ssh keys to add as authorized keys for created user.

### example

```yaml
# playbook.yml
- hosts: all
  roles:
    - role: setup_user
      setup_user:
        name: 'demo_user'
        allowed_ssh_keys:
          - https://github.com/gbrylinski.keys
```
