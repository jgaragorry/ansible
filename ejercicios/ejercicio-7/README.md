# Ejercicio 7: Gestión de Servicios con Ansible

Este ejercicio muestra cómo gestionar servicios en sistemas Linux.

## Pasos para ejecutar el playbook
1. Asegúrate de tener un archivo de inventario con los servidores.
2. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Detener Apache**: Usa el módulo `service` para detener Apache.
- **Habilitar SSH**: Usa el módulo `service` para habilitar y iniciar SSH.