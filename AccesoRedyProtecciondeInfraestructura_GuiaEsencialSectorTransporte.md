# Acceso a la Red y Protección de Infraestructura 🚦🔒

**Guía esencial para el sector transporte**

Este documento reúne de manera ampliada los contenidos clave del **Módulo 2: Acceso a la Red y Protección de la Infraestructura**, junto con explicaciones claras, ejemplos prácticos y preguntas resueltas. Está pensado como un artículo premium para lectores que buscan aprender y profundizar en la **ciberseguridad aplicada al transporte**.

---

## 1. Acceso a la Red

### Ethernet y Conmutación

* **Ethernet** es el estándar de red más utilizado en LANs. Identifica dispositivos por direcciones **MAC** y transmite datos en tramas.
* **Switching**: el switch dirige los datos solo al dispositivo de destino, mejorando el rendimiento y evitando colisiones.

👉 Ejemplo: en una terminal de tren, un switch asegura que los datos de la cámara de seguridad lleguen únicamente al servidor de grabación.

### Protocolo Spanning Tree (STP)

* Detecta y previene **bucles de red**.
* Bloquea enlaces redundantes hasta que se necesiten.
* Asegura **alta disponibilidad** en la red.

👉 Ejemplo: en la red de un aeropuerto, STP mantiene activa una ruta de respaldo en caso de fallo.

### VLANs

* Segmentan la red física en varias **redes lógicas independientes**.
* Mejoran la **seguridad** y la **eficiencia**.

👉 Ejemplo: separar la VLAN de **administración**, la de **operaciones logísticas** y la de **pasajeros Wi-Fi**.

### Trunking

* Permite que varias VLANs viajen por un único enlace físico.
* Usa **IEEE 802.1Q** para etiquetar las tramas.

👉 Ejemplo visual:

![Trunking VLANs](trunking.png)

### Seguridad de Puerto

* Limita qué dispositivos pueden conectarse a un puerto de switch.
* Funciona con direcciones **MAC autorizadas**.

👉 Ejemplo: solo se permiten cámaras homologadas en los puertos de un switch de videovigilancia.

### Redes Inalámbricas (Wi-Fi)

* Usan protocolos de cifrado como **WPA2/WPA3**.
* Deben estar configuradas con autenticación robusta.

👉 Ejemplo: el personal accede al sistema con tablets mediante Wi-Fi protegido por WPA3.

---

## 2. Protección de la Infraestructura y la Información

### Seguridad de la Infraestructura en Transporte

* Los sistemas de transporte (ferrocarriles, aeropuertos, puertos) son **infraestructuras críticas**.
* Se protegen con medidas físicas (accesos restringidos, cámaras) y digitales (segmentación, firewalls, redundancia).

### Sistemas SCADA

* Monitorizan y controlan operaciones en tiempo real.
* Deben estar aislados de redes abiertas y protegidos con controles estrictos.

### Redundancia y Resiliencia

* La red debe garantizar continuidad de servicio.
* Se implementan enlaces de respaldo y configuraciones de failover.

### Seguridad de la Información (CIA Triad)

* **Confidencialidad**: solo usuarios autorizados acceden.
* **Integridad**: los datos no se alteran sin permiso.
* **Disponibilidad**: los sistemas funcionan cuando se necesitan.

👉 Ejemplo visual sugerido: un triángulo representando el CIA.

### Control de Acceso

* **Físico**: biometría, tarjetas de proximidad, cámaras.
* **Lógico**: contraseñas robustas, MFA, segmentación, políticas de privilegios mínimos.

### Firewalls

* Filtran tráfico de red según reglas.
* Bloquean accesos no autorizados.

### VPNs

* Crean un túnel cifrado entre usuario y red corporativa.
* Permiten acceso remoto seguro.

### NAT

* Traduce direcciones privadas a una dirección pública.
* Permite compartir internet sin exponer la red interna.

👉 Ejemplo visual:

![NAT](nat.png)

---

## 3. Gestión de Identidades y Accesos (IAM)

* Define **quién accede a qué recursos y cómo**.
* Incluye:

  * **Autenticación multifactor (MFA)**.
  * **Roles y privilegios** (principio de mínimo privilegio).
  * **Registro y auditoría de accesos**.
* Mejora la seguridad y facilita el cumplimiento normativo.

👉 Ejemplo: un maquinista solo accede al panel de rutas, mientras que un administrador puede gestionar toda la red.

---

## 4. Tecnologías Emergentes en Transporte

* **IDS/IPS**: detectan y previenen intrusiones en la red.
* **Zero Trust**: nadie es confiable por defecto, cada acceso debe validarse.
* **Blockchain**: trazabilidad de la cadena logística.
* **Inteligencia Artificial**: detección de anomalías en tráfico de red.

---

## 5. Normativa y Cumplimiento

* **RGPD** y **LOPDGDD**: protegen los datos personales de pasajeros.
* **ISO 27001**: estándar internacional de gestión de seguridad.
* **NIS2**: directiva europea para infraestructuras críticas.

👉 Cumplir con estas normas aumenta la confianza y reduce riesgos legales.

---

## 6. Casos Prácticos en Transporte

* **Aeropuertos**: VLANs separan sistemas de control aéreo, administración y Wi-Fi de pasajeros.
* **Ferrocarriles**: SCADA gestiona señales y cambios de vía en tiempo real.
* **Logística marítima**: blockchain y VPNs aseguran datos de contenedores y rutas.

---

## 7. Glosario Clave

* **VLAN**: red lógica independiente dentro de una infraestructura física.
* **Trunking**: transportar varias VLANs por un solo enlace físico.
* **STP**: protocolo que evita bucles de red.
* **Firewall**: dispositivo que filtra tráfico según reglas.
* **VPN**: túnel cifrado para acceso remoto seguro.
* **NAT**: traducción de IP privadas a públicas.
* **SCADA**: sistema de supervisión y control en tiempo real.
* **IAM**: gestión de identidades y accesos.

---

## 8. Conclusión

El **sector transporte** requiere redes seguras, resilientes y protegidas frente a ciberamenazas. Tecnologías como **VLANs, STP, Trunking, Firewalls, VPNs, IAM, SCADA, IDS/IPS** y marcos normativos como **ISO 27001 y NIS2** son fundamentales para garantizar la continuidad y la seguridad.

En definitiva: **la ciberseguridad no es opcional en transporte, es un pilar estratégico.** 🚀

---

