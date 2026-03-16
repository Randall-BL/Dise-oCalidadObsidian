---
Fecha de creación: 2025-03-15 00:00
Fecha de Modificación: 2025-03-15 00:00
tags:
  - ia
  - machine-learning
  - nlp
Topic:
  - principios-ia
---

---

## 📚 Idea/Concepto

La ventana de contexto es el número máximo de tokens que un Transformer puede procesar simultáneamente, limitado por la complejidad O(n²) del Self-Attention en memoria y cómputo. Abarca tanto el prompt de entrada como la respuesta generada. Ventanas más largas aumentan el costo computacional y el consumo de VRAM del KV-Cache. Para textos que superan el límite se aplican estrategias como RAG o chunking con solapamiento. Limitación real: el "lost-in-the-middle" problem — los modelos tienden a atender mejor el inicio y el final del contexto, independientemente del tamaño de la ventana.

## 📌 Puntos Claves
- Limitado por la complejidad O(n²) del Self-Attention.
- Incluye prompt + respuesta generada.
- KV-Cache crece en VRAM linealmente con la longitud del contexto.
- Estrategias para textos largos: RAG, chunking con solapamiento.
- "Lost-in-the-middle": más contexto no garantiza mejor uso de toda la información.

## 🔗 Connections
- [[03_Arquitectura y Diseño/Mecanismo de Atención]]
- [[04_Implementación/Tokenización]]
- [[05_Pruebas/Alucinaciones]]
- [[04_Implementación/Embeddings]]

## 💡 Personal Insight
- El "lost-in-the-middle" problem es contraintuitivo: darle más contexto al modelo no siempre mejora la respuesta si la información clave queda enterrada en el medio.
- En producción, el tamaño de la ventana de contexto impacta directamente el costo por query — no es solo un límite técnico, es un factor de negocio.

## 🧾 Recursos
- Lost in the Middle paper: https://arxiv.org/abs/2307.03172
