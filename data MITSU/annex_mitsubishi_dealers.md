# Anexo — Métricas de los dealers Mitsubishi

## 1. Alcance

Este anexo contiene las métricas de todos los dealers asociados a Mitsubishi
en la base de datos.

Periodo analizado:

- Desde: 25 de diciembre de 2025
- Hasta: 25 de junio de 2026
- Ambas fechas incluidas

Universo:

- 159 dealers registrados
- 157 dealers con al menos una review
- 2 dealers sin reviews durante el periodo

Dealers sin actividad:

- DWINDO - CAKUNG (100703)
- MAHLIGAI - SUKABUMI (100685)

## 2. Resumen de la marca

| Ámbito | Reviews | Valoración media | eNPS |
|---|---:|---:|---:|
| Total | 4.512 | 4,691 | 81,60 |
| Sales | 496 | 4,546 | 75,40 |
| After Sales | 1.792 | 4,613 | 78,35 |

## 3. Metodología

El eNPS se calcula mediante la fórmula:

`eNPS = 100 × (5★ − 1★ − 2★ − 3★) / total de reviews`

Las reviews de 4 estrellas se consideran pasivas:

- no suman como promotoras;
- no restan como detractoras;
- forman parte del denominador.

Cuando no existen reviews en un ámbito:

- el volumen se representa como 0;
- la valoración media se representa como null;
- el eNPS se representa como null.

El eNPS Total incluye:

- Sales;
- After Sales;
- reviews sin clasificación de área.

## 4. Estructura del archivo detallado

El archivo `annex_mitsubishi_dealers.csv` contiene una fila por dealer y las
siguientes métricas:

- número de reviews totales;
- valoración media total;
- eNPS total;
- número de reviews Sales;
- valoración media Sales;
- eNPS Sales;
- número de reviews After Sales;
- valoración media After Sales;
- eNPS After Sales.

## 5. Lectura ejecutiva

A nivel agregado, Mitsubishi presenta:

- eNPS total de 81,60;
- eNPS Sales de 75,40;
- eNPS After Sales de 78,35.

After Sales presenta un resultado superior a Sales en 2,95 puntos de eNPS,
aunque ambos quedan por debajo del contexto global de la BBDD:

- eNPS global Total: 88,95;
- eNPS global Sales: 87,13;
- eNPS global After Sales: 86,53.

Por tanto, Mitsubishi se sitúa:

- 7,35 puntos por debajo del contexto global en Total;
- 11,73 puntos por debajo en Sales;
- 8,18 puntos por debajo en After Sales.

## 6. Dealers con mayor volumen

Entre los dealers con mayor número de reviews del periodo se encuentran:

- DIPO - PURI: 269 reviews;
- DIPO - PLUIT: 164 reviews;
- SUN - BLITAR: 160 reviews;
- SUN - A. YANI: 158 reviews;
- MUSTIKA - CIBUBUR: 142 reviews;
- SDM - MARGONDA: 127 reviews;
- SUN - PROBOLINGGO: 124 reviews;
- SUN - PURWOKERTO: 124 reviews;
- SARDANA - GATSU (MEDAN): 119 reviews;
- SUN - MALANG: 117 reviews.

Estos dealers deben tener más peso en la interpretación de los resultados de
la marca que los dealers con una o dos reviews.

## 7. Señales positivas con volumen relevante

Algunos resultados destacados son:

- SUN - PROBOLINGGO:
  - 124 reviews;
  - valoración media 5,000;
  - eNPS total 100;
  - eNPS Sales 100;
  - eNPS After Sales 100.

- SUN - BLITAR:
  - 160 reviews;
  - valoración media 4,981;
  - eNPS total 98,13;
  - eNPS After Sales 97,94.

- SDM - MARGONDA:
  - 127 reviews;
  - valoración media 4,953;
  - eNPS total 96,85;
  - eNPS Sales 95,24;
  - eNPS After Sales 100.

- DIPO - PLUIT:
  - 164 reviews;
  - valoración media 4,921;
  - eNPS total 95,73;
  - eNPS After Sales 96,40.

- SUN - A. YANI:
  - 158 reviews;
  - valoración media 4,930;
  - eNPS total 95,57;
  - eNPS After Sales 92,31.

## 8. Señales negativas

Los dealers con resultado total negativo son:

- SPS - INDRAMAYU:
  - 1 review;
  - eNPS -100;
  - muestra no representativa.

- SUN - BANYUMANIK:
  - 2 reviews;
  - eNPS -100;
  - muestra no representativa.

- SDIM - PALANGKARAYA:
  - 4 reviews;
  - eNPS -50;
  - After Sales -100 sobre 2 reviews.

- AIPO - PALEMBANG:
  - 3 reviews;
  - eNPS -33,33;
  - After Sales -100 sobre 2 reviews.

- BRA - SIDOARJO:
  - 3 reviews;
  - eNPS -33,33;
  - Sales y After Sales -100 sobre una review en cada área.

- GBI - PONTIANAK A.YANI:
  - 3 reviews;
  - eNPS -33,33;
  - Sales y After Sales -100 sobre una review en cada área.

Los porcentajes extremos de estos dealers deben interpretarse con cautela por
el reducido tamaño de muestra.

## 9. Casos de atención con mayor volumen

Los resultados más relevantes desde una perspectiva operativa no son
necesariamente los eNPS más bajos, sino aquellos que combinan una valoración
débil con un volumen suficiente.

Ejemplos:

### BRA - IMAM BONJOL

- 61 reviews;
- media 3,557;
- eNPS total 21,31;
- After Sales:
  - 30 reviews;
  - media 2,700;
  - eNPS -20,00.

### BRA - SEMARANG

- 32 reviews;
- media 3,625;
- eNPS total 25,00;
- After Sales:
  - 13 reviews;
  - media 2,462;
  - eNPS -30,77.

### SDM - BANDUNG

- 25 reviews;
- media 3,840;
- eNPS total 20,00;
- After Sales:
  - 8 reviews;
  - media 2,375;
  - eNPS -75,00.

### SUN - YASMIN

- 14 reviews;
- media 3,500;
- eNPS total 0,00;
- After Sales:
  - 6 reviews;
  - media 2,500;
  - eNPS -50,00.

### SUN - CIBINONG

- 11 reviews;
- media 3,545;
- eNPS total 27,27;
- Sales eNPS 0;
- After Sales eNPS 0.

## 10. Precauciones analíticas

- No comparar dealers sin controlar el número de reviews.
- Los resultados con menos de 10 reviews deben tratarse como indicativos.
- Un eNPS extremo con una review no equivale a un problema estructural.
- Las métricas totales pueden incluir reviews sin clasificación de área.
- Sales y After Sales no siempre suman el total.
- Las medias y los eNPS de la marca deben calcularse agregando reviews, no
  promediando dealers.
