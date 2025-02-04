# Ejercicio 4: Uso de Roles en Ansible

Este ejercicio muestra cómo usar roles para organizar tareas en Ansible.

## Pasos para ejecutar el playbook
1. Crea la estructura de roles: `ansible-galaxy init common` y `ansible-galaxy init webserver`.
2. Define las tareas en los roles dentro de `roles/common/tasks/main.yml` y `roles/webserver/tasks/main.yml`.
3. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Roles**: Usa roles para modularizar y reutilizar tareas.