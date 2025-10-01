# ¿Cómo elevar la productividad del gasto social?
**Medición de ineficiencias y diseño de incentivos en Salud y Educación (Chile)**  
**Memoria Ingeniería Civil Industrial — UTFSM (2025)**

> Repositorio público con los scripts y materiales que reproducen las figuras/tablas y análisis de la memoria.  
> **Nota:** los archivos con extensión `.txt` son **código R** (se mantuvieron como `.txt` por compatibilidad), puedes abrirlos como **.R** sin problemas.

---

## 👋 Descripción
Este repositorio contiene el código y las indicaciones para replicar los principales resultados de la memoria: modelos **DEA BCC–VRS orientados a output** en salud (A1–A2–B1–B2), análisis de **costo por egreso GRD** junto con **ALOS** y **ocupación**, y paneles de desempeño en educación (SIMCE y educación superior).

La lógica del repo es **transparencia + trazabilidad**: cada script documenta supuestos, fuentes oficiales y pasos de limpieza antes de graficar o estimar.

---

## 🗂️ Contenidos del repositorio
- `GRAFICOS_SALUD.txt` → R: gráficos/figuras de la sección Salud (incluye relaciones GRD–ALOS–ocupación).
- `MODELO_A1.txt` → R: DEA BCC–VRS orientado a output (nivel servicio/establecimiento, sin ajuste de calidad).
- `MODELO_A2.txt` → R: DEA BCC–VRS (variantes/robustez a nivel establecimiento).
- `MODELO_B1.txt` → R: DEA BCC–VRS (nivel servicio–establecimiento con otras combinaciones de inputs/outputs).
- `MODELO_B2.txt` → R: DEA BCC–VRS con **salida ajustada por calidad** (p. ej., egresos vivos).
- `MODELO_EDUCACION.txt` → R: paneles y lecturas por pares para resultados en **Educación** (SIMCE; matrícula/beneficios ES).
- `README.md` → este documento.

> Si prefieres, puedes renombrar cualquier `.txt` a `.R` para ejecutarlo directamente en RStudio.

---

## 🏗️ Requisitos
- **R ≥ 4.2** (recomendado) y **RStudio**.
- Paquetes sugeridos (instalación automática al correr los scripts si hiciera falta):
  - `tidyverse`, `readr`, `dplyr`, `ggplot2`
  - `lubridate`, `stringr`
  - Para DEA: `Benchmarking` o `deaR` (según el script)
  - Para regresiones simples/diagnóstico: `broom`, `modelr`
  - Para tablas/exports: `readxl` / `openxlsx` (si cargas planillas locales)

> **Datos**: los scripts asumen rutas locales o descarga desde **fuentes abiertas oficiales** (ver sección siguiente). Ajusta rutas con tus carpetas locales si corresponde.
