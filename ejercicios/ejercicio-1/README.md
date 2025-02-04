# Ejercicio 1: Instalación de Apache

Este ejercicio muestra cómo instalar y configurar Apache en un servidor remoto usando Ansible.

## Pasos para ejecutar el playbook
1. Asegúrate de tener un archivo de inventario con los servidores bajo el grupo `webservers`.
2. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Instalar Apache**: Usa el módulo `apt` para instalar el paquete `apache2`.
- **Habilitar e iniciar Apache**: Usa el módulo `service` para asegurar que Apache esté activo y en ejecución.