## Instalar Nginx | Nodejs | Pm2 | App.js usando Ansible

Generar una imagen con una aplicación con Nodejs ya instalada y configurada con Nginx como Servidor Web; Garantizar el inicio automático de la aplicacion (hello.js) cuando arranca o se reinicia el Servidor Web.

Útil para crear imágenes de máquinas virtuales preconfiguradas para entornos locales o proveedores de Cloud.

---

### 1. Revisar archivo de configuración de Vagrant
   - [Vagrantfile](Vagrantfile)

### 2. Iniciar Maquina Virtual con Ubuntu Server 22.04
   - `vagrant init bento/ubuntu-22.04`
   - `vagrant up`

### 3. Revisar playbook de Ansible
   - [playbook.yaml](files/playbook.yaml)

### 4. Archivos principales del projecto
   - [Script para ejecutar playbook](run_ansible.sh)
   - [Aplicación JavaScript](files/hello.js)
   - [Configuración Servidor Web Nginx](files/nginx.conf)
