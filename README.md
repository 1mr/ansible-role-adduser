# adduser

[![Build Status](https://travis-ci.com/1mr/ansible-role-cron.svg?branch=master)](https://travis-ci.com/1mr/ansible-role-cron)

This role helps to manage local users.

## Requirements

This role requires ansible 2.5 or higher.

## Role Variables

`adduser`, default:

```yaml
adduser:
  - name: debian
    state: absent
```

Example:

```yaml
    adduser:
      users:
        - alice
        - bob
```

## Dependencies

None

## Example Playbook

```yaml
    - hosts: servers
      roles:
         - { role: 1mr.adduser, tags: adduser }
```

## License

MIT

## Author Information

This role was created by Stas Stavnichuk.
