# Role ivansible.dev_vagrant

Install vagrant and plugins.
See instructions here: https://www.vagrantup.com/docs/installation/


## Requirements

None


## Variables

Available variables are listed below, along with default values.

    vagrant_package_url: latest

This can be one of:
 `ppa` (not recommended),
 `latest` (see here: https://www.vagrantup.com/downloads.html),
 url of vagrant `.deb` package.

    vagrant_plugin_list: []

If this list is not empty, a number of vagrant plugins will be installed
locally for target user (or reinstalled if vagrnant was upgraded).

    vagrant_allow_reinstall: no

Allows to refresh already downloaded redistributables.

    vagrant_cloud_token: ""

If this setting is defined and non-empty, target user will be
authenticated with vagrant cloud.


## Tags

- `dev_vagrant` -- install vagrant package
- `dev_vagplugins` -- install vagrant plugins
- `dev_vaglogin` -- authenticate with vagrant cloud


## Dependencies

None


## Example Playbook

    - hosts: vag2
      roles:
        - role: ivansible.dev_vagrant


## License

MIT


## Author Information

Created in 2018 by [IvanSible](https://github.com/ivansible)
