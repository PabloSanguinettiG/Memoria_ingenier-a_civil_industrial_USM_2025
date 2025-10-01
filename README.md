# ¿Cómo elevar la productividad del gasto social?
**Medición de ineficiencias y diseño de incentivos en Salud y Educación (Chile)**  
**Memoria Ingeniería Civil Industrial — UTFSM (2025)**

> **Nota:** los archivos con extensión `.txt` son **código R** (se mantuvieron como `.txt` por compatibilidad). Puedes abrirlos como **.R** sin problemas.

---

## Descripción
Este repositorio contiene el código y las indicaciones para replicar los principales resultados de la memoria: modelos **DEA BCC–VRS orientados a output** en salud (A1–A2–B1–B2), análisis de **costo por egreso GRD** junto con **ALOS** y **ocupación**, y paneles de desempeño en educación (SIMCE y educación superior).

La lógica del repositorio es **transparencia y trazabilidad**: cada script documenta supuestos, fuentes oficiales y pasos de limpieza antes de graficar o estimar.

---

## Contenidos del repositorio
- `GRAFICOS_SALUD.txt` → R: gráficos/figuras de la sección Salud (incluye relaciones GRD–ALOS–ocupación).
- `MODELO_A1.txt` → R: DEA BCC–VRS orientado a output (nivel servicio/establecimiento, sin ajuste de calidad).
- `MODELO_A2.txt` → R: DEA BCC–VRS (variantes/robustez a nivel establecimiento).
- `MODELO_B1.txt` → R: DEA BCC–VRS (nivel servicio–establecimiento con otras combinaciones de inputs/outputs).
- `MODELO_B2.txt` → R: DEA BCC–VRS con **salida ajustada por calidad** (por ejemplo, egresos vivos).
- `MODELO_EDUCACION.txt` → R: paneles y lecturas por pares para resultados en **Educación** (SIMCE; matrícula/beneficios ES).
- `README.md` → este documento.

---

Todo basado en: https://github.com/jaimercz/utfsm-thesis

