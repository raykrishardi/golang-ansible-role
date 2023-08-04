# Golang Ansible Role
The Golang ansible role allows you to install a specific Go version (only linux OS is supported at the moment) including setting up an example hello world Go web application as a `systemd` service.

- For Windows, you could simply install go using `choco install golang`
- For MacOS, you could simply install go using `brew install go`

## Getting Started

### Update the inventory file
Adjust the `example.inventory.ini` file according to your target host and SSH credentials then rename the file to `inventory.ini`

### Run on local machine
```
ansible-playbook testapp.yml -i inventory.ini
```

### Test on target machine (defined in the inventory file)
You could test whether the example hello world Go web application has been running successfully using the following commands on the target machine defined in the inventory file:
```
systemctl status hello-world
curl localhost:8080
```
