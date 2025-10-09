# 🌐 Conectividad IP y Gestión de Riesgos en el Sector Transporte

> Una guía clara, moderna y aplicada para profesionales y entusiastas de la ciberseguridad.

---

## 🚦 1. Conectividad IP

La conectividad IP es la **base de la comunicación en redes modernas**.  
En el sector transporte, permite que sistemas de tráfico, dispositivos IoT y sensores críticos trabajen juntos de forma segura y eficiente.

### 🔹 1.1 Enrutamiento estático vs dinámico

El enrutamiento es el proceso que permite a los routers decidir por dónde deben viajar los datos.  
Podemos diferenciar dos enfoques:

| Tipo de enrutamiento | Características | Ventajas | Limitaciones |
|----------------------|-----------------|----------|--------------|
| **Estático** | Rutas configuradas manualmente. | Control total, ideal para redes pequeñas. | No se adapta a cambios, difícil de escalar. |
| **Dinámico** | Protocolos que ajustan rutas automáticamente. | Escalable, adaptable, menos carga para administradores. | Más complejo y consume más recursos. |

📌 Ejemplo:  
- Una red pequeña de oficinas → **enrutamiento estático**.  
- Una red de aeropuertos o ferrocarriles → **OSPF o EIGRP**.

---

### 🔹 1.2 Protocolos de enrutamiento (RIP, OSPF, EIGRP)

- **RIP** → Protocolo sencillo basado en *número de saltos*.  
  Adecuado para redes pequeñas (máximo 15 saltos).  
- **OSPF** → Protocolo de estado de enlace, calcula la **ruta más corta** con el algoritmo de Dijkstra.  
  Ideal para redes grandes y complejas.  
- **EIGRP** → Protocolo híbrido de Cisco, combina lo mejor de RIP y OSPF.  
  Rápido, flexible y eficiente en redes empresariales.

⚖️ **Comparativa rápida**:

| Protocolo | Ideal para | Métrica principal | Ventajas |
|-----------|------------|------------------|----------|
| RIP | Redes pequeñas | Saltos | Sencillo |
| OSPF | Redes grandes | Coste (ancho de banda) | Escalable, rápido |
| EIGRP | Redes medianas/grandes (Cisco) | Métrica compuesta | Flexible, convergencia rápida |

---

### 🔹 1.3 ACLs (Access Control Lists)

Las **ACLs** son filtros que controlan qué tráfico puede entrar o salir de la red.  
Pueden configurarse en routers y switches para aumentar la seguridad:

- **Estándar** → filtran solo por dirección IP origen.  
- **Extendida** → permiten reglas avanzadas: dirección IP origen/destino, puertos, protocolos.

✅ Ejemplo: Permitir únicamente HTTPS (puerto 443) desde la red de administración hacia los servidores de datos.  
De esta forma se protege la información crítica frente a accesos no autorizados.

---

## 🔐 2. Gestión de Riesgos en Ciberseguridad

El sector transporte es considerado **infraestructura crítica**. Un ciberataque puede afectar operaciones, pasajeros, seguridad y reputación.  
Por ello, la **gestión de riesgos** es una estrategia fundamental.

### 2.1 Metodologías más usadas

- **NIST Cybersecurity Framework** → cinco pasos clave: Identificar, Proteger, Detectar, Responder y Recuperar.  
- **ISO 27001** → estándar internacional basado en mejora continua.  
- **MAGERIT** → metodología española para administraciones públicas, usada en sistemas de transporte crítico.

---

### 2.2 Evaluación de riesgos

La evaluación de riesgos es un proceso sistemático que incluye:

1. **Identificación de activos críticos** → sistemas de control de tráfico, redes SCADA, flotas y datos de pasajeros.  
2. **Detección de amenazas y vulnerabilidades** → ransomware, ataques DDoS, errores humanos o sistemas sin parchear.  
3. **Evaluación de impacto** → interrupciones operativas, fuga de datos, pérdida de confianza, consecuencias económicas.  
4. **Probabilidad** → ¿qué tan probable es que ocurra? (dependerá del nivel de exposición y del tipo de amenaza).  
5. **Priorización** → asignar recursos a los riesgos más críticos.  
6. **Implementación de medidas preventivas** → firewalls, IDS/IPS, MFA, segmentación de red, actualizaciones constantes.  
7. **Monitorización continua** → revisar periódicamente porque los riesgos evolucionan.

---

### 2.3 Tratamiento de riesgos

El tratamiento de riesgos responde a la pregunta: **¿qué hacemos con los riesgos detectados?**  
Las estrategias más comunes son:

- **Mitigar** → aplicar controles técnicos (firewalls, cifrado, IAM).  
- **Transferir** → contratar seguros cibernéticos o externalizar servicios críticos.  
- **Aceptar** → cuando el coste de mitigarlo es mayor al riesgo en sí (siempre con plan de contingencia).  
- **Evitar** → eliminar la actividad que genera el riesgo.  

---

### 2.4 Herramientas clave en el sector transporte

El ecosistema de seguridad en transporte cuenta con herramientas especializadas:

- 🛡️ **SIEM** → monitorización y correlación de eventos de seguridad.  
- 🚨 **IDS/IPS** → detección y bloqueo de intrusiones en tiempo real.  
- 🔍 **Gestión de vulnerabilidades** → detección de sistemas sin parches.  
- 👥 **IAM** → control estricto de identidades y accesos.  
- 🧪 **Red Teaming & Pentesting** → simulaciones de ataques reales.  
- 📦 **BCP/DRP** → continuidad de negocio y recuperación ante desastres.

---

## 📊 3. Buenas prácticas esenciales

- Mantener software y sistemas **siempre actualizados**.  
- Aplicar **autenticación multifactor** en accesos críticos.  
- Segmentar redes para aislar los sistemas más sensibles.  
- Realizar **auditorías y monitorización continua**.  
- Formar a los empleados en ciberseguridad.  

---

## ✅ Conclusión

La **conectividad IP** y la **gestión de riesgos** son dos pilares inseparables:  
- Sin conectividad, los sistemas no pueden operar.  
- Sin seguridad, la confianza y la continuidad se pierden.  

💡 La clave está en combinar **protocolos de red sólidos con metodologías de gestión de riesgos adaptadas al sector transporte**, logrando infraestructuras seguras, resilientes y confiables.
