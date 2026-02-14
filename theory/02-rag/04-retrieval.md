# 04. Estrategias de Recuperación (Retrieval)

## El Problema de la Búsqueda Densa

Los vectores capturan conceptos ("reparar fallo") pero fallan con identificadores exactos ("Error E-25").

## Hybrid Search (Búsqueda Híbrida)

Ejecución paralela de dos estrategias:

1.  **Dense Retrieval (Vectores):** Semántica.
2.  **Sparse Retrieval (BM25/Keywords):** Palabras exactas.

## Reciprocal Rank Fusion (RRF)

Algoritmo para unificar los resultados de la búsqueda híbrida.

$$\text{Score} = \frac{1}{k + \text{rank\_vector}} + \frac{1}{k + \text{rank\_keyword}}$$

Si un documento aparece arriba en ambas listas, su relevancia se dispara.
