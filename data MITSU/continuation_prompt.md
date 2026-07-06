Actúa como analista senior de reputación de retailers y concesionarios.

Dispones de un paquete de datos sobre 211 dealers seleccionados por tener más
de 100 reviews entre el 25/12/2025 y el 25/06/2026.

## Archivos

- README.md
- methodology.md
- data_dictionary.json
- dealers_211.json
- rankings.json
- category_drivers.jsonl
- category_barriers.jsonl
- executive_findings.md
- validation_report.json

## Reglas obligatorias

1. Lee primero `methodology.md` y `data_dictionary.json`.
2. No cambies la fórmula del eNPS.
3. No interpretes valores `null` como cero.
4. Distingue reviews de menciones o fragmentos.
5. No sumes menciones como si fueran personas o reviews únicas.
6. Controla siempre el volumen de muestra.
7. Marca resultados con menos de 10 menciones como indicativos.
8. Prioriza resultados que combinen porcentaje y volumen.
9. Separa claramente:
   - hechos observados;
   - inferencias;
   - hipótesis;
   - recomendaciones.
10. No inventes causalidad.
11. No generalices los drivers del top 10 o las barreras del bottom 10 a los
    211 dealers sin comprobarlo.
12. Cuando compares marcas o regiones, utiliza agregaciones ponderadas por
    volumen de reviews y muestra también el número de dealers.
13. Cuando analices categorías, utiliza menciones totales, positivas, negativas
    y sus porcentajes.
14. Indica siempre el periodo y los filtros aplicados.
15. Señala cualquier anomalía o inconsistencia antes de elaborar conclusiones.

## Definición de eNPS

eNPS = 100 × (reviews de 5 estrellas − reviews de 1, 2 y 3 estrellas)
       / total de reviews

Las reviews de 4 estrellas son pasivas, pero forman parte del denominador.

## Objetivo principal

Preparar un informe ejecutivo y accionable que incluya:

1. distribución general del eNPS;
2. mejores y peores dealers;
3. análisis por marca;
4. análisis por región y ciudad;
5. comparación entre Sales y After Sales;
6. drivers reputacionales;
7. barreras reputacionales;
8. dealers benchmark;
9. dealers críticos;
10. patrones transversales;
11. oportunidades operativas;
12. recomendaciones priorizadas;
13. limitaciones metodológicas.

## Análisis sugeridos

### Panorama general

- media, mediana, mínimo y máximo de eNPS;
- percentiles;
- distribución por tramos;
- relación entre volumen de reviews y eNPS;
- relación entre valoración media y eNPS.

### Marca y región

- eNPS ponderado por marca;
- eNPS mediano por marca;
- dispersión entre dealers;
- porcentaje de dealers por debajo de determinados umbrales;
- regiones con mayor consistencia;
- regiones con mayor riesgo.

### Sales frente a After Sales

- diferencia entre eNPS Sales y After Sales;
- dealers con mayor brecha;
- marcas con problemas concentrados en posventa;
- casos donde el total oculta un área crítica.

### Drivers y barreras

- frecuencia transversal de cada categoría;
- frecuencia transversal de cada subcategoría;
- volumen de menciones;
- tasa positiva o negativa;
- combinación de severidad y volumen;
- diferencias entre dealers top y bottom.

### Priorización

Construye una matriz que combine:

- impacto reputacional;
- volumen;
- severidad;
- recurrencia;
- capacidad de actuación.

## Formato esperado del informe

1. Resumen ejecutivo.
2. Metodología.
3. Panorama de los 211 dealers.
4. Rankings.
5. Comparativa por marca y región.
6. Análisis Sales vs. After Sales.
7. Drivers.
8. Barreras.
9. Casos benchmark.
10. Casos críticos.
11. Recomendaciones priorizadas.
12. Limitaciones.
13. Anexo de datos.

Antes de redactar el informe final, presenta una lista breve de controles de
calidad realizados y cualquier supuesto necesario.
