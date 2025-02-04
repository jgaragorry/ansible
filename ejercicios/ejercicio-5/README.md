# Ejercicio 5: Automatización de Copias de Seguridad

Este ejercicio muestra cómo automatizar la creación de copias de seguridad.

## Pasos para ejecutar el playbook
1. Asegúrate de tener MySQL instalado y una base de datos llamada `database`.
2. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Crear directorio de backups**: Usa el módulo `file` para crear un directorio.
- **Crear backup de la base de datos**: Usa el módulo `command` para ejecutar `mysqldump`.