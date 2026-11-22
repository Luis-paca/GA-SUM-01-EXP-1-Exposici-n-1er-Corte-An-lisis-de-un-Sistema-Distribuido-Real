# Bitácora de Trabajo — GA-SUM-02 / EXP-1

* **Universidad:** Universidad Técnica Estatal de Quevedo (UTEQ)
* **Facultad:** Facultad de Ciencias de la Computación
* **Carrera:** Ingeniería en Software — 7.º Nivel, Paralelo "A"
* **Asignatura:** Aplicaciones Distribuidas (`SOF-I-R`)
* **Equipo:** Grupo EJPZ (Kenny Isaías España Vera, Luis Jeremy Jaramillo Acosta, Heiner Ariel Zambrano Ronquillo, Luis Alberto Paca Pilataza)
* **Sistema analizado:** JobFinder — Bolsa de Empleos para Graduados UTEQ

---

## Sesión 1 — Domingo 15 de noviembre de 2026 (20:20 – 23:02)

* **Integrantes presentes:** Luis Alberto Paca Pilataza, Luis Jeremy Jaramillo Acosta, Kenny Isaías España Vera, Heiner Ariel Zambrano Ronquillo.
* **Commits de referencia:** `dd1ddb2`, `347f29c`, `fc02d15`, `b553e16`, `1c4a246`, `695f1b7`, `f155bd0`.
* **Lo realizado:**
  * Creación del repositorio público y estructura inicial de `README.md` con la información del equipo y el flujo de compilación LaTeX (`dd1ddb2`, `347f29c`).
  * Elaboración y carga del primer bosquejo a mano de la arquitectura distribuida de JobFinder (`fc02d15`).
  * Creación del borrador inicial de notas de presentación en `main.tex` (`1c4a246`).
  * Recolección colaborativa de la base bibliográfica inicial en `referencias.bib` cubriendo recomendación laboral para graduados, transporte TCP/UDP, latencia en WebSockets, evolución de microservicios y bases de datos distribuidas (`b553e16`, `695f1b7`, `f155bd0`).
* **Problemas encontrados y resueltos:**
  * Se delimitó el alcance de análisis técnico sobre JobFinder y se repartió la búsqueda de artículos por tema para evitar entradas duplicadas en `referencias.bib`.
  * Se acordó estandarizar la bibliografía en formato IEEE utilizando `biblatex` y `biber`.

---

## Sesión 2 — Jueves 19 de noviembre de 2026 (22:11 – 23:49)

* **Integrantes presentes:** Kenny Isaías España Vera, Heiner Ariel Zambrano Ronquillo, Luis Alberto Paca Pilataza, Luis Jeremy Jaramillo Acosta.
* **Commits de referencia:** `02e30f7`, `6ecc63d`, `4b7486e`, `5045d35`, `e2fed43`.
* **Lo realizado:**
  * Depuración y ampliación de `referencias.bib` incorporando artículos indexados recientes (2021–2025) de IEEE, MDPI, Elsevier y *Facta Universitatis* sobre TCP, QUIC, WebSockets y protocolos de mensajería (`02e30f7`).
  * Desarrollo incremental del contenido técnico en `main.tex`: Presentación y Arquitectura (`6ecc63d`), Transparencias de distribución y CAP/PACELC (`4b7486e`), Modelos de comunicación y Tolerancia a fallos (`5045d35`), y estructura de cierre con tabla de aportes, declaración de IA y anexos (`e2fed43`).
* **Problemas encontrados y resueltos:**
  * Al verificar los DOIs en Crossref se detectó que la referencia inicial `ref6` (`10.56726/IRJMETS53376`) devolvía error `HTTP 404`; se retiró del archivo `.bib` y se sustituyó por artículos de revistas indexadas verificables (`02e30f7`).
  * Se dividió la edición de `main.tex` por bloques independientes para sostener un historial progresivo y reducir conflictos de fusión.

---

## Sesión 3 — Viernes 20 de noviembre de 2026 (16:55 – 23:59)

* **Integrantes presentes:** Heiner Ariel Zambrano Ronquillo, Luis Jeremy Jaramillo Acosta, Kenny Isaías España Vera, Luis Alberto Paca Pilataza.
* **Commits de referencia:** `e36772b`, `e8a8591`, `2885c9b`, `74fe9e9`, `a8d9d55`, `8334fcd`, `e16084f`.
* **Lo realizado:**
  * Creación de `diapositivas.tex` (Beamer) con las láminas de Transparencias de distribución y CAP/PACELC, e integración de la primera captura subrayada (`evidencias/captura_camilleri2024_heiner.png`, Camilleri *et al.*, 2024, pág. 6 de 41) (`e36772b`, `e8a8591`).
  * Redacción en `main.tex` de las secciones 7, 8 y 9: comparación crítica con LinkedIn, lecciones aplicadas al PFC (`TA-PFC-E1`) y ejemplos del entorno propio en Ecuador (SGA UTEQ en matriculación, De Una / Banco Pichincha y conectividad móvil Valencia–Quevedo) (`2885c9b`).
  * Incorporación en `diapositivas.tex` de las secciones 1–2 (`a8d9d55`) y 5–6 (`e16084f`), además de la clasificación formal de fallos (*omisión*, *temporización*, *crash-stop*) y el criterio de verificación en la tabla de causas raíz `FORM-AC-01` (`e16084f`).
  * Completado de metadatos faltantes (volumen, páginas, coautores y DOI) en `referencias.bib` para `ref2`, `jeddou2023tcpquic` y `kumar2025kquic` (`8334fcd`).
