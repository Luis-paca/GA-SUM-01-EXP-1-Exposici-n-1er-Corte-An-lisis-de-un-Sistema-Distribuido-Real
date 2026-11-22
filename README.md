# GA-SUM-02 / EXP-1 — Análisis de Sistema Distribuido: WebSockets, TCP y UDP en JobFinder

Repositorio del **Equipo EJPZ** para la exposición del primer corte de la asignatura **Aplicaciones Distribuidas** (Facultad de Ciencias de la Computación, Carrera de Ingeniería en Software, Paralelo A — Universidad Técnica Estatal de Quevedo).

## Integrantes del Equipo (EJPZ)
* **España Vera Kenny Isaías**
* **Jaramillo Acosta Luis Jeremy**
* **Paca Pilataza Luis Alberto**
* **Zambrano Ronquillo Heiner Ariel**

## Video del Ensayo (Máximo 12 minutos)
* **Enlace al video (YouTube):** https://youtu.be/BtBp5cWaXLg

## Estructura del Repositorio
* `diapositivas.tex` / `diapositivas.pdf`: Presentación elaborada en LaTeX (`beamer`) con referencias en formato IEEE.
* `main.tex` / `main.pdf`: Notas desarrolladas de la exposición, ejemplos del entorno propio, tabla de aportes, declaración de uso de IA y anexos (boceto a mano y capturas de lectura).
* `referencias.bib`: Base bibliográfica verificada (15 fuentes: 11 artículos indexados 2021–2025 con DOI verificable y 4 fuentes primarias institucionales/técnicas).
* `Arquitectura_JobFinder_Real_EJPZ.drawio` / `arquitectura_jobfinder.png`: Diagrama editable y exportación gráfica en alta resolución de la arquitectura híbrida de JobFinder.
* `evidencias/`: Fotografía del boceto inicial a mano con nombres y fecha (`ArquitecturaDistribuidaAmano.jpeg`) y 5 capturas subrayadas de los artículos citados con número de página.
* `BITACORA.md`: Registro cronológico de sesiones de trabajo, commits de referencia y problemas técnicos resueltos.

## Instrucciones de Compilación

* **Compilador requerido:** `pdfLaTeX` + `Biber` (distribución TeX Live 2023+ o MiKTeX; probado también en Docker `texlive/texlive:latest`).
* **Archivos principales:** `diapositivas.tex` y `main.tex`.
* **Dependencias LaTeX:** `beamer`, `inputenc`, `fontenc`, `babel` (`spanish`), `csquotes`, `FiraSans`, `inconsolata`, `lmodern`, `graphicx`, `booktabs`, `tabularx`, `array`, `colortbl`, `xcolor`, `tikz`, `tcolorbox`, `enumitem`, `titlesec`, `geometry`, `hyperref`, `url`, `biblatex` (`style=ieee`, `backend=biber`).

Para regenerar ambos documentos PDF desde la terminal en la raíz del repositorio, ejecutar en orden:

```bash
# 1. Compilar Diapositivas Beamer
pdflatex diapositivas.tex
biber diapositivas
pdflatex diapositivas.tex
pdflatex diapositivas.tex

# 2. Compilar Notas de Presentación
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```
