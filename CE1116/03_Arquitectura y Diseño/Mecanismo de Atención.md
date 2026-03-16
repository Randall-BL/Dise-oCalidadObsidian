---
Fecha de creación: 2025-03-15 00:00
Fecha de Modificación: 2025-03-15 00:00
tags:
  - ia
  - machine-learning
  - arquitectura
Topic:
  - principios-ia
---

---

## 📚 Idea/Concepto

El mecanismo de atención computa representaciones contextuales mediante la fórmula: Attention(Q,K,V) = softmax(QK^T / √d_k)V, donde Q, K y V son proyecciones lineales de la entrada. El factor √d_k evita la saturación del softmax en alta dimensión. En decoders se usa Masked Self-Attention para impedir que el modelo vea tokens futuros durante la generación autoregresiva. Multi-Head Attention ejecuta h atenciones en paralelo capturando relaciones diversas. Su complejidad O(n²) limita la ventana de contexto.

## 📌 Puntos Claves
- Fórmula: Attention(Q,K,V) = softmax(QK^T / √d_k)V
- Q, K, V son proyecciones lineales de la misma entrada (Self-Attention).
- Masked Self-Attention evita ver tokens futuros en generación autoregresiva.
- Complejidad O(n²) es el cuello de botella que limita la ventana de contexto.

## 🔗 Connections
- [[03_Arquitectura y Diseño/Arquitectura Transformer]]
- [[04_Implementación/Embeddings]]
- [[04_Implementación/Ventana de Contexto]]

## 💡 Personal Insight
- La complejidad O(n²) conecta directamente por qué los LLMs tienen límite de contexto — no es arbitrario, es el costo de que cada token atienda a todos los demás.
- Flash Attention existe precisamente para atacar este cuello de botella sin cambiar el resultado matemático.

## 🧾 Recursos
- Vaswani et al. (2017) - "Attention is All You Need": https://arxiv.org/abs/1706.03762
- Flash Attention: https://arxiv.org/abs/2205.14135
