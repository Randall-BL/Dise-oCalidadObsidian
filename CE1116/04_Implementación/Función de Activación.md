---
Fecha de creación: 2025-03-15 00:00
Fecha de Modificación: 2025-03-15 00:00
tags:
  - ia
  - machine-learning
Topic:
  - principios-ia
---

---

## 📚 Idea/Concepto

Las funciones de activación introducen no linealidad en las redes neuronales, permitiéndoles aproximar funciones complejas que una composición lineal no podría capturar. En capas ocultas: GELU y SwiGLU son estándar en Transformers modernos; ReLU es eficiente pero sufre dying ReLU cuando neuronas quedan permanentemente inactivas; Sigmoid y Tanh se saturan causando vanishing gradients. En la capa de salida la función depende de la tarea: Softmax (clasificación multiclase), Sigmoid (binaria), lineal (regresión). La elección también determina la inicialización óptima de pesos: He init para ReLU, Xavier para Tanh/Sigmoid.

## 📌 Puntos Claves
- Sin activación, una red profunda equivale a una sola capa lineal.
- GELU y SwiGLU son las estándar en Transformers modernos.
- ReLU: eficiente pero sufre dying ReLU.
- Sigmoid/Tanh: se saturan → vanishing gradients.
- La función de salida cambia según la tarea: Softmax, Sigmoid o lineal.

## 🔗 Connections
- [[03_Arquitectura y Diseño/Redes Neuronales]]
- [[03_Arquitectura y Diseño/Arquitectura Transformer]]

## 💡 Personal Insight
- La elección de la función de activación no es cosmética — afecta convergencia, inicialización de pesos y el rango de la salida. Es una decisión de diseño real.
- Que GELU sea suave (no tiene el corte duro de ReLU en 0) probablemente ayuda al entrenamiento estable de modelos muy grandes.

## 🧾 Recursos
- Activation Functions overview: https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html
