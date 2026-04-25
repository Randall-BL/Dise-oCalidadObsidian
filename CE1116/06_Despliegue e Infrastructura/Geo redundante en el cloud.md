---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags:
  - cloud
  - redundancia
  - alta-disponibilidad
Topic:
  - Cloud Público
  - Cloud Hibridio
---

---

## 📚 Idea/Concepto 

La geo-redundancia (o disaster recovery) implica replicar y distribuir recursos across múltiples regiones geográficamente separadas. Una región típicamente contiene múltiples zonas de disponibilidad en una área geográfica amplia (ej: us-east-1 en Virginia). Protege contra desastres que afecten una región completa (huracanes, terremotos, interrupciones eléctricas masivas).

## 📌 Puntos Claves (Opcional)
- **Alcance**: Múltiples regiones geográficamente distantes
- **Separación física**: Cientos a miles de kilómetros de distancia
- **Latencia mayor**: 50-200ms típicamente entre regiones
- **Disaster Recovery**: Protege contra fallos catastróficos de región completa
- **Complejidad aumentada**: Requiere sincronización de datos, redireccionamiento de tráfico
- **Costo significativo**: Duplica la infraestructura en múltiples regiones
- **RTO/RPO variable**: Depende de la estrategia (active-passive vs active-active)

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Negocio]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[06_Despliegue e Infraestructura/Azure DevOps]]
- [[07_Mantenimiento/Monitoreo de Aplicación]]
## 💡 Personal Insight (Opcional)
- La geo-redundancia es esencial solo para aplicaciones misión-críticas con requisitos SLA muy estrictos
- El desafío principal es mantener datos consistentes entre regiones sin que la latencia impacte el rendimiento
- Existen dos estrategias principales:
    - **Active-Passive**: Una región recibe todo el tráfico; la otra es backup (más simple, RTO mayor)
    - **Active-Active**: Ambas regiones procesan tráfico; requiere sincronización más compleja (más caro, RTO menor)
- Los proveedores ofrecen servicios administrados para facilitar esto (ej: DynamoDB Global Tables en AWS)
## 🧾 Recursos (Opcional)
- [AWS Global Infrastructure & Regions](https://aws.amazon.com/about-aws/global-infrastructure/)
- [Google Cloud Regions & Multi-region](https://cloud.google.com/docs/geography-and-regions)
- [Azure Regions & Paired Regions](https://docs.microsoft.com/en-us/azure/availability-zones/cross-region-replication-azure)