Role Name
=========

Installs go on Ubuntu (and other Linux)

Requirements
------------

Requires Ansible 2.0 or higher.

Role Variables
--------------

* `golang_tar_name`: The specific version you want to install from the [Downloads page](https://golang.org/dl/)
* `golang_tar_checksum`: Checksum for the above tar from the [Download Page](https://golang.org/dl/)
* `golang_version_and_target`: Basically what `go version` returns (e.g. `go version go1.6.1 darwin/amd64`)
* `golang_download_base_url`: The base URL that you get the download from - probably not something you need to touch
* `golang_install_glide` : Install [Glide](https://glide.sh) if defined


Dependencies
------------

None.

License
-------

BSD

Author Information
------------------

Mahesh Paolini-Subramanya : @dieswaytoofast everywhere - [twitter](https://twitter.com/dieswaytoofast) / [linkedin](https://www.linkedin.com/in/dieswaytoofast) / [github](https://github.com/dieswaytoofast)
