---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags: 
Topic:
---

---

## 📚 Idea/Concepto 

La redundancia en zona (Zone Redundancy o AZ Redundancy) significa distribuir recursos across múltiples zonas de disponibilidad dentro de la misma región. Cada zona es un datacenter separado con poder, enfriamiento e infraestructura independientes, pero con latencia baja entre ellas. Protege contra el fallo de una zona completa.

## 📌 Puntos Claves (Opcional)
- **Alcance**: Múltiples zonas de disponibilidad en una región
- **Aislamiento**: Las zonas están físicamente separadas pero geográficamente cercanas
- **Latencia moderada**: Más alto que redundancia local pero aún muy bajo (< 10ms típicamente)
- **Protección de AZ**: Si una zona entera falla, la otra continúa operando
- **RTO/RPO muy bajo**: Las réplicas pueden detectarse y redirigir tráfico automáticamente
- **Costo moderado**: Más que redundancia local pero menos que geo-redundancia

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[06_Despliegue e Infraestructura/Azure DevOps]]
- [[07_Mantenimiento/Monitoreo de Aplicación]]
## 💡 Personal Insight (Opcional)
- La redundancia en zona es el estándar recomendado para producción en la mayoría de aplicaciones
- AWS, Google Cloud y Azure están diseñados con múltiples zonas en cada región para facilitar esto
- Distribuir bases de datos entre zonas requiere replicación síncrona (típicamente) para evitar pérdida de datos
- El failover automático entre zonas es crítico; requiere load balancers y health checks configurados adecuadamente
- Algunos proveedores ofrecen servicios administrados (como RDS Multi-AZ) que manejan esto automáticamente
## 🧾 Recursos (Opcional)
- [AWS Availability Zones](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)
- [Google Cloud Zones & Regions](https://cloud.google.com/docs/geography-and-regions#zones)
- [Azure Availability Zones](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview)