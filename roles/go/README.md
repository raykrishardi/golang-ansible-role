Role Name
=========

The Go ansible role allows you to install a specific go version (only linux OS is supported at the moment) including setting up an example hello world Go web application as a systemd service.

For Windows, you could simply install go using `choco install golang`

For MacOS, you could simply install go using `brew install go`

Requirements
------------

- ssh authentication to the instance (ssh keys or password)
- sudo permission and ability to run sudo without password


Role Variables
--------------

`vars/main.yml`
- Variables defined in this file is NOT recommended to be changed

`defaults/main.yml`
- Variables defined in this file can be changed as per your requirements

Dependencies
------------



Example Playbook
----------------

Please refer to `testapp.yml` for an example playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
