## socat

[![Build Status](https://travis-ci.org/Oefenweb/ansible-socat.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-socat) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-socat-blue.svg)](https://galaxy.ansible.com/Oefenweb/socat)

Set up (the latest version of) [socat](http://www.dest-unreach.org/socat/) in Debian-like systems.

#### Requirements

* `build-essential` (will be installed)
* `libreadline-dev` (will be installed)
* `libssl-dev` (will be installed)
* `libwrap0-dev` (will be installed)

#### Variables

* `socat_version`: [default: `1.7.3.1`]: Version to install
* `socat_remove_distro_version`: [default: `true`]: Whether or not to remove the distribution version
* `socat_configure_options`: [default: `[]`]: Options to pass to `./configure` (e.g. `['--disable-readline']`)

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - socat
```

#### License

MIT

#### Author Information

* Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-socat/issues)!
