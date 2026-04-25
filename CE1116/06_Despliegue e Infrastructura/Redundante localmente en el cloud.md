---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags:
  - cloud
  - redundancia
  - alta-disponibilidad
  - infraestructura
Topic:
  - Cloud Público
  - Cloud Hibridio
---

---

## 📚 Idea/Concepto 

La redundancia local en el cloud implica replicar y distribuir recursos dentro de una misma zona de disponibilidad (AZ - Availability Zone) o región. Garantiza que si una instancia o componente falla, otras copias están disponibles inmediatamente para asumir la carga, sin cambio geográfico.

## 📌 Puntos Claves (Opcional)
- **Alcance**: Dentro de una sola zona de disponibilidad o región
- **Latencia baja**: Comunicación entre réplicas es muy rápida
- **Protección contra fallos hardware**: Si un servidor falla, otros asumen la carga
- **Load balancing**: Distribuye tráfico entre múltiples instancias
- **RTO/RPO muy bajo**: Recovery Time Objective y Recovery Point Objective mínimos
- **Costo moderado**: Más barato que geo-redundancia pero hay costo de réplicas

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[06_Despliegue e Infraestructura/Azure DevOps]]
- [[07_Mantenimiento/Monitoreo de Aplicación]]
## 💡 Personal Insight (Opcional)
- La redundancia local es la base de cualquier arquitectura de alta disponibilidad en el cloud
- Usar load balancers y health checks es crítico: el load balancer debe detectar instancias no disponibles rápidamente
- Aunque proporciona protección contra fallos de hardware, no protege contra fallos de toda la zona de disponibilidad
- Para aplicaciones críticas, combina redundancia local con geo-redundancia para máxima protección
## 🧾 Recursos (Opcional)
- [AWS Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing/)
- [Google Cloud Load Balancing](https://cloud.google.com/load-balancing)
- [Azure Load Balancer](https://docs.microsoft.com/en-us/azure/load-balancer/)