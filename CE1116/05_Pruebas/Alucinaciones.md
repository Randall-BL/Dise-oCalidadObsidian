---
Fecha de creación: 2025-03-15 00:00
Fecha de Modificación: 2025-03-15 00:00
tags:
  - ia
  - machine-learning
  - calidad
Topic:
  - principios-ia
---

---

## 📚 Idea/Concepto

Las alucinaciones son respuestas falsas generadas por un LLM con aparente confianza, causadas por generación autoregresiva sin verificación factual nativa y sesgos del corpus de entrenamiento. Se clasifican en tres tipos: factuales (datos incorrectos), de razonamiento (inferencias erróneas) y de fuente (citas inventadas). Caso especial: sycophancy, donde el modelo confirma afirmaciones falsas del usuario optimizando su aprobación. Estrategias de mitigación: RAG para anclar respuestas en documentos reales, temperatura baja y prompts que soliciten incertidumbre explícita.

## 📌 Puntos Claves
- Tipos: factual, de razonamiento, de fuente.
- Causa estructural: generación autoregresiva sin mecanismo nativo de verificación.
- Sycophancy: el modelo confirma lo que el usuario quiere escuchar.
- Mitigaciones: RAG, temperatura baja, prompts que pidan incertidumbre.
- RLHF mal calibrado puede aumentar confianza en respuestas incorrectas.

## 🔗 Connections
- [[04_Implementación/Ventana de Contexto]]
- [[03_Arquitectura y Diseño/Mecanismo de Atención]]
- [[04_Implementación/Tokenización]]
- [[05_Pruebas/Pruebas Funcionales]]

## 💡 Personal Insight
- El sycophancy es especialmente peligroso en producción: el modelo te dice lo que querés escuchar, no lo que es correcto. Diseñar prompts que inviten al modelo a expresar incertidumbre es una práctica de ingeniería real.
- Las alucinaciones no son bugs — son consecuencias predecibles de cómo funciona la generación autoregresiva. Conocer la causa ayuda a diseñar sistemas más robustos.

## 🧾 Recursos
- TruthfulQA benchmark: https://arxiv.org/abs/2109.07958
- Survey on Hallucination in LLMs: https://arxiv.org/abs/2309.01219
