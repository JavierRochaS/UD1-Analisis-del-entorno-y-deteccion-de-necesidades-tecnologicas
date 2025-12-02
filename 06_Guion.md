# 6. Guion inicial del proyecto

Planificación de fases para la ejecución del proyecto:

### FASE 1: Análisis y Diseño (Semanas 1-2)
*  Auditoría de los equipos y red actual.
*  Diseño del esquema de direccionamiento IP (Subredes).
*  Selección de características del Servidor.

### FASE 2: Infraestructura Base (Semanas 3-4)
*  Instalación del Hipervisor y despliegue de Máquinas Virtuales.
*  Configuración de almacenamiento (RAID software).
*  Configuración de red estática en servidores.

### FASE 3: Servicios de Red y Directorio (Semanas 5-6)
*  Creación del Dominio y Usuarios (Directorio Activo).
*  **Implementación de DHCP Failover (Balanceo de carga).**
*  Pruebas de continuidad: Verificar asignación de IP tras caída de un nodo.

### FASE 4: Servicios Web y Datos (Semanas 7-8)
*  **Instalación del Stack LAMP (Linux, Apache, MariaDB, PHP).**
*  **Despliegue y configuración de Nextcloud.**
*  Configuración de cuotas de disco y permisos de usuario.

### FASE 5: Seguridad y Monitorización (Semanas 9-10)
*  **Configuración de reglas de Firewall (Iptables/Windows Firewall).**
*  Despliegue de Grafana para monitorizar el estado del sistema.
*  Programación de scripts de Copias de Seguridad.

### FASE 6: Cierre (Semana 11)
*  **Simulacro de recuperación de archivos (Restore).**
*  Documentación técnica y manuales de entrega.
