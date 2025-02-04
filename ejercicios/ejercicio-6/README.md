# Ejercicio 6: Configuración de un Balanceador de Carga

Este ejercicio muestra cómo configurar Nginx como balanceador de carga.

## Pasos para ejecutar el playbook
1. Asegúrate de tener un archivo de inventario con el servidor bajo el grupo `loadbalancer`.
2. Crea la carpeta `files/` y añade el archivo `nginx.conf`.
3. Ejecuta el playbook: `ansible-playbook playbook.yml`.

## Explicación del Playbook
- **Instalar Nginx**: Usa el módulo `apt` para instalar Nginx.
- **Configurar Nginx**: Usa el módulo `copy` para mover la configuración.
- **Reiniciar Nginx**: Usa el módulo `service` para reiniciar el servicio.