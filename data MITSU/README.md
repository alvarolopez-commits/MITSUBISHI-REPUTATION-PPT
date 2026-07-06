# Retail Reputation — 211 Dealers

Paquete de conocimiento para continuar el análisis en ChatGPT, Claude, Gemini
u otra herramienta de IA.

## Alcance

- Periodo: 2025-12-25 a 2026-06-25, ambos inclusive.
- Universo: 211 dealers.
- Criterio de selección: más de 100 reviews publicadas durante el periodo.
- Métricas disponibles:
  - volumen de reviews;
  - valoración media;
  - distribución de 1 a 5 estrellas;
  - volumen y distribución de Sales;
  - volumen y distribución de After Sales;
  - reviews sin clasificar;
  - eNPS total, Sales y After Sales.

## Análisis cualitativo disponible

El análisis detallado de categorías y subcategorías cubre:

- los 10 dealers con mejor eNPS total;
- los 10 dealers con peor eNPS total.

No se ha calculado todavía el ranking de drivers y barreras para los 191
dealers restantes.

## Archivos

- `dealers_211.json`: base canónica de métricas por dealer.
- `methodology.md`: fórmulas, filtros y criterios de ordenación.
- `data_dictionary.json`: definición de campos.
- `rankings.json`: top 10 y bottom 10 por eNPS total.
- `category_drivers.jsonl`: principales drivers positivos.
- `category_barriers.jsonl`: principales barreras reputacionales.
- `executive_findings.md`: conclusiones observadas.
- `validation_report.json`: estado de validación y advertencias.
- `continuation_prompt.md`: instrucciones para continuar en otra IA.

## Recomendación de carga en otra IA

Adjuntar primero:

1. `README.md`
2. `methodology.md`
3. `data_dictionary.json`
4. `dealers_211.json`
5. `category_drivers.jsonl`
6. `category_barriers.jsonl`
7. `rankings.json`
8. `executive_findings.md`
9. `validation_report.json`

Después, pegar el contenido de `continuation_prompt.md`.
