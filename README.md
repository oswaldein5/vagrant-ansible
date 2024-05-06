## Install Nginx | Nodejs | Pm2 | App.js using Ansible

Generate an image with an application with NodeJs already installed and configured with Nginx as a Web Server; Ensure the automatic start of the application (hello.js) when the Web Server starts.

Useful for building preconfigured virtual machine images for local environments or Cloud providers.

---

### 1. Check the Vagrant configuration file
   - [Vagrantfile](Vagrantfile)

### 2. Run Virtual Machine with Ubuntu Server 22.04
   - `vagrant init bento/ubuntu-22.04`
   - `vagrant up`

### 3. Check the Ansible playbook
   - [playbook.yaml](files/playbook.yaml)

### 4. Main project files
   - [Script to run playbook](run_ansible.sh)
   - [JavaScript Application](files/hello.js)
   - [Nginx Web Server Configuration](files/nginx.conf)