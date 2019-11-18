# Ansible Practice

Simple repository of practicing Ansible with Vagrant when studying

Your host would be an Ansible control machine and the VM started by Vagrant would be a managed node

## Requirements

- Hypervisor
- Vagrant
- Ansible

*Note: In this practice, VirtualBox is used as hypervisor. If other hypervisor is used, please modify key file location in your inventory file*

## Usage

Start virtual machine and now you are ready to use Ansible to deploy
```
$ cd vm; vagrant up
```

*Note: The first virtual machine started by Vagrant would have the SSH connection port `2222`. If there are other virtual machines existing alreay, please check SSH configuration with `vagrant ssh-config` and replace the connection port in the inventory file*

Test SSH connection
```
$ ansible all -m ping
```

## ONOS/Mininet Deployment

This is an Ansible practice to deploy a Software-Defined Network environment with ONOS as the controller and Mininet
