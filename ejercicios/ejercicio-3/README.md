# Ejercicio 3: Despliegue de una Aplicación Web

Este ejercicio muestra cómo desplegar una aplicación web usando Git y configurar un archivo de configuración.

## Pasos para ejecutar el playbook
1. Asegúrate de tener un archivo de inventario con los servidores bajo el grupo `webservers`.
2. Crea la carpeta `files/` y añade el archivo `app.conf`.
3. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Instalar Git**: Usa el módulo `apt` para instalar Git.
- **Clonar repositorio**: Usa el módulo `git` para clonar un repositorio de aplicación web.
- **Copiar archivo de configuración**: Usa el módulo `copy` para mover un archivo de configuración.