# mac-dev-playbook

Ansible Playbook for Setting up my Mac according to my preference.

### Applications that will be Installed

1. Brave Browser
2. Figma
3. Google Chrome
4. Iterm2
5. My SQL Workbench
6. Obsidian
7. Postman
8. Telegram
9. Vagrant
10. Virtualbox
11. Visual Studio Code

### Instructions to run

1. Installing Apple's command line tools

   ```
   xcode-select --install
   ```

2. Install ansible via Pip3

   ```
    pip3 install --upgrade pip3
   ```

   ```
   pip3 install ansible
   ```

3. Install the Ansible requirements

   ```
   ansible-galaxy install -r requirements.yml
   ```

4. Run the Ansible playbook
   ```
   ansible-playbook main.yml --ask-become-pass
   ```

### Global packages installation

To automate packages installation globally either from npm / pip / gems. Add the package name to

1. npm_packages -> npm packages
2. pip_packages -> python packages
3. gem_packages -> Ruby Gem packages

in the `vars/main.yml` file
