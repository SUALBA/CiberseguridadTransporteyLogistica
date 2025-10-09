# 🌐 Conectividad IP y Gestión de Riesgos en el Sector Transporte

> Una guía clara, moderna y aplicada para profesionales y entusiastas de la ciberseguridad.

---

## 🚦 1. Conectividad IP

La conectividad IP es la **base de la comunicación en redes modernas**.  
En el sector transporte, permite que sistemas de tráfico, dispositivos IoT y sensores críticos trabajen juntos de forma segura y eficiente.

### 🔹 1.1 Enrutamiento estático vs dinámico

| Tipo de enrutamiento | Características | Ventajas | Limitaciones |
|----------------------|-----------------|----------|--------------|
| **Estático** | Rutas configuradas manualmente. | Control total, ideal para redes pequeñas. | No se adapta a cambios, difícil de escalar. |
| **Dinámico** | Protocolos que ajustan rutas automáticamente. | Escalable, adaptable, menos carga para admins. | Más complejo y consume más recursos. |

📌 Ejemplo:  
- En una red pequeña de oficinas → **enrutamiento estático**.  
- En una red de aeropuertos o ferrocarriles → **OSPF o EIGRP**.

---

### 🔹 1.2 Protocolos de enrutamiento (RIP, OSPF, EIGRP)

- **RIP** → Simple, usa *número de saltos*. Máx. 15 → útil solo en redes pequeñas.  
- **OSPF** → Estado de enlace, calcula la ruta más corta (Dijkstra). Ideal para redes grandes.  
- **EIGRP** → Híbrido Cisco, combina lo mejor de RIP y OSPF. Rápido y eficiente.  

⚖️ **Comparativa rápida**:

| Protocolo | Ideal para | Métrica principal | Ventajas |
|-----------|------------|------------------|----------|
| RIP | Redes pequeñas | Saltos | Sencillo |
| OSPF | Redes grandes | Coste (ancho de banda) | Escalable, rápido |
| EIGRP | Redes medianas/grandes (Cisco) | Métrica compuesta | Flexible, convergencia rápida |

---

### 🔹 1.3 ACLs (Access Control Lists)

Las **ACLs** permiten **controlar qué tráfico entra o sale** de la red.  
- **Estándar**: filtran por IP origen.  
- **Extendida**: filtran por IP, protocolo y puertos.  

✅ Ejemplo: Permitir solo HTTPS (443) desde la red de administración a los servidores de datos.

---

## 🔐 2. Gestión de Riesgos en Ciberseguridad

El sector transporte es **infraestructura crítica**: un ataque puede afectar operaciones, pasajeros y reputación.  
Por eso, aplicar **metodologías de gestión de riesgos** es clave.

### 2.1 Metodologías más usadas
- **NIST** → Identificar, Proteger, Detectar, Responder, Recuperar.  
- **ISO 27001** → Estándar internacional basado en mejora continua.  
- **MAGERIT** → Usado en España, orientado al sector público.

---

### 2.2 Evaluación de riesgos
Pasos principales:  
1. Identificar activos críticos.  
2. Detectar amenazas y vulnerabilidades.  
3. Evaluar impacto y probabilidad.  
4. Priorizar riesgos.  
5. Implementar medidas preventivas.  
6. Monitorizar y revisar continuamente.  

⚠️ Ejemplo de amenazas:  
- Ransomware en sistemas SCADA.  
- Ataques DDoS a sistemas de reservas.  
- Amenazas internas por empleados negligentes.

---

### 2.3 Tratamiento de riesgos
Opciones estratégicas:
- **Mitigar** → Firewalls, IDS/IPS, MFA, cifrado.  
- **Transferir** → Seguros cibernéticos, outsourcing.  
- **Aceptar** → Riesgos mínimos, con planes de contingencia.  
- **Evitar** → Eliminar la actividad de riesgo.  

---

### 2.4 Herramientas clave en el sector transporte
- 🛡️ **SIEM** → monitorización y correlación de eventos.  
- 🚨 **IDS/IPS** → detección y bloqueo de intrusiones.  
- 🔍 **Gestión de vulnerabilidades** → priorizar parches críticos.  
- 👥 **IAM** → control de identidades y accesos.  
- 🧪 **Red Teaming / Pentesting** → simulación de ataques.  
- 📦 **BCP/DRP** → continuidad de negocio y recuperación ante desastres.  

---

## 📊 3. Buenas prácticas esenciales
- Actualizar software y parches.  
- Segmentar redes críticas.  
- Aplicar autenticación multifactor.  
- Revisar y auditar periódicamente.  
- Formar al personal en ciberseguridad.  

---

## 📝 4. Quiz Premium

Pon a prueba tus conocimientos:

1. ¿Qué protocolo usa **número de saltos** como métrica principal?  
2. ¿Qué significa **riesgo residual** en ciberseguridad?  
3. ¿Cuál es la diferencia clave entre enrutamiento estático y dinámico?  
4. ¿Qué herramienta se usa para **correlacionar eventos de seguridad en tiempo real**?  
5. ¿Qué estrategia de tratamiento de riesgos consiste en contratar **seguros cibernéticos**?

*(Respuestas al final del artículo para los suscriptores premium)*

---

## ✅ Conclusión

La **conectividad IP** y la **gestión de riesgos** son dos caras de la misma moneda:  
- Sin conectividad, no hay operaciones eficientes.  
- Sin gestión de riesgos, no hay confianza ni continuidad.  

💡 La clave está en **combinar protocolos de red robustos con metodologías sólidas de gestión de riesgos** para construir un ecosistema de transporte más seguro, resiliente y confiable.

---
