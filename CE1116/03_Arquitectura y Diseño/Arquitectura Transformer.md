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

El Transformer procesa secuencias en paralelo mediante Self-Attention, usando Positional Embeddings para preservar el orden. Sus bloques apilan Multi-Head Attention, una FFN (dos proyecciones lineales + activación GELU), Layer Normalization y conexiones residuales. Existen tres variantes: encoder-only (BERT), decoder-only (GPT/LLaMA) y encoder-decoder (T5). El KV-Cache optimiza la inferencia autoregresiva en producción reutilizando cálculos previos.

## 📌 Puntos Claves
- Procesa secuencias en paralelo, sin recurrencia.
- Sus bloques apilan: Multi-Head Attention + FFN + Layer Norm + conexiones residuales.
- Variantes: encoder-only (BERT), decoder-only (GPT), encoder-decoder (T5).
- KV-Cache es clave para inferencia eficiente en producción.

## 🔗 Connections
- [[03_Arquitectura y Diseño/Mecanismo de Atención]]
- [[04_Implementación/Embeddings]]
- [[04_Implementación/Función de Activación]]
- [[04_Implementación/Ventana de Contexto]]
- [[03_Arquitectura y Diseño/Redes Neuronales]]

## 💡 Personal Insight
- La distinción encoder-only vs decoder-only cambia completamente el caso de uso del modelo. BERT entiende, GPT genera.
- El hecho de que no use recurrencia fue el salto que permitió entrenar modelos masivos en paralelo.

## 🧾 Recursos
- Vaswani et al. (2017) - "Attention is All You Need": https://arxiv.org/abs/1706.03762
