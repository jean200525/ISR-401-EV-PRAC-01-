# EV-PRAC-01 — Evaluación de la Unidad I

**Asignatura:** Ingeniería de Requerimientos (ISR-401), UTEQ, 4.º nivel, paralelo B, SPA 2026–2027.  
**Estudiante:** ROBINSON ESPINOZA JEANPIERRE.  
**Caso:** ALERTARÍO — Sistema de Alerta Temprana de Crecidas.  
**Fecha de la sesión:** 18 de noviembre de 2026.

Repositorio: https://github.com/jean200525/ISR-401-EV-PRAC-01-

## Estructura

```
.
├── README.md                       Este archivo: instrucciones de compilación
├── EV-PRAC-01/
│   ├── main.tex                    Transcripción fiel de la prueba
│   ├── main.pdf                    PDF compilado desde main.tex
│   └── evidencias/
│       ├── hoja-01.jpg              Fotografía de la hoja 1
│       ├── hoja-02.jpg              Fotografía de la hoja 2
│       ├── hoja-03.jpg              Fotografía de la hoja 3
│       ├── hoja-04.jpg              Fotografía de la hoja 4
│       └── hoja-05.jpg              Fotografía de la hoja 5
└── sga/
    ├── caratula.tex                PDF de una página para el SGA (URL + captura)
    ├── caratula.pdf                PDF generado
    └── nota-ev.png                 Captura del resumen del cuestionario EV-CUE-01
```

Las fotografías están en formato **JPG** (la rúbrica acepta JPG o PNG) y se nombran `hoja-01.jpg` a `hoja-05.jpg`, según lo indicado en la sección 3 de la guía-rúbrica.

## Compilación reproducible

**Archivo principal:** `EV-PRAC-01/main.tex`.  
**Compilador:** `pdflatex`.  
**Orden de comandos:**

```bash
cd EV-PRAC-01
pdflatex -interaction=nonstopmode main.tex
```

El resultado es `EV-PRAC-01/main.pdf`. No se necesita BibTeX/Biber porque la transcripción no contiene citas ni bibliografía.

**Dependencias:** distribución TeX Live o MiKTeX con `babel-spanish`, `geometry`, `graphicx`, `tabularx`, `longtable`, `array` e `hyperref` (todas incluidas en una instalación estándar).

Para regenerar la carátula del SGA:

```bash
cd sga
pdflatex -interaction=nonstopmode caratula.tex
```

## Nota de fidelidad

`main.tex` reproduce el contenido escrito a mano, sin agregar, corregir ni completar respuestas. La portada incluye únicamente los datos de identificación y la declaración de transcripción fiel exigida en la regla R5 de la guía-rúbrica. Las fotografías originales se conservan en `EV-PRAC-01/evidencias/` y no se incrustan en `main.pdf`.
