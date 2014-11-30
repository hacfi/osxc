# osxc playbook for PHP development

## Installation

1. Install [Apple Xcode Command Line Tools](https://developer.apple.com/downloads/): [6.1 for 10.9](https://developer.apple.com/downloads/download.action?path=Developer_Tools/command_line_tools_os_x_10.9_for_xcode__xcode_6.1/command_line_tools_for_osx_10.9_for_xcode_6.1.dmg)

2. Install Ansible:

```sh
git clone git@github.com:ansible/ansible.git ~/src/github.com/ansible/ansible
cd ~/src/github.com/ansible/ansible
git submodule update --init --recursive
sudo make install
```

3. Download this repo:

```sh
git clone git@github.com:hacfi/osxc.git ~/src/github.com/hacfi/osxc
cd ~/src/github.com/hacfi/osxc
```

4. Install requirements:

```sh
ansible-galaxy install -r requirements.yml
```

5. Install individual playbooks:

```sh
ansible-playbook osx.yml
ansible-playbook configuration.yml
ansible-playbook apps.yml
ansible-playbook fonts.yml
```


For more information check out [osxc/starter](https://github.com/osxc/starter).