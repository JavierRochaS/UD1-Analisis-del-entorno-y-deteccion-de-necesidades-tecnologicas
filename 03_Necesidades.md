# 3. Identificación de necesidades tecnológicas

Tras la auditoría inicial en *Logística del Guadalquivir S.L.*, se detectan carencias críticas que comprometen la seguridad y la continuidad del negocio.

## Tabla de Análisis de Carencias y Soluciones

| Área | Situación Actual (Problema) | Solución Propuesta (Proyecto ASIR) |
| :--- | :--- | :--- |
| **Seguridad de Datos** | Copias de seguridad manuales en discos USB externos. Riesgo alto de pérdida por fallo humano, robo o *Ransomware*. | **Sistema de Backups 3-2-1:** Servidor NAS local para copias rápidas + Replicación automatizada y cifrada en la Nube. |
| **Gestión de Usuarios** | Uso de cuentas locales en cada PC. Contraseñas débiles y compartidas. Acceso indiscriminado a carpetas sensibles. | **Directorio Activo (Dominio):** Centralización de usuarios, grupos y políticas de seguridad (GPO) para controlar el acceso. |
| **Redes y Comunicaciones** | Red plana (192.168.1.x) compartida por PCs de facturación, móviles de invitados y cámaras. Saturación y riesgo de intrusiones. | **Segmentación VLAN:** Separación lógica de redes (VLAN Gestión, VLAN Almacén, VLAN Invitados) mediante Switch gestionable. |
| **Alta Disponibilidad** | El software de facturación reside en un PC antiguo. Si el disco falla, la empresa detiene su actividad. | **Virtualización:** Implementación de un hipervisor (Proxmox/Hyper-V) para facilitar la recuperación y snapshots. |

## Justificación del Proyecto
La prioridad absoluta es la **integridad y confidencialidad** de los datos. La empresa maneja datos de clientes protegidos por el RGPD; su pérdida o filtración acarrearía sanciones graves.
