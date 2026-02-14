# 05. RAG Avanzado (Optimización)

## Pre-Retrieval: Query Transformation

El usuario no siempre sabe preguntar bien.

- **HyDE (Hypothetical Document Embeddings):** Generar una respuesta falsa ideal, vectorizarla y buscar documentos reales similares a ella.
- **Multi-Query:** Generar 3 variaciones de la pregunta para cubrir más espacio semántico.

## Post-Retrieval: Reranking (Two-Stage)

El patrón de oro para precisión.

1.  **Stage 1 (Retrieval):** Embeddings (Bi-Encoder). Rápido. Recupera Top-50.
2.  **Stage 2 (Reranking):** Cross-Encoder. Lento y preciso. Lee pregunta+documento a la vez. Reordena y selecciona Top-3.
