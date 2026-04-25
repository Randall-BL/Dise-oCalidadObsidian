---
Fecha de creación: 2025-08-04 23:53
Fecha de Modificación: 2025-08-04 23:53
tags:
  - cloud
  - infraestructura
  - networking
Topic:
  - VPC
---

---

## 📚 Idea/Concepto 

Una Virtual Private Cloud (VPC) es una sección aislada y privada dentro de un cloud público donde puedes lanzar y configurar tus propios recursos de nube de forma controlada. Es como tener tu propio datacenter virtual dentro de la infraestructura compartida del proveedor. Permite definir rangos de IP, subredes, tablas de ruteo, gateways y controles de acceso.
## 📌 Puntos Claves (Opcional)
- **Aislamiento lógico**: Tus recursos están separados de otros usuarios del cloud público
- **Control de red**: Defines subredes, direccionamiento IP y rutas de tráfico
- **Seguridad granular**: Security groups y network ACLs permiten control fino del acceso
- **Conectividad flexible**: Puedes conectar a tu red on-premises mediante VPN o conexiones dedicadas
- **Multi-región**: Algunas VPCs permiten expandirse a múltiples zonas de disponibilidad

## 🔗 Connections
- [[03_Arquitectura y Diseño/Requerimientos No Funcionales]]
- [[02_Requerimientos/Requerimientos de Sistema]]
- [[02_Requerimientos/Requerimientos Funcionales]]
## 💡 Personal Insight (Opcional)
- Las VPCs son fundamentales para implementar arquitecturas seguras y escalables en el cloud público
- Aunque el cloud público es compartido, una VPC bien configurada proporciona el nivel de aislamiento necesario para cumplir requisitos de seguridad
- Es importante planificar bien el esquema de direccionamiento IP desde el inicio, ya que cambiar esto después es complejo
## 🧾 Recursos (Opcional)
- [AWS VPC Documentation](https://docs.aws.amazon.com/vpc/)
- [Google Cloud VPC Networks](https://cloud.google.com/docs/vpc)
- [Azure Virtual Networks](https://docs.microsoft.com/en-us/azure/virtual-network/)