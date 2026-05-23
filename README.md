# IELE756
#IELE756
**Team members**: Ja Ming Louie , Jose Thomas Hechenleitner
**Comunas**: Providencia, San Miguel, Paine
**Date**: 05 de marzo, 2026
**Descripción del Proyecto**:

# Proyecto Final — IELE756  
## Análisis de anomalía epidemiológica y hospitalaria en la comuna de Paine

---

# Objetivo del Proyecto

El objetivo de este proyecto es investigar una anomalía observada en la comuna de Paine, donde se identifica simultáneamente:

- Baja tasa de Enfermedades de Notificación Obligatoria (ENO)
- Alta tasa de hospitalización GRD
- Alta razón de dependencia demográfica

El análisis busca comprender por qué Paine rompe el patrón esperado entre vigilancia epidemiológica y utilización hospitalaria, utilizando información integrada proveniente de bases ENO, GRD y CENSO mediante técnicas de análisis exploratorio, visualización y modelamiento estadístico.

---

# Contexto

Durante el desarrollo de las Tareas 1, 2 y 3 del curso, se detectó que Paine presentaba un comportamiento atípico respecto de otras comunas de la Región Metropolitana.

Mientras variables demográficas como envejecimiento y dependencia poblacional sugieren una alta carga sanitaria, la comuna presenta:

- Baja tasa ENO
- Alta utilización hospitalaria (GRD)

Esto sugiere un desacople entre vigilancia epidemiológica y carga hospitalaria efectiva.

---

# Datos Utilizados

## Bases de datos

- **CENSO**  
  Información demográfica y población comunal.

- **ENO**  
  Base nacional de Enfermedades de Notificación Obligatoria.

- **GRD**  
  Base nacional de Altas Hospitalarias GRD (2022–2024).

---

# Comunas Analizadas

## Comunas principales

- Providencia
- San Miguel
- Paine

## Comunas comparativas

- La Pintana
- Calera de Tango
- San José de Maipo
- San Ramón

---

# Metodología

## 1. Limpieza y preparación de datos

Se realizó:

- Filtrado comunal
- Estandarización de códigos
- Manejo de valores desconocidos
- Validación de calidad de datos
- Integración ENO + GRD + CENSO

### Limitaciones importantes detectadas

- Aproximadamente 45% de ENO posee comuna anonimizada (`*****`)
- Existencia de registros con nacionalidad desconocida

---

## 2. Construcción de indicadores

Se calcularon:

- Tasa ENO por 10.000 habitantes
- Tasa GRD por 10.000 habitantes
- Razón de dependencia
- Índice de subdetección (GRD / ENO)
- Mortalidad intrahospitalaria
- Severidad GRD
- Length of Stay (LOS)

---

## 3. Visualización y análisis exploratorio

Se realizaron:

- Gráficos comparativos
- Scatter plots
- Rankings
- Z-scores
- Modelos de regresión lineal
- Análisis de residuos
- Comparación de diagnósticos CIE-10
- Comparación de especialidades médicas

---

# Principales Hallazgos

## Anomalía principal de Paine

Paine presenta simultáneamente:

- Baja tasa ENO
- Alta tasa GRD
- Alta razón de dependencia

Esto sugiere:

- Posible subdetección epidemiológica
- Atención tardía
- Mayor gravedad al momento de hospitalización
- Barreras de acceso o resolución primaria

---

## Índice de subdetección

Paine obtuvo uno de los índices GRD/ENO más altos del análisis, reforzando la hipótesis de subregistro epidemiológico o diagnóstico tardío.

---

## Resultados estadísticos

Los modelos muestran que:

- Paine posee menos ENO de lo esperado según su perfil demográfico
- Paine presenta más GRD de lo esperado según edad y dependencia

Esto refuerza su comportamiento como *outlier* sanitario.

---

# Resultados Clínicos Relevantes

## Diagnósticos predominantes en Paine

Los capítulos CIE-10 más frecuentes fueron:

- Enfermedades digestivas
- Embarazo, parto y puerperio
- Traumatismos
- Enfermedades respiratorias

---

## Mortalidad intrahospitalaria

Paine presentó la mayor tasa de mortalidad intrahospitalaria entre las comunas analizadas.

---

# Limitaciones

- Tamaño reducido de comunas comparativas
- Alta anonimización ENO
- Variables censales parcialmente aproximadas
- Modelos estadísticos exploratorios y no causales
- Posibles diferencias territoriales de acceso hospitalario

---

# Conclusiones

Los resultados sugieren que Paine presenta una desconexión relevante entre vigilancia epidemiológica y carga hospitalaria efectiva.

La combinación de:

- Baja notificación ENO
- Alta hospitalización
- Alta dependencia demográfica
- Alta mortalidad intrahospitalaria

apunta a posibles problemas de acceso temprano, detección oportuna y resolución preventiva.

El proyecto demuestra cómo la integración de múltiples fuentes de datos puede identificar anomalías territoriales relevantes para salud pública.

---

# Declaración de Uso de IA

Este proyecto utilizó herramientas de inteligencia artificial como apoyo técnico durante su desarrollo.

- **Gemini** fue utilizado como asistente de guía en codificación y análisis, particularmente para depuración, ideas de análisis exploratorio y apoyo metodológico.
- **ChatGPT** fue utilizado para apoyar la elaboración del archivo README y la generación del documento `requirements.txt`.

Todas las decisiones analíticas, interpretaciones, validaciones y conclusiones finales fueron realizadas y revisadas por los autores.

---

# Repository Structure

```text
Proyecto-Final-IELE756/
│
├── README.md
├── requirements.txt
├── Tarea0.ipynb
├── Tarea1.ipynb
├── Tarea2.ipynb
├── Tarea3.ipynb
└── final_anomaly.ipynb
```
