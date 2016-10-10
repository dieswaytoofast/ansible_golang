Role Name
=========

Installs go on Ubuntu (and other Linux)

Requirements
------------

Requires Ansible 2.0 or higher.

Example playbook -

```
#!/usr/bin/env /usr/bin/ansible-playbook
---

- hosts: localhost
  vars:
    ansible_golang_install_glide: true
    ansible_golang_user: vagrant
    ansible_golang_group: vagrant
    ansible_golang_gopath: "$HOME/go"
  roles:
    - ansible_golang
```


Role Variables
--------------

* `ansible_golang_user`: The user that go is installed as/for. _Must be defined in your playbook_
* `ansible_golang_group`: The group that go is installed as/for. _Must be defined in your playbook_
* `ansible_golang_user_dir`: $GOPATH. _Must be defined in your playbook_

* `ansible_golang_tar_name`: The specific version you want to install from the [Downloads page](https://golang.org/dl/)
* `ansible_golang_tar_checksum`: Checksum for the above tar from the [Download Page](https://golang.org/dl/)
* `ansible_golang_version_and_target`: Basically what `go version` returns (e.g. `go version go1.6.1 darwin/amd64`)
* `ansible_golang_download_base_url`: The base URL that you get the download from - probably not something you need to touch
* `ansible_golang_install_glide` : Install [Glide](https://glide.sh) if defined
* `ansible_golang_glide_download_base_url`: The base URL for [Glide](https://glide.sh)
* `ansible_golang_glide_sh_name`: The executable that does the [Glide](https://glide.sh) installation


Dependencies
------------

None.

License
-------

BSD

Author Information
------------------

Mahesh Paolini-Subramanya : @dieswaytoofast everywhere - [twitter](https://twitter.com/dieswaytoofast) / [linkedin](https://www.linkedin.com/in/dieswaytoofast) / [github](https://github.com/dieswaytoofast)
