Actúa como analista senior de reputación de redes de concesionarios.

Dispones del archivo:

`annex_mitsubishi_top_bottom_drivers.json`

Este archivo contiene el análisis de drivers y barreras de los diez mejores y
diez peores dealers Mitsubishi con al menos 50 reviews durante el periodo
25/12/2025–25/06/2026.

## Reglas obligatorias

1. Utiliza el JSON como fuente canónica.
2. No cambies la fórmula de eNPS.
3. Distingue reviews de menciones o fragmentos.
4. Una mención no equivale necesariamente a una review única.
5. No interpretes una tasa elevada sin mostrar el volumen de menciones.
6. Marca los resultados con menos de 10 menciones como indicativos.
7. Los drivers positivos están ordenados por porcentaje positivo y después por
   volumen.
8. Las barreras negativas están ordenadas por número absoluto de menciones
   negativas y después por porcentaje negativo.
9. No generalices los resultados de estos 20 dealers a los 159 dealers
   Mitsubishi sin comprobarlo.
10. Separa siempre:
    - hechos observados;
    - inferencias;
    - hipótesis;
    - recomendaciones.
11. No inventes causalidad.
12. Indica siempre el periodo, los filtros y el tamaño de muestra.

## Contexto

- Marca: Mitsubishi
- Dealers registrados en la BBDD: 159
- Dealers con actividad: 157
- Dealers con al menos 50 reviews: 23
- Top analizado: 10 dealers
- Bottom analizado: 10 dealers
- Mínimo para categorías y subcategorías: 3 menciones

## Objetivos sugeridos

Analiza:

1. patrones compartidos entre los mejores dealers;
2. patrones compartidos entre los peores dealers;
3. diferencias entre drivers positivos y barreras;
4. dealers que puedan servir como benchmark;
5. dealers que requieran intervención prioritaria;
6. prácticas positivas potencialmente transferibles;
7. problemas operativos recurrentes;
8. posibles líneas de investigación sobre textos originales;
9. recomendaciones de mejora por dealer;
10. recomendaciones transversales para Mitsubishi.

## Priorización recomendada

Para las fortalezas, combina:

- positive_rate;
- mentions_positive;
- mentions_total;
- volumen de reviews del dealer.

Para las barreras, combina:

- mentions_negative;
- negative_rate;
- mentions_total;
- volumen de reviews del dealer;
- total_enps.

No priorices automáticamente una tasa del 100% cuando esté basada en una
muestra pequeña.

## Formato de respuesta recomendado

1. Resumen ejecutivo.
2. Metodología y alcance.
3. Drivers de los mejores dealers.
4. Barreras de los peores dealers.
5. Patrones transversales.
6. Benchmarks.
7. Casos críticos.
8. Matriz de prioridades.
9. Recomendaciones accionables.
10. Limitaciones y siguientes análisis.
