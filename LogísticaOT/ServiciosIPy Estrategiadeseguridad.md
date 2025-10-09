# 🌐 Servicios IP y Estrategia de Ciberseguridad  
*Una guía clara, profesional y cercana para entender los fundamentos técnicos y estratégicos de la seguridad digital.*

---

## 📖 Índice  
1. [Servicios IP](#-servicios-ip)  
   - [DHCP y DNS](#-dhcp-y-dns)  
   - [NAT y PAT](#-nat-y-pat)  
   - [VPNs y GRE Tunnels](#-vpns-y-gre-tunnels)  
2. [Estrategia de Ciberseguridad](#-estrategia-de-ciberseguridad)  
   - [Definición](#-definición-de-una-estrategia-de-ciberseguridad)  
   - [Alineación con los objetivos del transporte](#-alineación-con-los-objetivos-del-sector-transporte)  
   - [Implementación](#-implementación-de-la-estrategia-de-ciberseguridad)  
   - [Marcos de referencia](#-marcos-de-referencia-en-ciberseguridad)  
3. [Resumen](#-resumen)  
4. [Glosario](#-glosario)  
5. [Enlaces de interés](#-enlaces-de-interés)  

---

## 🌍 Servicios IP  

Los **Servicios IP** son el corazón de las redes modernas. Gracias a ellos podemos:  
✔️ Conectar dispositivos.  
✔️ Asignar direcciones dinámicamente.  
✔️ Traducir direcciones privadas a públicas.  
✔️ Proteger datos y comunicaciones.  

### 🔑 DHCP y DNS  

#### 📌 DHCP (Dynamic Host Configuration Protocol)  
- Asigna **automáticamente direcciones IP** a dispositivos en la red.  
- Reduce errores humanos y simplifica la administración.  

👉 **Ejemplo:** Tu móvil se conecta al Wi-Fi de casa → el router (servidor DHCP) le entrega una IP válida sin que tengas que configurar nada.

#### 🌐 DNS (Domain Name System)  
- Traduce **nombres de dominio legibles** (ej: `google.com`) en direcciones IP (ej: `142.250.190.78`).  
- Sin DNS tendríamos que memorizar números.  

⚠️ **Atención en ciberseguridad:** el DNS es objetivo de ataques como **DNS spoofing** o **envenenamiento de caché**.  
✅ Solución: **DNSSEC** y monitorización constante.

---

### 🔄 NAT y PAT  

#### 📌 NAT (Network Address Translation)  
- Traduce IPs privadas en **una IP pública**.  
- Aporta **anonimización y eficiencia** en el uso de direcciones IPv4.  

✔️ Beneficio en seguridad: oculta la red interna.  
❌ No es suficiente por sí solo → debe combinarse con **firewalls** y segmentación.  

#### 📌 PAT (Port Address Translation)  
- Extiende NAT añadiendo **puertos** para diferenciar conexiones.  
- Permite que **muchos dispositivos compartan la misma IP pública**.  

👉 **Ejemplo visual:**  
- PC1 → `192.168.0.1:1001` → `85.123.45.67:1001`  
- PC2 → `192.168.0.2:1002` → `85.123.45.67:1002`  

Desde fuera, todo parece provenir de **85.123.45.67**, pero el router sabe a quién pertenece cada conexión.

---

### 🔐 VPNs y GRE Tunnels  

#### 📌 VPN (Virtual Private Network)  
- Crea un **túnel seguro cifrado** entre redes o dispositivos.  
- Garantiza **confidencialidad e integridad** de datos.  
- Ideal para empleados remotos o conexiones a infraestructuras críticas.  

👉 **Ejemplo:** Te conectas desde una cafetería pública a tu empresa. La **VPN cifra los datos** para que ni un hacker en esa red pueda interceptarlos.

#### 📌 GRE Tunnels (Generic Routing Encapsulation)  
- Encapsula distintos protocolos en un túnel IP.  
- Muy útil para **interconectar redes con infraestructuras distintas**.  
- No cifra por defecto → suele usarse combinado con **IPsec**.  

👉 **Analogía:** Es como un túnel de carretera que permite que pasen vehículos de cualquier tipo, incluso si normalmente no estarían permitidos.

---

## 🛡️ Estrategia de Ciberseguridad  

En el **sector transporte**, la ciberseguridad es crítica:  
🚉 Sistemas de control de tráfico.  
✈️ Plataformas de gestión de pasajeros.  
🚚 Flotas y logística.  
⚡ Infraestructuras SCADA.  

Una buena estrategia debe ser **proactiva, integral y alineada al negocio**.  

### 📌 Definición de una estrategia de ciberseguridad  
- **Identificación de activos críticos.**  
- **Evaluación de riesgos** (ransomware, DDoS, insiders).  
- **Objetivos claros y medibles.**  
- **Políticas de seguridad** (accesos, cifrado, autenticación).  

---

### 📌 Alineación con los objetivos del sector transporte  
Una estrategia de ciberseguridad debe apoyar directamente a la misión del negocio:  

- **Seguridad de pasajeros.**  
- **Minimizar interrupciones operativas.**  
- **Cumplimiento normativo (ENS, RGPD, NIS).**  
- **Optimización de recursos.**  

---

### 📌 Implementación de la estrategia de ciberseguridad  
**Pasos clave:**  
1. Desarrollo de **políticas de seguridad**.  
2. **Capacitación y concienciación** del personal.  
3. Implementación de **tecnologías** → NGFW, IDS/IPS, VPNs, segmentación.  
4. **Gestión de riesgos y respuesta a incidentes.**  
5. **Auditoría y mejora continua.**  

---

### 📌 Marcos de referencia en ciberseguridad  

Los principales frameworks que marcan la diferencia:  
- **ISO/IEC 27001** → SGSI, estándar internacional.  
- **NIST Cybersecurity Framework** → Identificar, Proteger, Detectar, Responder, Recuperar.  
- **CIS Controls** → buenas prácticas priorizadas.  
- **ENS (España)** → obligatorio en sector público.  
- **Directiva NIS (UE)** → protección de infraestructuras críticas.  
- **ITIL** → gestión de servicios TI.  
- **Zero Trust** → nunca confiar, siempre verificar.  
- **COBIT** → gobernanza TI, alineación negocio-tecnología.  

---

## 📝 Resumen  

Este módulo combina **fundamentos técnicos (Servicios IP)** con **visión estratégica (Ciberseguridad)**.  
La clave está en:  
- Entender cómo funcionan **DHCP, DNS, NAT, PAT, VPN y GRE**.  
- Desarrollar una **estrategia sólida**, alineada con el negocio y apoyada en **marcos de referencia internacionales**.  

---

## 📚 Glosario  

- **DHCP**: asigna IPs dinámicas.  
- **DNS**: traduce nombres en IPs.  
- **NAT/PAT**: traducción de IPs y puertos.  
- **VPN**: túnel seguro y cifrado.  
- **GRE**: túnel multiprotocolo.  
- **ENS**: normativa española de seguridad.  
- **ISO 27001 / NIST / COBIT**: frameworks clave de referencia.  

---

## 🔗 Enlaces de interés  

- 🎥 [Túneles GRE explicados](https://www.youtube.com/watch?v=FeUl50V9Uwc)  
- 📘 [Metodología de Ciberdefensa para Organizaciones](https://publications.iadb.org/publications/spanish/document/Metodologia-de-ciberdefensa-para-organizaciones-version-2.0.pdf)  
- 🛡️ [Autodiagnóstico de Ciberseguridad para PYMEs](https://autodiagnosticociberseguridad.ipyme.org/)  
- 📑 [Ciberseguridad en el transporte: cómo implementarla](https://safecore.io/es/la-cybersecurity-nei-trasporti-come-implementarla/)  

---
✍️ *Elaborado con un enfoque profesional, cercano y práctico para el sector transporte y cualquier organización que quiera fortalecer su ciberseguridad.*  
