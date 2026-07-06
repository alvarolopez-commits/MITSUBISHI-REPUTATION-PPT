# Metodología

## 1. Periodo analizado

- Fecha inicial: 2025-12-25
- Fecha final: 2026-06-25
- Ambas fechas están incluidas.

## 2. Selección de dealers

Se seleccionaron los dealers con más de 100 reviews publicadas dentro del
periodo.

Total resultante: 211 dealers.

## 3. Fórmula de eNPS basada en estrellas

eNPS = 100 × (R5 − R1 − R2 − R3) / Rtotal

Donde:

- R1: reviews de 1 estrella.
- R2: reviews de 2 estrellas.
- R3: reviews de 3 estrellas.
- R5: reviews de 5 estrellas.
- Rtotal: total de reviews del universo correspondiente.

Las reviews de 4 estrellas son pasivas:

- no se suman como promotoras;
- no se restan como detractoras;
- sí forman parte del denominador.

## 4. Ámbitos del eNPS

### eNPS total

Incluye todas las reviews:

- Sales;
- After Sales;
- Unclassified.

### eNPS Sales

Incluye exclusivamente reviews clasificadas como `sales`.

### eNPS After Sales

Incluye exclusivamente reviews clasificadas como `after-sales`.

Cuando no existen reviews en un área, el eNPS se representa como `null`.
Nunca debe interpretarse `null` como cero.

## 5. Advertencia conceptual

El indicador se denomina eNPS en este análisis, pero no es el Employee Net
Promoter Score tradicional obtenido mediante una pregunta de recomendación a
empleados.

Es una adaptación calculada a partir de las estrellas de las reviews.

## 6. Categorías y subcategorías

Una mención equivale a un fragmento de texto categorizado dentro de una review.

Cada fragmento puede contener:

- categoría;
- subcategoría;
- sentimiento positivo, negativo u otro estado disponible.

Una misma review puede generar más de un fragmento y, por tanto, más de una
mención.

## 7. Drivers positivos

Indicador:

positive_rate = positive_mentions / total_mentions × 100

Condición aplicada:

- al menos 3 menciones totales.

Ordenación:

1. mayor porcentaje positivo;
2. en caso de empate, mayor volumen de menciones;
3. si continúa el empate, orden de la taxonomía de la base de datos.

Se conservaron las dos mejores categorías y las dos mejores subcategorías de
cada dealer del top 10.

## 8. Barreras reputacionales

Condición aplicada:

- más de 3 menciones totales;
- equivale a un mínimo efectivo de 4 menciones.

Ordenación:

1. mayor número absoluto de menciones negativas;
2. en caso de empate, mayor porcentaje negativo;
3. si continúa el empate, mayor volumen total.

negative_rate = negative_mentions / total_mentions × 100

Se conservaron las dos categorías y las dos subcategorías con mayor influencia
negativa para cada dealer del bottom 10.

## 9. Rankings

### Mejores dealers

Orden descendente por eNPS total.

### Peores dealers

Orden ascendente por eNPS total.

Cuando dos valores redondeados coinciden, debe utilizarse el valor calculado
sin redondear.

## 10. Precauciones analíticas

- No comparar porcentajes sin observar el volumen de menciones.
- Resultados basados en menos de 10 menciones deben considerarse indicativos.
- No atribuir causalidad únicamente por coexistencia de una barrera y un eNPS
  bajo.
- Separar siempre hechos observados, inferencias e hipótesis.
- No sumar menciones como si fueran reviews únicas.
