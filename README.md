# nginx

This role enables to install nginx on a system.

## Requirements

No requirements.

## Role Variables

| Name                                         | Type    | Location            | Description                                                                                              |
| -------------------------------------------- | ------- | ------------------- | -------------------------------------------------------------------------------------------------------- |
| nginx_version                                | string  | `defaults/main.yml` | The version of NGinx to install. Defaults to `1.20.0`.                                                   |
| nginx_centos_yum_repository_stable_url       | string  | `defaults/main.yml` | The base URL of Nginx stable yum repository. Defaults to `https://nginx.org/packages/centos`.            |
| nginx_centos_yum_repository_mainline_url     | string  | `defaults/main.yml` | The base URL of Nginx mainline yum repository. Defaults to `https://nginx.org/packages/mainline/centos`. |
| nginx_centos_gpg_key_url                     | string  | `defaults/main.yml` | The URL of Nginx GPG signing key. Defaults to `https://nginx.org/keys/nginx_signing.key`.                |
| nginx_centos_yum_repository_mainline_enabled | boolean | `defaults/main.yml` | A flag indicating if mainline yum repository should be enabled. Defaults to `false`.                     |

## Dependencies

No dependencies.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: julb.nginx }
```

## License

MIT

## Author Information

More to find on my [Github](https://github.com/julb).

## Contributing

This project is totally open source and contributors are welcome.

When you submit a PR, please ensure that the syntax has been checked.
