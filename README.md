# dev-playbooks

Ansible Playbooks for setting up dev environment and dev linux laptops written by [Raza Akbari](https://github.com/rhakbari)

## Installing Ansible

```bash
sudo apt-add-repository --yes --update ppa:ansible/ansible
```

```bash
sudo apt install ansible
```

# Installing Dev packages for Frontend and Backend

```bash
ansible-playbook -i '/home/rhakbari/Desktop/ivolve-repos/dev-playbooks' install-java17.yml
```

```bash
ansible-playbook -i '/home/rhakbari/Desktop/ivolve-repos/dev-playbooks' --extra-vars "node_version=16.x" --ask-become-pass install-node.yml
```

```bash
ansible-playbook -i '/home/rhakbari/Desktop/ivolve-repos/dev-playbooks' install-go.yml
```

```bash
ansible-playbook -i '/home/rhakbari/Desktop/ivolve-repos/dev-playbooks' install-mysql.yml
```

```bash
ansible-playbook -i '/home/rhakbari/Desktop/ivolve-repos/dev-playbooks' --ask-become-pass install-neovim.yml
```