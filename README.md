** This playbook has been built to customize Kali Linux, therefore only works on systems using the apt package manager **

Instructions 

- Install ansible on host device (Kali Linux only supports ansible-core, this will suffice)
- Clone the repo and enter it (git clone)
- Ensure you have a sudo token (run sudo whoami)
- Run ansible-playbook main.yml 

Post-Installation 

It is reccomended to log out or reboot the device after installation, this will solve any issues with config files being sources correctly. I3wm also needs to be selected on the login page of the device to be used. 

** Thanks to Ippsec for inspiring this project, note that the firefox extensions playbook is borrowed from his Parrot Ansible playbook 
- https://github.com/IppSec/parrot-build
