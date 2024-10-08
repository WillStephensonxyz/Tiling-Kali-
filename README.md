# Tiling Kali

** This playbook has been built to customize Kali Linux, therefore only works on systems using the apt package manager **

This ansible playbook customizes Kali Linux to my personal prefrences, it will install/configure a few tools not native to the distribution

- i3wm (window manager)
- rofi 
- tmux configuration
- docker
- .zshrc config

Additional tools are also installed for penetration testing, see the install-tools role for these programs

Firefox extensions are also installed, namely foxyproxy for use with burpsuite

### Instructions 

- Install ansible on host device (Kali Linux only supports ansible-core, this will suffice)
- Clone the repo
- Ensure you have a sudo token (run sudo whoami)
- Tmux needs to be run for the first time to create the defaults directory to avoid erros
- Run ansible-playbook main.yml 


```bash
apt install ansible
git clone https://github.com/WillStephensonxyz/Tiling-Kali-.git
sudo whoami 
tmux
ansible-playbook main.yml 
```

### Post-Installation 

You'll need to log out or reboot the device after installation, this will solve any issues with config files being sourced correctly. I3wm also needs to be selected on the login page of the device to be used. 
 Thanks to Ippsec for inspiring this project, note that the firefox extensions playbook is borrowed from his Parrot Ansible playbook 
- https://github.com/IppSec/parrot-build
