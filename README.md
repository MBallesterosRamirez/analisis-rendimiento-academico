# Análisis de Rendimiento Académico

Análisis de datos académicos con Python para identificar patrones de rendimiento estudiantil en la Institución Madeg

## Descripción del proyecto

Este proyecto tiene como objetivo analizar el rendimiento académico de estudiantes de grado 10, utilizando datos reales anonimizados provenientes de una institución educativa.

Se busca identificar patrones de desempeño académico y construir una base para futuros modelos predictivos que permitan anticipar resultados y apoyar la toma de decisiones.

---

## Fuente de los datos

Los datos fueron extraídos de una plataforma educativa institucional.

Para garantizar la privacidad:

* Se eliminaron datos sensibles
* Se trabajó con información anonimizada

---

## Proceso de limpieza de datos

Se realizó un proceso completo de limpieza y preparación:

1. Eliminación de filas irrelevantes (títulos, encabezados duplicados)
2. Estandarización de nombres de columnas:

   * Conversión a minúsculas
   * Eliminación de tildes
   * Reemplazo de espacios por guion bajo (_)
3. Eliminación de columnas vacías o innecesarias
4. Validación de tipos de datos (`df.info()`)
5. Validación estadística (`df.describe()`)
6. Identificación de valores faltantes

---

## Transformación de datos

1. Separación de la variable de convivencia (datos categóricos)
2. Creación de dos datasets:

   * `datos_notas.csv`
   * `datos_convivencia.csv`
3. Transformación de formato ancho a formato largo (`melt`)
4. Separación de variables:

   * asignatura
   * tipo (jv1, acumulado)
5. Reconstrucción del dataset usando `pivot_table`

---

## Dataset final

El dataset final contiene:

* 496 registros
* Variables:

  * código
  * estudiante (anonimizado)
  * asignatura
  * jv1 (nota del periodo)
  * acumulado (promedio del periodo)

Cada fila representa el desempeño de un estudiante en una asignatura específica.

---

## Objetivo analítico

Este proyecto permite:

* Identificar asignaturas con mayor dificultad
* Analizar el rendimiento por estudiante
* Comparar desempeño entre asignaturas
* Sentar bases para predicción de notas futuras

---

## ⚙️ Tecnologías utilizadas

* Python
* Pandas
* Google Colab
* Excel

---

## Próximos pasos

* Identificación de estudiantes en riesgo académico
* Análisis comparativo entre periodos
* Modelo de predicción de rendimiento académico

---

## Autor

Proyecto desarrollado por Ing. Mauricio Ballesteros
Ingeniero de Sistemas | Docente de Tecnología y Programación

