
# Automatización y Protección contra Ataques 🚦



---

## 1. Automatización y Programabilidad ⚙️

### 1.1 Conceptos básicos de automatización
- **Automatización en redes**: ejecución de tareas repetitivas y complejas sin intervención manual constante.
- **Ventajas**:
  - ✅ Mayor eficiencia operativa.  
  - ✅ Reducción de errores humanos.  
  - ✅ Respuesta rápida a incidentes.

📌 *Ejemplo*: En un sistema de transporte público, la automatización puede reconfigurar rutas de red según condiciones del tráfico o aislar segmentos comprometidos tras un ciberataque.

### 1.2 Programación y scripting en redes 💻
- Permiten automatizar configuraciones y monitoreo.  
- Lenguajes comunes: **Python, Bash, PowerShell**.  
- Scripts → reducen tiempos, generan alertas, ejecutan backups.

📌 *Ejemplo*: Un script en Python que revisa el estado de routers/switches y alerta si detecta anomalías.

### 1.3 Uso de APIs y herramientas de automatización 🔌
- **APIs** → interacción programada con dispositivos y sistemas.  
- **Herramientas destacadas**:
  - REST APIs → gestión remota con HTTP.  
  - **Ansible** → playbooks YAML para configurar routers/firewalls.  
  - **Cisco ACI** → políticas centralizadas.  
  - **Puppet y Chef** → administración masiva de infraestructuras.

📌 *Ejemplo*: Una API REST que reconfigura rutas en tiempo real para priorizar transporte en caso de congestión.

---

## 2. Protección contra Ataques 🔒

### 2.1 Técnicas comunes en transporte 🚉✈️🚢
- **Ransomware** → cifrado de sistemas críticos (ej. control de tráfico).  
- **DDoS** → saturación de reservas y sistemas de pasajeros.  
- **Phishing/Spear Phishing** → robo de credenciales a empleados.  
- **Explotación SCADA** → manipulación de sistemas industriales.  
- **Intercepción de comunicaciones V2V/V2I** → manipulación de tráfico conectado.

### 2.2 Defensa en profundidad 🛡️
- Estrategia de **múltiples capas de seguridad**:
  - 🔑 Cifrado de datos (en tránsito y reposo).  
  - 🔀 Segmentación de red.  
  - 🔐 Autenticación multifactor (MFA).  
  - 👁️ IDS/IPS para detectar y bloquear intrusiones.  
  - 📡 Monitorización continua.

### 2.3 Plan de Respuesta a Incidentes (PRI) 📑
**Fases principales:**
1. **Preparación** → equipos, roles, simulaciones, IDS/Firewalls.  
2. **Identificación** → detección y clasificación de incidentes.  
3. **Contención** → aislamiento de sistemas comprometidos.  
4. **Erradicación** → eliminación de malware y aplicación de parches.  
5. **Recuperación** → restauración de servicios críticos.  
6. **Lecciones aprendidas** → documentación y actualización del plan.

### 2.4 Tecnologías de protección específicas ⚡
- **NGFW** → firewalls de nueva generación.  
- **VPNs** → cifrado en accesos remotos.  
- **Sistemas anti-DDoS**.  
- **Segmentación de red**.  
- **IDS/IPS**.  
- **Cifrado TLS**.  
- **MFA**.  
- **SOAR** → automatización de respuesta.  
- **SCADA seguros**.  
- **Gestión de vulnerabilidades**.

---

## 3. Pregunta de Test ✅❓

- **Monitoreo continuo de redes es importante porque...**  
  👉 Permite detectar y responder a amenazas en tiempo real.

- **Objetivo de un túnel VPN...**  
  👉 Cifrar las comunicaciones entre redes a través de internet.

- **El uso de scripts en redes ayuda a...**  
  👉 Automatizar tareas repetitivas como la configuración de routers y switches.

- **Herramientas de automatización de redes permiten...**  
  👉 Configurar y gestionar redes automáticamente sin intervención manual.

- **Un ataque de fuerza bruta es...**  
  👉 Intento de probar múltiples contraseñas hasta acceder al sistema.

- **Plan de respuesta a incidentes debe incluir...**  
  👉 Procedimientos para identificar, contener y erradicar un ataque.

- **Una API en redes se utiliza para...**  
  👉 Facilitar la interacción entre aplicaciones o dispositivos.

- **En redes de transporte, una API puede ayudar a...**  
  👉 Automatizar la configuración y gestión de dispositivos.

- **Ventaja de APIs en automatización...**  
  👉 Integración y automatización de configuraciones desde distintos sistemas.

- **Defensa en profundidad apropiada...**  
  👉 Implementar múltiples capas (firewalls, cifrado, MFA, segmentación).

- **Tecnología de protección contra ataques en transporte...**  
  👉 Firewalls.

- **Objetivo principal de tecnologías de protección...**  
  👉 Detectar y prevenir amenazas como malware, phishing o DDoS.

- **Propósito del scripting en redes...**  
  👉 Automatizar tareas repetitivas y mejorar eficiencia.

- **Propósito de un plan de respuesta a incidentes...**  
  👉 Minimizar impacto y restaurar operaciones rápidamente.

- **Qué es la automatización de redes...**  
  👉 Ejecución automática de tareas como configuraciones y monitoreo.

- **Defensa en profundidad es...**  
  👉 Uso de múltiples capas de seguridad.

- **Ataque DoS es...**  
  👉 Interrumpir servicio de una red al sobrecargarla de tráfico.

- **Phishing es...**  
  👉 Correos fraudulentos para engañar y obtener credenciales.

- **Ransomware es...**  
  👉 Malware que cifra datos y exige rescate.

- **Ataque que intenta saturar una red...**  
  👉 DDoS.

---

## 4. Glosario 📖

- **API**: Reglas que permiten interacción entre sistemas.  
- **Automatización de redes**: Ejecución automática de configuraciones.  
- **Fuerza bruta**: Prueba de múltiples contraseñas.  
- **DDoS**: Saturar con tráfico malicioso.  
- **Defensa en profundidad**: Múltiples capas de seguridad.  
- **Phishing**: Engaño mediante correos falsos.  
- **Plan de Respuesta a Incidentes**: Procedimientos de reacción ante ciberataques.  
- **Ransomware**: Malware que cifra datos y exige rescate.  
- **Scripting**: Automatización mediante programación.  
- **Segmentación de red**: División en subredes aisladas.  
- **IDS/IPS**: Sistemas para detectar o prevenir intrusiones.  
- **MFA**: Autenticación multifactor.  

---

## 5. Enlaces de interés 🔗

- [Automatización y Programabilidad de Redes](https://www.youtube.com/watch?v=IAw3AckXdoE)  
- [INCIBE - Respuesta a incidentes](https://www.incibe.es/empresas/blog/respuesta-incidentes-estais-preparados)  
- [Plantilla plan de respuesta](https://cgalma.com/wp-content/uploads/2024/05/Plantilla-de-respuesta-a-incidentes-de-ciberseguridad.pdf)

---

✍️ **Autor:sualba.dev @2025 ** Material adaptado para estudio y divulgación en ciberseguridad en transporte.
