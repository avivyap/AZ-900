--------
# Azure Monitor

Azure Monitor es el servicio de supervisión de Azure que permite recopilar, analizar y visualizar métricas y registros de recursos de Azure y de entornos locales.
## Componentes principales

### Metrics

Recopilan datos de rendimiento casi en tiempo real, como:

- CPU
- Memoria (según el recurso)
- Disco
- Tráfico de red
### Logs

Almacenan información en un **Log Analytics Workspace** para poder realizar consultas y análisis mediante KQL (Kusto Query Language).

### Alerts

Permiten generar notificaciones cuando se cumple una condición.

Ejemplos:

- Una VM deja de responder.
- El uso de CPU supera el 90 %.
- La latencia de una aplicación supera los 5000 ms.

### Dashboards

Permiten crear paneles personalizados para visualizar métricas, registros y el estado de los recursos.

### Application Insights

Servicio orientado a supervisar aplicaciones.

Permite recopilar información como:

- Disponibilidad
- Rendimiento
- Excepciones
- Dependencias
- Solicitudes HTTP

### Azure Monitor Agent (AMA)

Agente que se instala en máquinas virtuales Windows y Linux para:

- Recopilar métricas.
- Recopilar registros (logs).
- Enviar la información a un **Log Analytics Workspace**.

> **Importante para el AZ-104:** Si una pregunta menciona recopilar registros de una máquina virtual y enviarlos a **Log Analytics**, la respuesta suele ser **Azure Monitor Agent (AMA)**.