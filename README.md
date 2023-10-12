# Vagrant Jenkins

Automatically sets up Jenkins on a Vagrant box using Ansible.

## Requirments

Ansible: https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

Vagrant: https://developer.hashicorp.com/vagrant/docs/installation

## Usage

```vagrant up```

```ansible-playbook -i inventory/virtualbox.hosts playbooks/virtualbox.yml```

## Setup Jenkins UI

```vagrant ssh jenkins```
```sudo cat /var/lib/jenkins/secrets/initialAdminPassword```
```Jenkins URL: http://192.168.56.13:8080/```

## Cleanup

* `vagrant halt; vagrant destroy -f`
