# k3s-single-ansible

# What is this?
This is a simple ansible playbook to install k3s on a single node. It is intended to be used for development and testing purposes.

# How to use
ansible install
```bash
sudo apt update
sudo apt upgrade -y
sudo apt install software-properties-common
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
```

run playbook
```bash
ansible-playbook build.yml -i inventory.yml --ask-become-pass
```

<!-- 太字にする -->
**Completed!**

check k3s cluster
```bash
watch sudo k3s kubectl get all
```
