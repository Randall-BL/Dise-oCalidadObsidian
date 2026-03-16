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

Los embeddings son vectores densos aprendidos durante el entrenamiento que representan tokens u otras entidades en un espacio de dimensión fija. En Transformers, Token Embeddings se suman con Positional Embeddings para formar la entrada al modelo. Los embeddings estáticos (Word2Vec) asignan un vector fijo por token; los contextuales (BERT, GPT) generan vectores que varían según el contexto. La similitud coseno entre vectores mide cercanía semántica y es la base de búsqueda semántica y RAG.

## 📌 Puntos Claves
- Token Embeddings + Positional Embeddings = entrada al Transformer.
- Estáticos (Word2Vec): un vector fijo por token.
- Contextuales (BERT, GPT): el vector cambia según el contexto de la oración.
- Similitud coseno permite búsqueda semántica y es la base de RAG.

## 🔗 Connections
- [[04_Implementación/Tokenización]]
- [[03_Arquitectura y Diseño/Mecanismo de Atención]]
- [[03_Arquitectura y Diseño/Arquitectura Transformer]]
- [[04_Implementación/Ventana de Contexto]]

## 💡 Personal Insight
- Los Positional Embeddings son lo que le da al Transformer noción de orden sin usar recurrencia — es una solución elegante a un problema fundamental.
- RAG es básicamente búsqueda por similitud coseno entre embeddings; entender embeddings es entender cómo funciona la memoria externa de los LLMs.

## 🧾 Recursos
- Word2Vec paper: https://arxiv.org/abs/1301.3781
- Hugging Face Embeddings: https://huggingface.co/blog/getting-started-with-embeddings
