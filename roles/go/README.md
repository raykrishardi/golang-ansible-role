Role Name
=========

The Golang ansible role allows you to install a specific Go version (only linux OS is supported at the moment) including setting up an example hello world Go web application as a systemd service.

- For Windows, you could simply install go using `choco install golang`
- For MacOS, you could simply install go using `brew install go`

You could test whether the example hello world Go web application has been running successfully using the following commands on the target machine defined in the inventory file:
```
systemctl status hello-world
curl localhost:8080
```

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

Please refer to `testapp.yml` for an example playbook (including overwritting the default ansible role variable value)

License
-------

BSD

Author Information
------------------

[Ray Layadi](https://www.linkedin.com/in/ray-krishardi-layadi/)
