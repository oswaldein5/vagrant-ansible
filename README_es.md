## Instalar Nginx | Nodejs | Pm2 | App.js usando Ansible

Generar una imagen local mediante **Vagrant** utilizando **Ansible** para la instalación y configuración de Ubuntu, Nodejs y Nginx como Servidor Web; Garantizar el inicio automático de la aplicacion (hello.js) cuando arranca o se reinicia el Servidor Web.

Útil para crear imágenes de máquinas virtuales preconfiguradas para entornos locales o proveedores de Cloud.

---
### 1. Playbook de Ansible
   - [playbook.yaml](files/playbook.yaml)

### 2. Archivos del projecto
   - [Script para ejecutar playbook](run_ansible.sh)
   - [Aplicación JavaScript](files/hello.js)
   - [Configuración Servidor Web Nginx](files/nginx.conf)
  
### 3. Archivo de configuración de Vagrant
   - [Vagrantfile](Vagrantfile)

### 4. Iniciar Maquina Virtual con Ubuntu Server 22.04
```sh
vagrant init bento/ubuntu-22.04
vagrant up
http://localhost
```
