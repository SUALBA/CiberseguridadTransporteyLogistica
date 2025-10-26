# Solución Profesional: Configuración de Firewall y ACLs en Packet Tracer

**Ejercicio Módulo 5: Ciberseguridad en Redes y Sistemas de Transporte y Logística**

---

## 1. Introducción

Este documento presenta una solución completa y profesional para el Ejercicio del Módulo 5, enfocado en la configuración de un firewall y listas de control de acceso (ACLs) en una red simulada. El objetivo es proteger una red de oficina con varios departamentos, asegurando el cumplimiento de políticas de seguridad específicas.

La solución se ha diseñado utilizando **Cisco Packet Tracer** como herramienta de simulación, siguiendo las mejores prácticas de la industria para la segmentación de redes y la implementación de políticas de seguridad.

### Requisitos del Ejercicio

El escenario de red debe cumplir con las siguientes directrices de seguridad:

1.  **Acceso Restringido a Finanzas:** Solo los empleados del departamento de administración pueden acceder al sistema de finanzas.
2.  **Salida a Internet Controlada:** Solo los dispositivos internos de la oficina pueden acceder a Internet.
3.  **Bloqueo de Tráfico Externo:** Todo el tráfico no autorizado proveniente de Internet debe ser bloqueado.

---

## 2. Diseño de la Topología de Red

Para cumplir con los requisitos, se ha diseñado una topología de red segmentada en tres zonas principales: Administración, Otros Departamentos y Servidores. Esta segmentación permite aplicar políticas de seguridad granulares y controlar el flujo de tráfico entre los diferentes departamentos.

### Diagrama de la Topología

A continuación, se muestra el diagrama de la red implementada:

