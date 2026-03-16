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

La tokenización convierte texto en tokens mapeados a índices enteros dentro de un vocabulario fijo construido con algoritmos como BPE (Byte Pair Encoding) o WordPiece. El vocabulario incluye tokens especiales ([UNK], [CLS], [SEP]) con funciones estructurales. El conteo de tokens determina el uso de la ventana de contexto disponible para el modelo.

## 📌 Puntos Claves
- Los tokens se mapean a índices enteros, no a vectores (eso es embedding).
- Algoritmos de construcción del vocabulario: BPE, WordPiece, SentencePiece.
- Tokens especiales: [UNK] (desconocido), [CLS] (clasificación), [SEP] (separador).
- El tokenizador es específico de cada modelo — no son intercambiables.

## 🔗 Connections
- [[04_Implementación/Embeddings]]
- [[04_Implementación/Ventana de Contexto]]
- [[03_Arquitectura y Diseño/Arquitectura Transformer]]

## 💡 Personal Insight
- El error más común es confundir tokenización con embedding. Son etapas distintas: primero texto → índice (tokenización), luego índice → vector (embedding).
- Un tokenizador entrenado mayormente en inglés es menos eficiente en español — los mismos conceptos requieren más tokens.

## 🧾 Recursos
- Hugging Face Tokenizers docs: https://huggingface.co/docs/tokenizers
