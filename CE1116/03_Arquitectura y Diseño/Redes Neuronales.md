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

Una red neuronal es un modelo de capas de neuronas donde cada una computa salida = f(Wx + b). El aprendizaje usa backpropagation y optimizadores como Adam para actualizar pesos minimizando el error. Las redes profundas sufren vanishing gradients, problema resuelto con conexiones residuales y normalización. Arquitecturas comunes: MLP, CNN, RNN y Transformer.

## 📌 Puntos Claves
- Cada neurona computa: salida = f(Wx + b).
- Aprende mediante backpropagation + optimizadores como Adam.
- Vanishing gradients es el problema central en redes profundas.
- Conexiones residuales y Layer Norm son las soluciones modernas.

## 🔗 Connections
- [[03_Arquitectura y Diseño/Arquitectura Transformer]]
- [[03_Arquitectura y Diseño/Mecanismo de Atención]]
- [[04_Implementación/Función de Activación]]
- [[04_Implementación/Embeddings]]

## 💡 Personal Insight
- Entender f(Wx + b) como la operación base de toda la IA moderna cambia cómo se piensa en los modelos — todo es álgebra lineal + no linealidad.
- El problema de vanishing gradients explica directamente por qué existe el Transformer.

## 🧾 Recursos
- Deep Learning Book - Goodfellow et al.: https://www.deeplearningbook.org
