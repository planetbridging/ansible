# ANSIBLE EXAMPLES
Just a couple examples of ansible

```
$ ansible-playbook vagrant.yaml
```
Vagrant is a fun little tool to auto deploy images into virtualbox and with this current setup it will auto download the ubuntu/xenial64 image then deploy 3 boxes

```
$ ansible-playbook git_example.yaml
```
Example of git

```
$ ansible-playbook setup_vm_example.yaml
```
In the off chance needing to talk to vmware and/or vsphere this is a setup


```
$ ansible-playbook ssh_example.yaml
```
Installs and auto generates ssh keys with openssh

```
$ ansible-playbook ssl_example.yaml
```
Installs and auto generates certificates .pem .crt .csr for self signing


Random commands that helped with errors
```
sudo chown -R "${USER:-$(id -un)}" .
```
Helped with the mixed sudo and normal git add .

```
sudo virtualbox
```
To access the created virtualbox