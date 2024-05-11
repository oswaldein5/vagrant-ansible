## Install Nginx | Nodejs | Pm2 | App.js using Ansible

Generate a local image via **Vagrant** using **Ansible** for the installation and configuration of Ubuntu, Nodejs and Nginx as Web Server; Ensure the automatic start of the application (hello.js) when starting or restarting the Web Server.

Useful for building preconfigured virtual machine images for local environments or Cloud providers.

---

### 1. Ansible Playbook
   - [playbook.yaml](files/playbook.yaml)

### 2. Project files
   - [Script to run playbook](run_ansible.sh)
   - [JavaScript Application](files/hello.js)
   - [Nginx Web Server Configuration](files/nginx.conf)
  
### 3. Vagrant configuration file
   - [Vagrantfile](Vagrantfile)

### 4. Start Virtual Machine with Ubuntu Server 22.04
```sh
vagrant init bento/ubuntu-22.04
vagrant up
http://localhost
```
