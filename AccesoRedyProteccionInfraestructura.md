# Acceso a la Red y Protección de la Infraestructura 🚦🔒

Este resumen une los contenidos clave del **Módulo 2: Acceso a la Red y Protección de la Infraestructura** con ejemplos prácticos y preguntas tipo test resueltas. Ideal para estudiantes, profesionales o apasionados de la **ciberseguridad en el sector transporte**.

---

## 1. Acceso a la Red

### Ethernet y Conmutación

* **Ethernet**: estándar de red más usado en LAN. Transmite datos en forma de paquetes y usa direcciones **MAC** para identificar dispositivos.
* **Switching**: el switch envía los datos **solo al dispositivo correcto**, evitando colisiones y mejorando la eficiencia.

👉 Ejemplo: en una terminal de tren, un switch envía el vídeo de una cámara directamente al servidor, sin saturar al resto de dispositivos.

### Protocolo Spanning Tree (STP)

* Previene **bucles de red** en switches.
* Desactiva enlaces redundantes y, si el principal falla, activa otro automáticamente.
* Garantiza **disponibilidad y estabilidad**.

👉 Ejemplo: en una red ferroviaria, STP asegura que las cámaras de seguridad tengan siempre un camino operativo hacia el centro de control.

### VLANs

* Segmentan una red física en varias **redes lógicas**.
* Mejoran la **seguridad** (cada VLAN es independiente) y la gestión del tráfico.

👉 Ejemplo: separar la VLAN de **administración**, la de **logística** y la de **Wi-Fi para pasajeros** en un aeropuerto.

### Trunking

* Permite que varias VLANs viajen por un único enlace físico.
* Usa **IEEE 802.1Q** para etiquetar el tráfico.

👉 Ejemplo visual:

![Trunking VLANs](trunking.png)

*(Enlace trunk entre dos switches transportando VLANs de logística, administración y pasajeros)*

### Seguridad de Puerto

* Restringe qué dispositivos pueden conectarse a un puerto del switch.
* Se basa en direcciones **MAC autorizadas**.

👉 Ejemplo: solo las cámaras autorizadas pueden conectarse a los puertos del switch en un sistema de videovigilancia.

### Redes Inalámbricas (Wi-Fi)

* Usan ondas de radio para conectar dispositivos.
* Protocolos de seguridad como **WPA2/WPA3** protegen las comunicaciones.

👉 Ejemplo: tablets del personal de una estación acceden de forma segura con WPA3.

---

## 2. Protección de la Infraestructura y la Información

### Seguridad de la Infraestructura en Transporte

* Las redes de transporte (ferrocarriles, aeropuertos, puertos) son **infraestructuras críticas**.
* Medidas: controles físicos (vigilancia, acceso restringido) y cibernéticos (firewalls, segmentación).

### Sistemas SCADA

* Supervisan y controlan operaciones críticas en tiempo real (tráfico, trenes, logística).
* Deben estar aislados y protegidos contra accesos no autorizados.

### Redundancia y Resiliencia

* Redes críticas necesitan **conexiones de respaldo** para seguir funcionando ante fallos o ataques.

### Seguridad de la Información

* **CIA Triad**: Confidencialidad, Integridad y Disponibilidad.
* Medidas: cifrado, autenticación multifactor, monitorización continua.
* Amenazas: ransomware, phishing, DDoS.

### Control de Accesos

* **Físicos**: tarjetas, biometría, cámaras.
* **Lógicos**: MFA, contraseñas robustas, segmentación.

### Tecnologías Clave

* **Firewalls**: filtran tráfico según reglas.
* **VPNs**: crean túneles cifrados para accesos remotos.
* **Segmentación de Red**: divide la red en subredes aisladas.

👉 Ejemplo visual de **NAT** (Network Address Translation):

![NAT](nat.png)

*(Varios dispositivos privados comparten una única IP pública mediante un router con NAT)*

---

## 3. Preguntas Clave Resueltas ✅

* **Segmentación de red**: limita el acceso entre partes de la red → mejora la seguridad.
* **STP**: evita bucles en switches.
* **Firewall**: dispositivo que filtra el tráfico según reglas.
* **Control de acceso físico**: videovigilancia, cerraduras electrónicas, biometría.
* **Port Security**: asegura que solo dispositivos autorizados usen un puerto.
* **VPN**: acceso seguro a sistemas centrales desde ubicaciones remotas.
* **VLAN**: aislar redes lógicas dentro de una misma infraestructura física.
* **Switch**: conecta dispositivos en una LAN y gestiona tráfico por direcciones MAC.
* **SCADA**: monitoreo y control de operaciones críticas.
* **NAT**: varios dispositivos comparten una única IP pública.

---

## 4. Conclusión

El **sector transporte** depende de redes robustas y seguras. Tecnologías como **Ethernet, STP, VLANs, Trunking, Firewalls, VPNs, Segmentación, SCADA y Port Security** son la columna vertebral que garantiza:

* Operaciones seguras y eficientes.
* Protección de infraestructuras críticas.
* Defensa contra ciberamenazas.

En definitiva: **la ciberseguridad no es opcional, es vital** para la continuidad y la seguridad en el transporte moderno.

---

