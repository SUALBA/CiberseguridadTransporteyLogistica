# 🌐 Ejercicio Módulo 4 – DHCP, DNS, NAT y PAT en redes de Transporte y Logística  

## 1️⃣ DHCP – Dynamic Host Configuration Protocol  

### 🔹 ¿Qué es?  
El **DHCP** es un protocolo de red que asigna **direcciones IP y parámetros de configuración** a los dispositivos de forma **automática**.  
- Funciona en **capa 7 (Aplicación)** del modelo OSI.  
- Utiliza **UDP** como protocolo de transporte (puerto **67 servidor** y **68 cliente**).  

### 🔹 ¿Cómo funciona?  
Proceso **DORA**:  
1. **Discover** → el cliente busca un servidor DHCP.  
2. **Offer** → el servidor responde con una oferta de IP.  
3. **Request** → el cliente solicita esa IP.  
4. **Acknowledge** → el servidor confirma y asigna la IP.  

👉 Resultado: el dispositivo recibe IP, máscara, gateway y DNS.  

---

## 2️⃣ DNS – Domain Name System  

### 🔹 ¿Qué es?  
El **DNS** es el "traductor de Internet". Convierte **nombres de dominio** en **direcciones IP**.  
- Funciona en **capa 7 (Aplicación)**.  
- Utiliza **UDP/53** para consultas rápidas y **TCP/53** para transferencias de zona.  

### 🔹 ¿Cómo funciona?  
1. El cliente pregunta: *“¿Cuál es la IP de `miportal.com`?”*  
2. El servidor DNS responde con la IP correspondiente.  
3. El navegador se conecta a esa IP.  

👉 Sin DNS, tendríamos que memorizar números como `142.250.190.78`.  

⚠️ **En ciberseguridad:**  
- Vulnerable a **DNS spoofing** o **cache poisoning**.  
- Solución → usar **DNSSEC** y monitorización.  

---

## 3️⃣ NAT – Network Address Translation  

### 🔹 ¿Qué es?  
El **NAT** es un protocolo que traduce **direcciones IP privadas ↔ públicas**.  
- Funciona en el **router** (capa 3 - Red).  
- Permite que múltiples dispositivos de la red interna usen **una sola IP pública**.  

### 🔹 Tipos de NAT  
- **Static NAT**: 1 IP privada ↔ 1 IP pública.  
- **Dynamic NAT**: varias IP privadas ↔ un rango de IP públicas.  
- **NAT Overload (PAT)**: muchas IP privadas ↔ **una sola IP pública + puertos**.  

👉 Beneficio: optimiza el uso de direcciones IPv4.  

⚠️ No es un protocolo de seguridad, pero **oculta las IP internas**.  

---

## 4️⃣ PAT – Port Address Translation  

### 🔹 ¿Qué es?  
El **PAT** es una extensión de NAT.  
- Usa **números de puerto** para diferenciar las conexiones de distintos dispositivos.  
- También se le llama **NAT Overload**.  

### 🔹 ¿Cómo funciona?  
Ejemplo:  
- Laptop → `192.168.1.2:1025` → `85.123.45.67:2001`  
- Smartphone → `192.168.1.3:1040` → `85.123.45.67:2002`  
- Consola → `192.168.1.4:1100` → `85.123.45.67:2003`  

👉 Así todos usan la **misma IP pública**, pero con **puertos distintos**.  

---

## 🚀 Conclusión  

- **DHCP** → asigna IPs dinámicamente.  
- **DNS** → traduce nombres ↔ IPs.  
- **NAT** → traduce IPs privadas ↔ públicas.  
- **PAT** → traduce IPs + usa puertos para diferenciar sesiones.  

🔐 En ciberseguridad, todos estos servicios deben configurarse con cuidado porque:  
- DHCP puede ser explotado con ataques **spoofing**.  
- DNS es objetivo de **redirecciones maliciosas**.  
- NAT/PAT ayudan a ocultar redes internas, pero requieren apoyo de **firewalls y segmentación**.  

---
