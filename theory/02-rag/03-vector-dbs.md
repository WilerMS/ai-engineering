# 03. Bases de Datos Vectoriales e Indexación

## Algoritmos de Indexación (ANN)

La búsqueda exacta (KNN) es $O(N)$ e inviable a escala.

### HNSW (Hierarchical Navigable Small World)

El estándar actual. Estructura de grafo multinivel (autopistas vs calles).

- **Latencia:** Milisegundos.
- **Recall:** >95%.

## Stack Tecnológico

### Cloud Native

- **Pinecone:** Serverless, líder de mercado.
- **AWS OpenSearch / Aurora:** Si ya estás en AWS.

### Local / Docker (Recomendado para aprendizaje)

- **Qdrant:** Rust, alto rendimiento.
- **Weaviate:** Go, modular.
- **Chroma:** Simple, Python-native.
