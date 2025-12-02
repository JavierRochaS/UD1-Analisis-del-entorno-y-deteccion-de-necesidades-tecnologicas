# 3. Identificación de necesidades tecnológicas

Tras la auditoría inicial, se detectan carencias críticas que se resolverán mediante una infraestructura integral ASIR optimizada.

## Tabla de Análisis de Carencias y Soluciones

| Área | Situación Actual (Problema) | Solución Propuesta (Proyecto ASIR) |
| :--- | :--- | :--- |
| **Continuidad de Red** | Un solo router entrega IPs. Si falla, la empresa se queda sin conexión. | **DHCP Failover:** Implementación de dos servidores DHCP balanceados para asegurar que siempre haya asignación de IPs. |
| **Colaboración y Web** | Descontrol de versiones de archivos y uso inseguro de USBs. | **Nube Privada (Nextcloud):** Sistema centralizado en servidor propio para compartir documentación de forma segura. |
| **Seguridad de Datos** | Copias manuales en discos externos. Riesgo de pérdida por fallo físico. | **Sistema de Backups 3-2-1:** Copias automatizadas en disco local y replicación cifrada a la nube. |
| **Gestión de Usuarios** | Cuentas locales y contraseñas compartidas ("1234"). | **Directorio Activo:** Gestión centralizada de usuarios, grupos y permisos de acceso. |
| **Monitorización** | Mantenimiento reactivo (se actúa cuando algo se rompe). | **Monitorización Proactiva (Grafana):** Panel de control para vigilar el estado de los servidores (disco, RAM, red). |
| **Seguridad de Red** | Red plana e insegura. El router de la operadora no filtra nada. | **Firewall Perimetral:** Configuración de un cortafuegos (iptables/nftables o pfsense) para filtrar el tráfico no deseado. |

## Justificación Académica
El proyecto maximiza el uso de los recursos existentes (sin compra de electrónica de red) y centra la solución en la **configuración avanzada de sistemas**: Redundancia de servicios (DHCP), Seguridad lógica (Firewall/Permisos) y Sistemas de información (Web/Datos).
