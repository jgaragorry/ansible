# Ejercicio 2: Creación de Usuarios y Grupos

Este ejercicio muestra cómo crear usuarios y grupos en sistemas Linux usando Ansible.

## Pasos para ejecutar el playbook
1. Asegúrate de tener un archivo de inventario con los servidores.
2. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Crear grupo 'developers'**: Usa el módulo `group` para crear un grupo llamado `developers`.
- **Crear usuario 'john'**: Usa el módulo `user` para crear un usuario llamado `john` y asignarlo al grupo `developers`.