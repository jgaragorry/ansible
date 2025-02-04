# Comandos Comunes en Ansible

Este archivo contiene una lista de los comandos más usados en Ansible, explicando qué hace cada uno. Estos comandos son útiles para la automatización de tareas de configuración y despliegue.

---

## Comandos Básicos

- **`ansible --version`**: Muestra la versión de Ansible instalada en el sistema.  
- **`ansible all --ping`**: Verifica la conectividad con todos los nodos gestionados.  
- **`ansible-playbook playbook.yml`**: Ejecuta un playbook de Ansible.  

---

## Comandos de Inventario

- **`ansible-inventory --list`**: Muestra el inventario en formato JSON.  
- **`ansible-inventory --graph`**: Muestra el inventario en formato gráfico.  

---

## Comandos de Módulos

- **`ansible webservers -m apt -a "name=apache2 state=present"`**: Instala Apache en los servidores del grupo `webservers`.  
- **`ansible dbservers -m service -a "name=mysql state=started"`**: Inicia el servicio MySQL en los servidores del grupo `dbservers`.  
- **`ansible all -m copy -a "src=files/app.conf dest=/etc/app.conf"`**: Copia un archivo desde el nodo de control a los nodos gestionados.  
- **`ansible all -m file -a "path=/backups state=directory mode=0755"`**: Crea un directorio en los nodos gestionados.  
- **`ansible all -m command -a "mysqldump -u root -pPassword123 database > /backups/db_backup.sql"`**: Ejecuta un comando directamente en los nodos gestionados.  

---

## Comandos de Roles

- **`ansible-galaxy init nombre_del_rol`**: Crea la estructura básica de un rol en Ansible.  

---

## Comandos de Plantillas

- **`ansible all -m template -a "src=templates/app.conf.j2 dest=/etc/app.conf"`**: Genera un archivo de configuración dinámico usando una plantilla Jinja2.  

---

## Comandos de Usuarios y Grupos

- **`ansible all -m user -a "name=john group=developers password={{ 'password123' | password_hash('sha512') }}"`**: Crea un usuario en los nodos gestionados.  
- **`ansible all -m group -a "name=developers state=present"`**: Crea un grupo en los nodos gestionados.  

---

## Comandos de Git

- **`ansible all -m git -a "repo=https://github.com/ejemplo/app-web.git dest=/var/www/app version=main"`**: Clona un repositorio Git en los nodos gestionados.  

---

## Comandos de Servicios

- **`ansible all -m service -a "name=nginx state=restarted"`**: Reinicia un servicio en los nodos gestionados.  
- **`ansible all -m service -a "name=apache2 state=stopped"`**: Detiene un servicio en los nodos gestionados.  

---

## Comandos de Variables

- **`ansible-playbook playbook.yml --extra-vars "app_name=MiApp app_port=8080"`**: Pasa variables adicionales a un playbook.  

---

## Comandos de Verificación

- **`ansible-playbook playbook.yml --check`**: Realiza una simulación ("dry run") para ver qué cambios se aplicarían sin ejecutarlos realmente.  

---

## Comandos de Depuración

- **`ansible-playbook playbook.yml -vvv`**: Ejecuta un playbook con un nivel de verbosidad alto para depuración.  

---

Este archivo es una referencia rápida para los comandos más usados en Ansible. ¡Espero que te sea útil! 😊