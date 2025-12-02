# 3. Identificación de necesidades tecnológicas

Tras la auditoría inicial en *Logística del Guadalquivir S.L.*, se detectan carencias críticas que comprometen la seguridad y la continuidad del negocio.

## Tabla de Análisis de Carencias y Soluciones

| Área | Situación Actual (Problema) | Solución Propuesta (Proyecto ASIR) |
| :--- | :--- | :--- |
| **Seguridad de Datos** | Copias de seguridad manuales en discos USB externos. Riesgo crítico de pérdida de datos por fallo humano o *Ransomware*. | **Sistema de Backups 3-2-1:** Servidor NAS local para copias rápidas + Replicación automatizada y cifrada en la Nube. |
| **Gestión de Usuarios** | Uso de cuentas locales en cada PC. Contraseñas débiles y compartidas. Acceso indiscriminado a carpetas sensibles. | **Directorio Activo (Dominio):** Centralización de usuarios, grupos y políticas de seguridad (GPO) para controlar el acceso. |
| **Redes** | Red plana (192.168.1.x) saturada y sin seguridad. El Wi-Fi de invitados da acceso a los servidores de la empresa. | **Segmentación VLAN:** Separación lógica de redes (VLAN Gestión, VLAN Almacén, VLAN Invitados) mediante Switch gestionable. (En virtualbox simulariamos con diferentes redes internas) |
| **Monitorización** | **Mantenimiento Reactivo:** No se sabe si un servidor ha caído o si el disco está lleno hasta que el usuario se queja. | **Monitorización Proactiva (Grafana):** Dashboard en tiempo real para visualizar estado de CPU, Discos y Red antes de que fallen. |
| **Alta Disponibilidad** | El software de facturación reside en un PC antiguo. Si el hardware falla, la empresa para. | **Virtualización:** Implementación de un hipervisor (Proxmox/Hyper-V) para facilitar la recuperación y snapshots. |

## Justificación del Proyecto
La prioridad es pasar de un modelo de "reparación de averías" a uno de **gestión profesional de sistemas**. La implementación de Grafana permitirá al departamento técnico anticiparse a los problemas, mientras que el Directorio Activo asegurará la confidencialidad exigida por el RGPD.
