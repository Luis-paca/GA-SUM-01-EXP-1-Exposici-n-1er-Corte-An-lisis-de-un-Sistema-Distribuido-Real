# GA-SUM-02 / EXP-1 — Análisis de Sistema Distribuido: WebSockets, TCP y UDP en JobFinder 

Repositorio del **Equipo EJPZ** para la exposición del primer corte de la asignatura **Aplicaciones Distribuidas** (Carrera de Ingeniería en Software, Paralelo A — Universidad Técnica Estatal de Quevedo).

## Integrantes del Equipo (EJPZ)
* **España Vera Kenny Isaías**
* **Jaramillo Acosta Luis Jeremy**
* **Paca Pilataza Luis Alberto**
* **Zambrano Ronquillo Heiner Ariel**

## Video del Ensayo (Máximo 12 minutos)
* **Enlace al video (YouTube No Listado / Google Drive abierto):** 

## Estructura del Repositorio
* `diapositivas.tex` / `diapositivas.pdf`: Presentación elaborada en LaTeX (`beamer`) con referencias en formato IEEE.
* `main.tex` / `main.pdf`: Notas desarrolladas de la exposición (2 a 4 páginas), ejemplos del entorno propio, tabla de aportes, declaración de IA y anexo del esquema inicial a mano.
* `referencias.bib`: Base bibliográfica verificada (mínimo 6 fuentes de los últimos 5 años, incluyendo artículos con DOI verificable).
* `Arquitectura_JobFinder_Real_EJPZ.drawio` / `arquitectura_jobfinder.png`: Diagrama editable y exportación gráfica de la arquitectura híbrida de JobFinder.
* `demo_websockets_ejpz/`: Scripts de demostración en vivo (`demo_udp.js`, `server_jobfinder.js`, `cliente_jobfinder.html`).
* `evidencias/`: Fotografía del boceto inicial a mano (`ArquitecturaDistribuidaAmano.jpeg`) y capturas anotadas de los artículos citados.
* `BITACORA.md`: Registro cronológico de sesiones de trabajo y problemas técnicos resueltos.

## Instrucciones de Compilación

* **Compilador requerido:** `pdfLaTeX` + `Biber` (distribución TeX Live 2023+ o MiKTeX).
* **Archivos principales:** `diapositivas.tex` y `main.tex`.
* **Dependencias LaTeX:** `beamer`, `inputenc`, `fontenc`, `babel` (`spanish`), `lmodern`, `graphicx`, `booktabs`, `tabularx`, `hyperref`, `csquotes`, `tikz`, `enumitem`, `titlesec`, `array`, `xcolor`, `geometry`, `url`, `biblatex` (`style=ieee`, `backend=biber`).

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
