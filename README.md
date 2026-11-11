# FORM-AC-01 — Análisis de caso: fallo real en un sistema distribuido

Aplicaciones Distribuidas (ISR-701) · Universidad Técnica Estatal de Quevedo · SPA 2026–2027

**Caso analizado:** incidente de GitHub del 21 de octubre de 2018

## Integrantes (grupo CLQR)

- Castro Coello Mario Sebastián (`reyshadow0`)
- Loor Suárez Steffanny del Rocío (`SteffannyLoorSuarez1`)
- Quintero Rico Luis David (`Kinetro`)
- Rivas Piloso Dayver Yahir (`drivasp`)

## Contenido del repositorio

| Ruta | Descripción |
|---|---|
| `main.tex` | Archivo principal del análisis |
| `secciones/` | Secciones del documento (una por archivo) |
| `referencias.bib` | Referencias (BibLaTeX, estilo IEEE) |
| `diagrama/` | Diagrama de causas raíz: archivo editable de draw.io (`.drawio`) y su exportación |
| `evaluaciones-pares/` | Evaluaciones recibidas de los otros equipos en la presentación |
| `main.pdf` | Versión final compilada |

El diagrama se abre con draw.io (aplicación de escritorio o <https://app.diagrams.net>) mediante
*File → Open from → Device*.

## Compilación

- **Compilador:** `pdflatex`
- **Bibliografía:** `biber` (paquete `biblatex` con estilo `ieee`)
- **Archivo principal:** `main.tex`
- **Distribución usada:** MiKTeX 26.5 en Windows

Orden de comandos, ejecutados desde la raíz del repositorio:

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

El resultado es `main.pdf`.

### Dependencias

Paquetes de LaTeX: `fontenc`, `inputenc`, `babel` (idioma `spanish`), `lmodern`, `microtype`,
`geometry`, `graphicx`, `booktabs`, `tabularx`, `array`, `float`, `xcolor`, `csquotes`,
`biblatex` con `biblatex-ieee`, y `hyperref`. Además se necesita el programa `biber`.
MiKTeX instala automáticamente los paquetes que falten; en TeX Live vienen incluidos en el
esquema completo (`scheme-full`).
