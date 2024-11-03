# Ansible playbook demo
This playbook is a demo which sets up a local developer machine.

Specific applications included:
- Ansible
- Docker (desktop)
- Homebrew for Linux
- Python 2.7.18

## Requirements
This playbook was written for Ubuntu Desktop 22.04 LTS, using the Gnome Desktop.

Make sure to install Ansible beforehand to run the playbook.
```
apt install ansible
```

This playbook also assumes the use of Ansible 2.10.8, as that is the latest
included in the Ubuntu 22.04 apt repository at the time of this writing.

## Running
The playbook runs commands that require root privileges. In order to run the
playbook without errors, include the `--ask-become-pass` option in the run command, and enter your user password.
```
ansible-playbook setup_dev.yml --ask-become-pass
```

After the playbook has ran, source your `.bashrc` file or login to the
machine to load.
