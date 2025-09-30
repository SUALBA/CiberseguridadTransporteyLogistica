# 🌐 Fundamentos de Redes y Ciberseguridad en el Transporte

> 📘 **Resumen práctico + visual**: preguntas tipo test, teoría de redes y conceptos de ciberseguridad aplicados al sector transporte.

---

## 🔹 Conceptos básicos de redes

Una **red** es un conjunto de dispositivos (ordenadores, servidores, routers, switches, etc.) que se interconectan para **compartir información y recursos**.

---

## 🏗 Modelos de referencia

### ⚡ Modelo OSI (7 capas)
1. **Física** → 🔌 Transmisión de bits (cables, señales, conectores).  
2. **Enlace de datos** → 🆔 Direcciones **MAC**, control de errores locales.  
3. **Red** → 🌍 Direccionamiento **IP** y enrutamiento.  
4. **Transporte** → 🚦 Confiabilidad extremo a extremo (**TCP/UDP**).  
5. **Sesión** → 🔄 Mantiene la comunicación entre dispositivos.  
6. **Presentación** → 🔐 Traducción, compresión, cifrado.  
7. **Aplicación** → 🌐 Servicios de red (**HTTP, FTP, DNS**).  

### 🌍 Modelo TCP/IP (4 capas)
- **Acceso a la red** (física + enlace).  
- **Internet** (direccionamiento IP, enrutamiento).  
- **Transporte** (TCP/UDP).  
- **Aplicación** (HTTP, FTP, SMTP, DNS).  

📌 **Truco rápido:**  
- OSI = **7 capas**  
- TCP/IP = **4 capas**  

```plaintext
OSI (7)                         TCP/IP (4)
-------------------------------------------------
Aplicación                      Aplicación
Presentación
Sesión
Transporte                      Transporte
Red                             Internet
Enlace de Datos                 Acceso a la red
Física

🚦 Tecnologías de red en el transporte
🖥️ SCADA

Monitorea y controla procesos industriales críticos (🚉 trenes, ✈️ aeropuertos, 🚦 semáforos).

✅ Útil pero 🎯 objetivo de ciberataques.

🚗 ITS (Intelligent Transportation Systems)

Sensores + redes para gestionar tráfico en tiempo real, peajes electrónicos y vehículos conectados (V2V, V2I).

🎯 Beneficios: eficiencia, seguridad, sostenibilidad.

🛠️ Dispositivos de red clave
Dispositivo	Función principal	Ejemplo práctico
Router	🔀 Interconecta redes distintas (IP, NAT)	Conectar LAN ↔ WAN
Switch	🔗 Conecta dispositivos en la misma LAN	PCs de una oficina
Firewall	🔥 Filtra tráfico por reglas	Bloqueo de puertos no autorizados
Access Point	📡 Wi-Fi en la red	Zona Wi-Fi en estación
IDS/IPS	🛡️ Detectan y bloquean intrusiones	Alertas de ataques

📌 Atajo mental:

Switch = dentro de la red.

Router = entre redes.

Firewall = control de acceso.

🔐 Ciberseguridad en el transporte

La ciberseguridad protege la tríada CIA:

🔑 Pilares

Confidencialidad → Solo acceden usuarios autorizados 👤.

Integridad → Los datos no se alteran sin permiso ✍️.

Disponibilidad → Los sistemas funcionan cuando se necesitan ⏱️.

⚠️ Amenazas principales

💣 Ransomware → Secuestro de datos.

🎣 Phishing → Robo de credenciales.

🌊 DDoS → Saturación de sistemas.

🕹️ Ataques a SCADA/ITS → Manipulación de tráfico o trenes.

👥 Amenazas internas → Errores humanos o sabotaje.

🧩 Anatomía de un ciberataque

🔍 Reconocimiento

🛠️ Preparación

🚪 Intrusión

🔓 Escalada de privilegios

🔀 Movimiento lateral

🎯 Ejecución del objetivo

📤 Exfiltración

♻️ Persistencia

📊 Impacto de los ciberataques en transporte

🚧 Interrupción de servicios (trenes, vuelos, tráfico).

📉 Daño reputacional.

💸 Pérdidas económicas (rescates, multas).

⚡ Riesgo físico (accidentes).

🔺 Gráfico: Tríada CIA en ciberseguridad 
        +-------------------+
        | Confidencialidad  |
        | (Acceso limitado) |
        +-------------------+
                 ▲
                 |
+----------------+----------------+
| Integridad                     |
| (Datos sin alteraciones)       |
+----------------+----------------+
                 |
                 ▼
        +-------------------+
        | Disponibilidad    |
        | (Acceso garant.)  |
        +-------------------+

✅ Conclusión

El transporte moderno depende de redes y sistemas interconectados, lo que lo hace más eficiente 🚀 pero también más vulnerable 🛑.
Conocer modelos de red, dispositivos clave y principios de ciberseguridad es esencial para proteger estas infraestructuras críticas.
