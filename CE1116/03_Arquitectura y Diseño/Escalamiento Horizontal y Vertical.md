---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags:
  - cloud
  - escalamiento
  - arquitectura
Topic:
  - Escalamiento horizontal y vertical
---

---

## 📚 Idea/Concepto 

El escalamiento en el cloud se refiere a la capacidad de aumentar recursos para manejar más carga. Existen dos enfoques principales:

**Escalamiento Vertical**: Aumentar la capacidad de una máquina individual (más CPU, RAM, almacenamiento).

**Escalamiento Horizontal**: Agregar más máquinas/instancias al sistema distribuyendo la carga entre ellas.

## 📌 Puntos Claves (Opcional)
### Escalamiento Vertical

- **Upgrade de recursos**: Cambiar a instancias más potentes
- **Downtime**: Generalmente requiere parar la instancia actual
- **Límite físico**: Existe un máximo de recursos por máquina
- **Simpler operativamente**: Menos componentes para gestionar

### Escalamiento Horizontal

- **Agregar instancias**: Distribuir carga entre múltiples máquinas
- **Sin downtime**: Se pueden agregar nuevas instancias sin parar las actuales
- **Escalabilidad teórica infinita**: Puedes agregar tantas instancias como necesites
- **Requiere load balancing**: Necesitas distribuir el tráfico entre instancias
- **Más complejo operativamente**: Requiere orquestación y sincronización

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[02_Requerimientos/Requerimientos Funcionales]]
- [[01_Procesos de Desarrollo/Product Owner]]
## 💡 Personal Insight (Opcional)
- El escalamiento horizontal es generalmente preferido en arquitecturas cloud modernas porque proporciona mayor resiliencia y flexibilidad
- El escalamiento vertical es útil para aplicaciones monolíticas o que requieren acceso a recursos en una sola máquina (como bases de datos tradicionales)
- Las arquitecturas bien diseñadas suelen usar ambos: escalamiento vertical para máquinas base y horizontal para manejar picos de demanda
- El auto-scaling basado en métricas (CPU, memoria, tráfico) es una capacidad clave del cloud que automatiza estas decisiones
## 🧾 Recursos (Opcional)
- [AWS Auto Scaling](https://aws.amazon.com/autoscaling/)
- [Google Cloud Scaling & Load Balancing](https://cloud.google.com/docs/load-balancing)
- [Azure Virtual Machine Scale Sets](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/)