* **Problemas encontrados y resueltos:**
  * Al integrar las secciones 7–9 en `2885c9b` se recortó por error el bloque final de `main.tex` (declaración de IA, referencias y apertura de anexos); se detectó de inmediato y se restauró en `74fe9e9` para mantener el documento compilable.
  * Al contrastar contra Crossref se completaron campos omitidos en `kumar2025kquic` (DOI `10.1109/ACCESS.2025.3578120`, vol. 13, págs. 100392–100404) y `jeddou2023tcpquic` (vol. 4, págs. 2596–2608) (`8334fcd`).

---

## Sesión 4 — Sábado 21 de noviembre de 2026 (18:33 – 23:45)

* **Integrantes presentes:** Kenny Isaías España Vera, Luis Alberto Paca Pilataza, Luis Jeremy Jaramillo Acosta, Heiner Ariel Zambrano Ronquillo.
* **Commits de referencia:** `90dd836`, `7ebaac2`, `07608ea`, `16949c5`, `fc7574c`, `40de8cc`, `58be075`, `5449302`, `13a33bb`, `3c4d872`, `c7c1d18`, `6461c75`, `7c2c381`, `1c0a469` y commit de cierre.
* **Lo realizado:**
  * Actualización del boceto a mano incorporando los nombres de los cuatro integrantes y la fecha (`20/11/2026`) escritos a esfero, movido a `evidencias/ArquitecturaDistribuidaAmano.jpeg`, junto con la captura subrayada de Yao *et al.* (2023, pág. 1) (`90dd836`).
  * Carga de las capturas subrayadas de Mitrović *et al.* (2023, págs. 268 y 278) (`7ebaac2`) y de Yaroshynskyi *et al.* (2025, pág. 2 de 21) (`58be075`), reuniendo cinco evidencias de lectura de los cuatro integrantes en el Anexo B de `main.tex`.
  * Actualización bibliográfica: incorporación de Petrescu *et al.* (2025) (`07608ea`), retiro de la clave local sin definir `espana2025bolsa` y adición de fuentes primarias verificables (INEC ENEMDU mayo 2025, Seguimiento a Graduados UTEQ 2022 y publicaciones técnicas de LinkedIn Engineering) (`16949c5`, `fc7574c`, `40de8cc`).
  * Migración de `main.tex` de BibTeX clásico (`IEEEtran`) a `biblatex` con `biber`, completado de la tabla de aportes y declaración de uso de IA (Claude y Gemini) (`fc7574c`, `58be075`).
  * Carga del diagrama editable `Arquitectura_JobFinder_Real_EJPZ.drawio` y actualización de su exportación gráfica `arquitectura_jobfinder.png` en alta resolución (`3729 × 1560 px`).
  * Rediseño final de `diapositivas.tex` (tarjetas `tcolorbox`, `FiraSans` e `Inconsolata`, Práctica 2 sobre código Spring Boot y DevTools) y adaptación completa de `main.tex` al orden y reparto definitivo de expositores (`5449302`, `3c4d872`).
  * Corrección del nombre oficial de la facultad en `main.tex`, renombrado del documento compilado a `main.pdf` y actualización de `diapositivas.pdf` (`c7c1d18`, `6461c75`, `7c2c381`, `1c0a469`).
  * Grabación del ensayo grupal completo (rostro y voz de los cuatro integrantes, ≤ 12 minutos), publicación en YouTube (`https://youtu.be/BtBp5cWaXLg`), actualización de `README.md`, prueba de compilación limpia en Docker (`pdflatex -> biber -> pdflatex -> pdflatex`) y etiquetado final `v1.0`.
* **Problemas encontrados y resueltos:**
  * **Motor bibliográfico inconsistente:** `main.tex` compilaba con BibTeX mientras `diapositivas.tex` y `README.md` indicaban `biber`; se migró `main.tex` a `biblatex`/`biber` para unificar el comando de regeneración.
  * **Cifras sin fuente primaria:** se eliminó `espana2025bolsa` y se respaldaron los porcentajes directamente con INEC (2025), UTEQ (2022) y LinkedIn Engineering con fechas de acceso.
  * **Límite de tiempo en Overleaf gratuito:** el rediseño de `diapositivas.tex` con `tcolorbox[most]` y `FiraSans` superó el límite del plan gratuito; se compiló localmente en contenedor Docker (`texlive/texlive:latest`), corrigiendo los desbordes verticales (`Overfull \vbox`) en las láminas 5 y 6 y el desborde horizontal (`Overfull \hbox`) en `main.tex` (`seguridad.auditoria`) hasta lograr 0 errores y 0 advertencias.
  * **Coherencia de entregables:** se renombraron los PDFs finales a `diapositivas.pdf` y `main.pdf`, se sustituyó el PNG del diagrama por su exportación HD (`3729 × 1560 px`), se corrigió el nombre de facultad y se alineó `README.md` con los archivos reales del repositorio.

---

## Resumen de verificación previa a la entrega

| Verificación | Estado |
| :--- | :---: |
| Trabajo distribuido en ≥ 3 días distintos (15, 19, 20 y 21 nov) | Cumplido (4 días) |
| Mínimo 3 commits significativos por integrante | Cumplido (todos ≥ 6 commits) |
| Diagrama editable `.drawio` y exportación gráfica HD (`3729 × 1560`) | Cumplido |
| Foto del boceto inicial a mano con nombres y fecha (`evidencias/`) | Cumplido |
| Mínimo 3 capturas anotadas de artículos con página indicada | Cumplido (5 capturas) |
| Compilación reproducible `pdflatex -> biber -> pdflatex -> pdflatex` | Cumplido (0 errores) |
| Declaración de uso de IA y tabla de aportes en `main.tex` | Cumplido |
| Video del ensayo (≤ 12 min, 4 integrantes) enlazado en `README.md` | Cumplido (`youtu.be/BtBp5cWaXLg`) |
