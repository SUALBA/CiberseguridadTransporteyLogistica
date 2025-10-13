# 🚛 Ciberseguridad en Transporte y Logística

> Esquemas, casos de estudio y ejercicios prácticos para proteger infraestructuras críticas de transporte

[![GitHub stars](https://img.shields.io/github/stars/SUALBA/CiberseguridadTransporteyLogistica?style=social)](https://github.com/SUALBA/CiberseguridadTransporteyLogistica)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## 🎯 ¿Para quién es este repositorio?

- 🔐 **Profesionales de ciberseguridad** que trabajan en sectores de transporte
- 🚌 **Administradores de flotas** y sistemas de transporte público
- 🎓 **Estudiantes** de ciberseguridad e ingeniería de sistemas
- 🏢 **Responsables de IT** en empresas de logística
- 🔧 **Ingenieros de sistemas ITS** (Intelligent Transportation Systems)

---

## 📚 Contenido del Repositorio

### 🔥 Casos de Estudio Reales

#### 💥 [NotPetya: El Ataque que Paralizó la Logística Mundial](./Ataque_de_Ransomware_NotPetya_contra_Maersk_(2017).pdf)
Análisis exhaustivo del ciberataque más costoso de la historia y su devastador impacto en Maersk, líder mundial en transporte marítimo.

**Lo que aprenderás:**
- 🎯 **Anatomía del ataque**: Fases DORA (Discover, Offer, Request, Acknowledge) adaptadas a ransomware
- 💰 **Impacto cuantificado**: $250-300 millones en pérdidas
- 📊 **Números del desastre**: 45,000 PCs + 4,000 servidores inutilizados, 76 puertos paralizados
- 💾 **El rescate milagroso**: Cómo una copia de seguridad olvidada en África salvó a Maersk
- 🛡️ **Medidas preventivas**: Segmentación de red, NGFW, IDS/IPS, copias offline

**Formatos disponibles:**
- 📄 [Documento PDF](./Ataque_de_Ransomware_NotPetya_contra_Maersk_(2017).pdf)
- 🌐 [Versión HTML interactiva](./ataqueNOTPETJA.html) con visualizaciones

---

#### 🚌 Ataque a Empresa Municipal de Autobuses
*Caso de estudio de infraestructura crítica urbana*

**Sistemas comprometidos:**
- 🚦 Sistema de Control de Tráfico (SCADA)
- 💳 Plataforma de Pagos Electrónicos
- 📡 Red de Telemetría GPS
- 📹 Sistema de Videovigilancia

**Recursos incluidos:**
- 🗺️ [Diagrama de arquitectura de red](./autobusesRed.html) - Visualización SVG interactiva
- 📊 [Análisis de riesgos completo](./ejercicioAnalisisdeRiesgosEmpresaTranporte.html)
- 🔐 Matriz de amenazas por tipo de activo
- ✅ Checklist de medidas de mitigación

---

### 🎓 Ejercicios Prácticos

#### 🌐 [Fundamentos de Redes: DHCP, DNS, NAT y PAT](./ejercicioDHCP_DNS_%20NAT_PAT.html)

Ejercicio interactivo que cubre los protocolos fundamentales de red con enfoque en seguridad.

**Incluye:**
- ⚙️ Configuración práctica en routers Cisco
- 🔄 Flujos de protocolo con diagramas animados
- ⚔️ Vectores de ataque comunes (DHCP Starvation, DNS Poisoning, NAT Traversal)
- 🛡️ Controles defensivos (DHCP Snooping, DNSSEC, NGFW)
- 💻 Comandos CLI listos para implementar

**Formatos:**
- 🌐 [Versión HTML interactiva](./ejercicioDHCP_DNS_%20NAT_PAT.html) - Recomendado para aprendizaje
- 📝 [Versión Markdown](./ejercicioDHCP_DNS_%20NAT_PAT.md) - Para referencia rápida

---

## 🏗️ Arquitecturas de Referencia

### 🚌 Sistema de Transporte Urbano

Diagramas de infraestructura real con segmentación por VLANs y mejores prácticas de seguridad.

**Componentes cubiertos:**
- 🌐 **5 VLANs segmentadas**: Administración, Pagos, Monitoreo, IoT, Management
- 🔥 **Perímetro de seguridad**: Firewall UTM, Router Central, Switches gestionados
- 📍 **Dispositivos de campo**: TPVs, Displays informativos, Cámaras IP
- 📡 **Telemetría móvil**: GPS 3G/4G/5G en flota
- 🔐 **Conectividad segura**: Túneles VPN-IPSec entre estaciones

**Ver diagramas:**
- 🗺️ [Infraestructura completa](./autobusesRed.html)
- 🏢 [Red empresa de autobuses](./REdEmpresaAutobuses.html)

---

## 🎯 Temas Cubiertos

### Sectores de Transporte
- 🚌 **Transporte Público** (Autobuses urbanos e interurbanos)
- 🚂 **Ferrocarril** (Metro, cercanías, larga distancia)
- ✈️ **Aviación** (Sistemas aeroportuarios)
- 🚢 **Marítimo** (Puertos, navieras, logística portuaria)
- 📦 **Logística y Supply Chain** (Almacenes, distribución)

### Áreas Técnicas
- 🔐 **Seguridad en sistemas SCADA/ICS**
- 🌐 **Arquitecturas de red vehicular (V2X)**
- 📡 **IoT en flotas y telemetría**
- 💳 **Seguridad en sistemas de pago**
- 🛡️ **Protección de infraestructuras críticas**
- 📋 **Análisis y gestión de riesgos**
- ⚖️ **Compliance**: ISO 27001, IEC 62443, RGPD, PCI-DSS

### Amenazas Específicas
- 🦠 Ransomware en sistemas operacionales (NotPetya, WannaCry)
- 🌊 Ataques DDoS a sistemas de control
- 🎣 Spear Phishing dirigido a personal crítico
- 👤 Amenazas internas (empleados, contratistas)
- 🔧 Exploits en protocolos industriales (EternalBlue, Mimikatz)
- 📍 GPS Spoofing y manipulación de telemetría

---

## 🚀 Cómo Usar Este Repositorio

### Para Aprender
```bash
# 1. Clona el repositorio
git clone https://github.com/SUALBA/CiberseguridadTransporteyLogistica.git

# 2. Navega al directorio
cd CiberseguridadTransporteyLogistica

# 3. Abre los archivos HTML en tu navegador
# Recomendado: empezar por el caso NotPetya
```

### Para Implementar en tu Organización

1. **Evaluación inicial**
   - Revisa el [análisis de riesgos de transporte](./ejercicioAnalisisdeRiesgosEmpresaTranporte.html)
   - Identifica tus activos críticos usando la metodología presentada

2. **Diseño de arquitectura**
   - Usa los [diagramas de red](./autobusesRed.html) como referencia
   - Adapta la segmentación de VLANs a tu entorno

3. **Implementación de controles**
   - Aplica las medidas preventivas del [caso NotPetya](./Ataque_de_Ransomware_NotPetya_contra_Maersk_(2017).pdf)
   - Configura servicios básicos con el [ejercicio DHCP/DNS/NAT/PAT](./ejercicioDHCP_DNS_%20NAT_PAT.html)

4. **Monitorización y mejora continua**
   - Establece baselines de seguridad
   - Realiza auditorías periódicas
   - Mantén actualizados los parches

---

## 📊 Matriz de Contenido por Nivel

| Nivel | Contenido Recomendado | Objetivo |
|-------|----------------------|----------|
| 🟢 **Básico** | Ejercicio DHCP/DNS/NAT/PAT | Entender fundamentos de red |
| 🟡 **Intermedio** | Diagramas de arquitectura | Diseñar redes segmentadas |
| 🟠 **Avanzado** | Análisis de riesgos | Evaluar y mitigar amenazas |
| 🔴 **Experto** | Caso NotPetya | Respuesta a incidentes complejos |

---

## 🛡️ Frameworks y Estándares Aplicados

Este repositorio sigue mejores prácticas de:

- 📘 **NIST Cybersecurity Framework** (Identify, Protect, Detect, Respond, Recover)
- 🔐 **ISO/IEC 27001:2022** (Sistema de Gestión de Seguridad de la Información)
- 🏭 **IEC 62443** (Seguridad para sistemas de automatización y control industrial)
- 🇪🇺 **Esquema Nacional de Seguridad (ENS)** - España
- 💳 **PCI-DSS** (para sistemas de pago)
- 📜 **RGPD** (protección de datos personales)

---

## 🤝 Contribuir

¿Tienes un caso de estudio, diagrama o ejercicio que añadir? ¡Las contribuciones son bienvenidas!

**Áreas donde necesitamos ayuda:**
- 📝 Casos de estudio de otros sectores (aviación, ferrocarril, marítimo)
- 🔧 Ejercicios de hardening de sistemas embarcados
- 📊 Playbooks de respuesta a incidentes
- 🌍 Traducciones a otros idiomas

Ver [CONTRIBUTING.md](CONTRIBUTING.md) para detalles.

---

## 📞 Contacto y Soporte

- 👤 **Autor**: Susana Alba
- 🌐 **Web**: [sualba.dev](https://sualba.dev)
- 
- 📧 **Email**: [sualba.dev@gmail.com](mailto:sualba.dev@gmail.com)

---

## 📄 Licencia

Este proyecto está bajo licencia MIT. Ver [LICENSE](LICENSE) para más detalles.

---

## ⭐ Agradecimientos

Este repositorio fue creado para contribuir a la comunidad de ciberseguridad y ayudar a proteger infraestructuras críticas de transporte. Si encuentras útil este contenido, considera:

- ⭐ Dar una estrella al repositorio
- 🔄 Compartirlo con colegas del sector
- 💬 Proporcionar feedback y sugerencias
- 🤝 Contribuir con nuevos casos o mejoras

---

## 🔖 Tags y Topics

`cybersecurity` `transportation-security` `logistics` `iot-security` `scada` `its` `critical-infrastructure` `ransomware` `case-study` `network-security` `fleet-management` `public-transport` `smart-cities` `incident-response`

---

<div align="center">

**Proteger el transporte es proteger la movilidad de la sociedad**

🚛 🚂 ✈️ 🚢 🚌

*Desarrollado con 💙 para mejorar la ciberseguridad en infraestructuras críticas*

</div>