![Diagrama de la Topología de Red](https://private-us-east-1.manuscdn.com/sessionFile/dqzeSCd9w0jcJl0oEsAgJA/sandbox/lt0EaqRcFWKabahGcTKxKw-images_1761251061543_na1fn_L2hvbWUvdWJ1bnR1L3RvcG9sb2dpYV9yZWQ.png?Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9wcml2YXRlLXVzLWVhc3QtMS5tYW51c2Nkbi5jb20vc2Vzc2lvbkZpbGUvZHF6ZVNDZDl3MGpjSmwwb0VzQWdKQS9zYW5kYm94L2x0MEVhcVJjRldLYWJhaEdjVEt4S3ctaW1hZ2VzXzE3NjEyNTEwNjE1NDNfbmExZm5fTDJodmJXVXZkV0oxYm5SMUwzUnZjRzlzYjJkcFlWOXlaV1EucG5nIiwiQ29uZGl0aW9uIjp7IkRhdGVMZXNzVGhhbiI6eyJBV1M6RXBvY2hUaW1lIjoxNzk4NzYxNjAwfX19XX0_&Key-Pair-Id=K2HSFNDJXOU9YS&Signature=WXGucpmWgjpIFuKYENw4meQjlbIfSC-i3K0b1ijcSLgExTa0eK0dzCw6TcgurzPzmbMLnTf2TfhpoDG2FDG9KNCZz7AYIxQUzKqR5R3~Be7bOXIHTEAviwq5NZwHEE0MOud50zn4wIESqrAfd61vBBg67LAKLmAcaAOftGe07EClgPKD451kpkQfc7QKwqY15N6J1CqDKFj5tnVt2jQDIOxxsDXrk90JlVcP~zK9WRGDVTaRoALNcK8DEnop~Lif7n-zqAN4ODFcZ8ySx35rKkUaXkf6U8EkS8SXS~9fmoE6pii4FOVulIiRZYFjjcQl5Xie5G21CD1b6KoNxxZ5YA__)

### Segmentación de Red y Direccionamiento IP

La red se ha dividido en las siguientes subredes:

| Segmento | Red | Máscara | Gateway | Descripción |
|---|---|---|---|---|
| Administración | 192.168.10.0 | 255.255.255.0 | 192.168.10.1 | Departamento de Administración |
| Otros Departamentos | 192.168.20.0 | 255.255.255.0 | 192.168.20.1 | Resto de la oficina |
| Servidores | 192.168.30.0 | 255.255.255.0 | 192.168.30.1 | Servidor de Finanzas |
| Internet (WAN) | 200.1.1.0 | 255.255.255.0 | N/A | Conexión externa simulada |

---

## 3. Guía de Implementación en Packet Tracer

Dado que no es posible generar directamente un archivo `.pkt`, he preparado una guía detallada paso a paso para que usted pueda construir la topología y aplicar las configuraciones en Packet Tracer. Este enfoque le permitirá comprender a fondo cada etapa del proceso.

**El documento completo con la guía se encuentra adjunto como `guia_packet_tracer.md`.**

Este manual incluye:

-   **Construcción de la topología:** Cómo agregar y conectar routers, switches y PCs.
-   **Configuración de dispositivos:** Instrucciones detalladas para configurar las direcciones IP en cada PC y servidor.
-   **Configuración del router:** El script completo para el `Router-Principal`, incluyendo interfaces, ACLs y NAT.
-   **Verificación y pruebas:** Comandos y procedimientos para verificar que la solución funciona como se espera.

---

## 4. Scripts de Configuración

Para facilitar la implementación, se proporcionan los scripts de configuración completos para los dispositivos de red.

### Configuración del Router Principal (`Router-Principal`)

Este script contiene toda la lógica de seguridad, incluyendo la configuración de las interfaces, las listas de control de acceso (ACLs) para el filtrado de tráfico y la configuración de NAT para permitir el acceso a Internet.

**El script completo se encuentra en el archivo adjunto: `configuracion_router.txt`**

### Configuración de Dispositivos Finales

Este archivo detalla las configuraciones IP (dirección IP, máscara de subred, puerta de enlace y DNS) para cada PC y para el servidor de finanzas.

**Las configuraciones se encuentran en el archivo adjunto: `configuracion_dispositivos.txt`**

---

## 5. Plan de Verificación y Pruebas

Para validar que la implementación cumple con todos los requisitos de seguridad, se ha diseñado un plan de pruebas exhaustivo. La siguiente tabla resume las pruebas a realizar y los resultados esperados.

**El plan de pruebas completo y detallado se encuentra en el archivo adjunto: `tabla_pruebas.md`**

| # | Prueba | Origen | Destino | Resultado Esperado | Política Verificada |
|---|---|---|---|---|---|
| 1 | Acceso a Finanzas desde Admin | PC-Admin1 | Servidor-Finanzas | ✅ **Éxito** | Permitir Admin → Finanzas |
| 2 | Acceso a Finanzas desde Otros | PC-Otros1 | Servidor-Finanzas | ❌ **Bloqueado** | Denegar Otros → Finanzas |
| 3 | Acceso a Internet desde Admin | PC-Admin1 | Internet (ISP) | ✅ **Éxito** | Permitir salida a Internet |
| 4 | Tráfico entrante desde Internet | Internet (ISP) | PC-Admin1 | ❌ **Bloqueado** | Bloquear tráfico externo |

---

## 6. Conclusión

La solución propuesta implementa de manera efectiva los controles de seguridad requeridos en el ejercicio. Mediante el uso de **segmentación de red**, **listas de control de acceso (ACLs)** y **Network Address Translation (NAT)**, hemos logrado:

-   **Aislar los activos críticos:** El servidor de finanzas está protegido y solo es accesible desde el departamento de administración.
-   **Controlar el perímetro de la red:** Se permite el tráfico de salida hacia Internet de forma controlada, mientras que se bloquea todo el tráfico entrante no solicitado, protegiendo la red interna de amenazas externas.
-   **Cumplir con las políticas de seguridad:** La configuración garantiza que se cumplan todas las reglas de negocio y seguridad especificadas.

Le recomiendo seguir la `guia_packet_tracer.md` adjunta para replicar este escenario. Este ejercicio práctico es fundamental para comprender los conceptos de defensa en profundidad y la seguridad en redes.

Si tiene alguna pregunta durante la implementación, no dude en consultarme.


