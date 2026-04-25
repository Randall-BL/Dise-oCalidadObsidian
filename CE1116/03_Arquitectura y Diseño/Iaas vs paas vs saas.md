---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags:
  - cloud
  - modelos
  - arquitectura
  - infraestructura
Topic:
  - Iaas
---

---

## 📚 Idea/Concepto 

Son tres modelos de entrega en la nube que difieren en el nivel de responsabilidad y control que el cliente tiene sobre la infraestructura:

**IaaS (Infrastructure as a Service)**: El proveedor gestiona hardware (servidores, almacenamiento, redes); tú gestionas SO, middleware, aplicaciones.

**PaaS (Platform as a Service)**: El proveedor gestiona infraestructura + SO + middleware; tú gestionas aplicaciones y datos.

**SaaS (Software as a Service)**: El proveedor gestiona todo; tú solo usas la aplicación (Gmail, Salesforce, Teams).

## 📌 Puntos Claves (Opcional)
### IaaS

- Máximo control y flexibilidad
- Ejemplos: AWS EC2, Google Compute Engine, Azure VMs
- Mejor para: Aplicaciones personalizadas, control total necesario
- Responsabilidad: Cliente gestiona aplicaciones, SO, patches

### PaaS

- Balance entre control y facilidad
- Ejemplos: Google App Engine, AWS Elastic Beanstalk, Heroku
- Mejor para: Desarrollo rápido sin gestionar infraestructura
- Responsabilidad: Cliente solo gestiona código y datos

### SaaS

- Mínimo control, máxima facilidad
- Ejemplos: Microsoft 365, Salesforce, Slack, Google Workspace
- Mejor para: Usuarios finales, equipo IT pequeño
- Responsabilidad: El proveedor gestiona casi todo

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[02_Requerimientos/Requerimientos de Negocio]]
- [[04_Implementación/Estándares de Programación]]
## 💡 Personal Insight (Opcional)
- No hay un modelo "mejor" universalmente; depende del caso de uso y capacidades del equipo
- Las organizaciones frecuentemente usan los tres modelos en diferentes áreas: SaaS para colaboración, PaaS para desarrollo ágil, IaaS para cargas especializadas
- El modelo SaaS reduce carga operacional pero reduce flexibilidad; IaaS requiere más expertise pero máxima flexibilidad
- Entender el modelo de responsabilidad compartida en cada uno es crítico para seguridad
## 🧾 Recursos (Opcional)
- [AWS IaaS, PaaS, SaaS Comparison](https://aws.amazon.com/es/types-of-cloud-computing/)
- [Google Cloud Service Models](https://cloud.google.com/docs/cloud-services)
- [Microsoft Azure Service Models](https://azure.microsoft.com/es-es/resources/cloud-computing-dictionary/what-are-iaas-paas-saas/)