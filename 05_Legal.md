# 5. Obligaciones legales y normativas

El diseño del proyecto se basa en el principio de "Privacidad por Diseño" para garantizar el cumplimiento normativo:

## 1. Protección de Datos (RGPD y LOPDGDD)
La implementación de una **Nube Privada (Nextcloud)** alojada localmente ofrece ventajas legales críticas frente a nubes públicas:
* **Soberanía del Dato:** Los datos de los clientes nunca salen de los servidores de la empresa, eliminando riesgos de transferencias internacionales no autorizadas.
* **Control de Acceso (Art. 32):** Se implementará autenticación centralizada. Cada empleado tendrá su propio usuario/contraseña para acceder a los archivos, acabando con las "cuentas compartidas".
* **Derechos ARCO:** La centralización de datos facilita la localización rápida de información para responder a solicitudes de acceso, rectificación o supresión por parte de los clientes.

## 2. Propiedad Intelectual y Licencias
Para garantizar la viabilidad legal y reducir costes operativos:
* **Política de Software Libre:** Se prioriza el uso de software con licencias **GPL, MIT o Apache** (Linux, MariaDB, Grafana), lo que permite su uso comercial gratuito y legal sin necesidad de pagar licencias propietarias (CALs).
* **Inventario:** Se realizará una auditoría inicial para detectar y eliminar cualquier software "pirata" existente en los equipos antiguos.

## 3. LSSI-CE (Comercio Electrónico)
* **Seguridad Web:** El acceso a la Intranet/Nextcloud estará protegido mediante **HTTPS/TLS** con certificados (Self-signed o Let's Encrypt) para cifrar las comunicaciones internas.

## 4. Prevención de Riesgos Laborales (PRL)
El entorno de trabajo del administrador de sistemas cumplirá con:
* **Seguridad Física:** Organización del cableado en el rack para evitar caídas y asegurar la ventilación de los equipos (prevención de incendios).
* **Ergonomía:** Ajuste de monitores y periféricos en el puesto de control para prevenir fatiga visual y trastornos musculoesqueléticos.
