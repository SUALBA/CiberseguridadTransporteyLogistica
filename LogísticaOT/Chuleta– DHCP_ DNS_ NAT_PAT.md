# 🌐 Chuleta Express – DHCP, DNS, NAT y PAT
**Ciberseguridad en Redes y Sistemas de Transporte y Logística (Módulo 4)**

---

## 1️⃣ DHCP – Dynamic Host Configuration Protocol
📍 **Función:** Asigna IPs automáticamente a los dispositivos de la red.  

### 🔄 Flujo DORA
```ascii
Cliente ---Discover---> Servidor
Servidor ---Offer------> Cliente
Cliente ---Request----> Servidor
Servidor ---Acknowledge> Cliente
🔌 Puertos: UDP 67 (servidor), UDP 68 (cliente)

🖥️ Ejemplo: Laptop → 192.168.1.2 | Smartphone → 192.168.1.3

⚔️ Ataques: DHCP Starvation, Rogue DHCP
🛡️ Defensas: DHCP Snooping, reservas, monitoreo

2️⃣ DNS – Domain Name System
📍 Función: Traduce nombres de dominio ↔ direcciones IP.

🔄 Flujo
ascii
Copiar código
Usuario → "miportal"
DNS     → "192.168.1.5"
Navegador → Conecta a la laptop
🔌 Puertos: UDP 53 (consultas), TCP 53 (zonas)

🖥️ Ejemplo: "miportal" → 192.168.1.5

⚔️ Ataques: Spoofing, Cache Poisoning, DNS Tunneling
🛡️ Defensas: DNSSEC, listas negras, monitorización

3️⃣ NAT – Network Address Translation
📍 Función: Traduce IPs privadas ↔ IP pública (Capa 3).

🔄 Ejemplo
ascii
Copiar código
PC1: 192.168.1.2 → 203.0.113.1
PC2: 192.168.1.3 → 203.0.113.1
PC3: 192.168.1.4 → 203.0.113.1

[192.168.1.2] \
[192.168.1.3] ---> [Router NAT] ---> [203.0.113.1] ---> Internet
[192.168.1.4] /
⚔️ Ataques: NAT Traversal, IP Spoofing
🛡️ Defensas: Firewalls NGFW, ACLs, segmentación de red

4️⃣ PAT – Port Address Translation
📍 Función: NAT con puertos → varios dispositivos, 1 IP pública.

🔄 Ejemplo
ascii
Copiar código
PC1 (192.168.1.2) → 203.0.113.1:10001
PC2 (192.168.1.3) → 203.0.113.1:10002
PC3 (192.168.1.4) → 203.0.113.1:10003

192.168.1.2:1025 ---> 203.0.113.1:10001 ---> Internet
192.168.1.3:1040 ---> 203.0.113.1:10002 ---> Internet
192.168.1.4:1100 ---> 203.0.113.1:10003 ---> Internet
⚔️ Ataques: Port Scanning, Session Hijacking
🛡️ Defensas: IDS/IPS, registro de conexiones, VPN/IPsec

📊 Resumen Comparativo
Servicio	Función	Puerto(s)	Ataques	Defensas
DHCP	Asignar IPs dinámicas	UDP 67/68	Starvation, Rogue DHCP	Snooping, reservas
DNS	Traducir nombre ↔ IP	UDP/TCP 53	Spoofing, Poisoning	DNSSEC, filtrado
NAT	Privadas ↔ Pública	-	NAT Traversal, Spoofing	Firewalls, ACLs
PAT	NAT + puertos	-	Scanning, Hijacking	IDS/IPS, VPN

✨ Regla de oro en ciberseguridad
Estos servicios son básicos para que la red funcione.
⚠️ Si no los proteges, los atacantes los usarán como puerta de entrada.
