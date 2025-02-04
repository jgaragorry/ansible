# Comandos Comunes en Ansible

## Comandos Básicos
- **`ansible --version`**: Muestra la versión de Ansible instalada.
- **`ansible all --ping`**: Verifica la conectividad con todos los nodos gestionados.
- **`ansible-playbook playbook.yml`**: Ejecuta un playbook.

## Comandos de Inventario
- **`ansible-inventory --list`**: Muestra el inventario en formato JSON.
- **`ansible-inventory --graph`**: Muestra el inventario en formato gráfico.

## Comandos de Módulos
- **`ansible webservers -m apt -a "name=apache2 state=present"`**: Instala Apache en los servidores del grupo `webservers`.
- **`ansible dbservers -m service -a "name=mysql state=started"`**: Inicia el servicio MySQL en los servidores del grupo `dbservers`.