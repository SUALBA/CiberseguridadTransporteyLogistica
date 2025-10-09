# 🌐 Ejercicio Módulo 4 – DHCP, DNS, NAT y PAT  
**Ciberseguridad en redes y sistemas de Transporte y Logística: Fundamentos y aplicaciones prácticas**

Este ejercicio une teoría y práctica: configuramos **DHCP, DNS, NAT y PAT** en una red simulada.  
El objetivo es entender cómo funcionan estos servicios y cómo se aplican en un entorno real de transporte/logística.

---

## 1️⃣ DHCP – Asignación dinámica de IPs  

### 🔹 Escenario
Tienes una red en casa con:
- 💻 Laptop  
- 📱 Smartphone  
- 🎮 Consola de videojuegos  

### 🔹 Configuración en el router
```bash
ip dhcp pool CASA
 network 192.168.1.0 255.255.255.0
 default-router 192.168.1.1
 dns-server 192.168.1.1
 lease 7



👉 El router asignará automáticamente IPs a los dispositivos:

Laptop → 192.168.1.2

Smartphone → 192.168.1.3

Consola → 192.168.1.4

🔹 Fundamento técnico

DHCP → Dynamic Host Configuration Protocol.

Funciona en capa 7 (Aplicación).

Usa UDP (puertos 67 servidor, 68 cliente).

Proceso DORA (Discover, Offer, Request, Acknowledge).

Cliente ---Discover---> Servidor
Servidor ---Offer------> Cliente
Cliente ---Request----> Servidor
Servidor ---Acknowledge> Cliente


2️⃣ DNS – Traducción de nombres en IPs
🔹 Escenario

Queremos que al escribir http://miportal
 el navegador abra la laptop (192.168.1.5).

🔹 Configuración
ip host miportal 192.168.1.5



👉 Flujo:

Usuario escribe: http://miportal

Servidor DNS responde: 192.168.1.5

Navegador conecta a la laptop.

🔹 Fundamento técnico

DNS → Domain Name System.

Funciona en capa 7 (Aplicación).

Usa UDP/53 (consultas rápidas) y TCP/53 (transferencias de zona).

Usuario → "miportal"
DNS → "192.168.1.5"
Navegador → Conecta al servidor web en laptop



⚠️ Riesgo: DNS Spoofing / Cache Poisoning.
✅ Defensa: DNSSEC + monitorización.

3️⃣ NAT – Network Address Translation
🔹 Escenario

Eres admin de red de una pequeña empresa con 3 PCs:

PC1 → 192.168.1.2

PC2 → 192.168.1.3

PC3 → 192.168.1.4

👉 La empresa solo tiene 1 IP pública: 203.0.113.1.

🔹 Configuración
ip nat inside source list 1 interface FastEthernet0/0 overload
access-list 1 permit 192.168.1.0 0.0.0.255



👉 El router traduce:

Interno (192.168.1.x) → Externo (203.0.113.1)

🔹 Diagrama
[192.168.1.2] \
[192.168.1.3] ---> [Router NAT] ---> [203.0.113.1] ---> Internet
[192.168.1.4] /

🔹 Fundamento técnico

NAT permite que varios dispositivos compartan una sola IP pública.

Funciona en capa 3 (Red).

Tipos:

Static NAT → 1:1

Dynamic NAT → rango de IPs

NAT Overload (PAT) → una IP pública + puertos

⚠️ Limitación: NAT no es una medida de seguridad completa.
✅ Siempre reforzar con firewalls e IDS/IPS.

4️⃣ PAT – Port Address Translation
🔹 Escenario

El router asigna un puerto único a cada dispositivo:

PC1 (192.168.1.2) → 203.0.113.1:10001

PC2 (192.168.1.3) → 203.0.113.1:10002

PC3 (192.168.1.4) → 203.0.113.1:10003

👉 Ejemplo de tráfico:

PC1 pide una web → 192.168.1.2 → 203.0.113.1:10001

El servidor responde → 203.0.113.1:10001 → router → PC1

🔹 Diagrama
Interno                        NAT/PAT Router               Internet
---------                      -----------------            ---------
192.168.1.2:1025   --->        203.0.113.1:10001   --->     Servidor web
192.168.1.3:1040   --->        203.0.113.1:10002   --->     Juego online
192.168.1.4:1100   --->        203.0.113.1:10003   --->     Streaming

🔹 Fundamento técnico

PAT = NAT + puertos.

Permite que decenas o cientos de dispositivos compartan una sola IP pública.

El router mantiene una tabla de mapeos IP:puerto ↔ dispositivo interno.

⚔️ Ataques y Defensas

DHCP

Ataques: DHCP Starvation, Rogue DHCP.

Defensas: DHCP Snooping, rangos limitados, reservas.

DNS

Ataques: DNS Spoofing, Cache Poisoning, DNS Tunneling.

Defensas: DNSSEC, filtrado de dominios, monitorización.

NAT/PAT

Ataques: NAT Traversal, Port Scanning, Session Hijacking.

Defensas: Firewalls NGFW, IDS/IPS, segmentación de red, VPN/IPsec.

📚 Conclusión

DHCP: asigna IPs dinámicas de forma automática.

DNS: traduce nombres ↔ IPs, esencial para la navegación.

NAT: permite que varias IP privadas compartan una IP pública.

PAT: añade puertos para diferenciar conexiones simultáneas.

🔑 En ciberseguridad → todos deben configurarse con controles y defensas adicionales.

✅ Gracias a estos servicios, una red doméstica o empresarial puede funcionar con eficiencia, escalabilidad y seguridad.
