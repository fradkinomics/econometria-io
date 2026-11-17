# Econometría Aplicada a Organización Industrial

Trabajo de **Econometría Aplicada a Organización Industrial** — Maestría en Economía, Universidad de San Andrés (2026).

## Contenido

Estimación de demanda de productos diferenciados con datos de ventas minoristas, desde modelos **logit** hasta el modelo **BLP** (Berry, Levinsohn & Pakes), y simulación de una fusión. El código sigue un pipeline numerado:

| Script | Contenido |
|---|---|
| `01_datos.py` | Armado de la base a partir de `data/TP_data.xlsx` |
| `02`–`04` | Logit por MCO, con efectos fijos de marca y de marca y tienda |
| `05`–`06` | Variables instrumentales (costos e instrumentos de Hausman) |
| `07_elasticidades.py` | Elasticidades del logit |
| `08_datos_blp.py` | Preparación de datos para BLP |
| `09`–`11` | Estimación BLP, sensibilidad, elasticidades y costos marginales |
| `12_fusion.py` | Simulación de la fusión |

## Cómo reproducir

Correr los scripts en orden desde la raíz del proyecto (`python code/01_datos.py`, etc.). Las bases intermedias y `output/` no están en el repositorio por su tamaño: se regeneran al correr el pipeline. La estimación BLP (`09`) tarda varios minutos por especificación.

## Herramientas

Python (pandas, NumPy, statsmodels, linearmodels, PyBLP)

## Estructura del repositorio

- `code/` — pipeline de estimación
- `data/` — datos crudos y documentación de PyBLP
- `notas/` — notas de método
- consigna e informe (PDF)
