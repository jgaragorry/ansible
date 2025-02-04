# Ejercicio 8: Uso de Variables y Plantillas

Este ejercicio muestra cómo usar variables y plantillas en Ansible.

## Pasos para ejecutar el playbook
1. Crea la carpeta `templates/` y añade el archivo `app.conf.j2`.
2. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Variables**: Define variables como `app_name` y `app_port`.
- **Plantillas**: Usa el módulo `template` para generar archivos de configuración dinámicos.