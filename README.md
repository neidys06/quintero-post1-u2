# Post-contenido — Unidad 2: HTML5 Básico

## Descripción
Repositorio del laboratorio de la Unidad 2 de Programación Web — Séptimo
Semestre. Contiene dos partes: página de portafolio con etiquetas semánticas
de HTML5 (`parte-1-pagina-semantica/`) y formulario de registro con
validación nativa HTML5 (`parte-2-formulario-registro/`).

## Parte 1 — Página semántica
Página de portafolio personal que implementa `header`, `nav`, `main`,
`section`, `article`, `aside` y `footer`, con listas `ul`/`ol`/`dl`, un
bloque de multimedia (audio) con su recurso de accesibilidad asociado
(transcripción), una sección de preguntas frecuentes con
`details`/`summary`, y meta tags de SEO. Ver `parte-1-pagina-semantica/`.


## Decisiones de diseño

### 1. Estructura semántica de "Logros y Certificaciones" (Parte 1)
Se eligió la **Opción A**: cada logro se marca como un `<article>`
independiente. Se aplicó el criterio de la guía teórica (sección 2.3):
"¿tiene sentido por sí solo fuera del sitio?". Una certificación (por
ejemplo, un curso o un reconocimiento) es un dato autocontenido: tiene
nombre, fecha e institución propios, y podría copiarse tal cual a un CV o a
un perfil de LinkedIn sin perder sentido, sin depender del resto de la
página. Por eso corresponde a contenido redistribuible por sí mismo, que es
justamente la definición de `<article>` en la guía.

### 2. Formato multimedia de la introducción personal (Parte 1)
Se eligió la **Opción B**: audio con transcripción dentro de
`<details>`/`<summary>`. El clip es una introducción hablada de 20-40
segundos sin necesidad de mostrar entorno ni gestos, por lo que el video no
aporta información adicional relevante frente al audio. El audio es más
simple de grabar (no requiere edición de video ni generar un archivo `.vtt`
sincronizado por timestamps) y de todas formas cumple el principio
"Perceptible" de WCAG (guía 7.1) gracias a la transcripción completa y
literal incluida en el `<details>`, que cualquier usuario —incluyendo
quienes usan lector de pantalla o no pueden reproducir audio— puede leer.


## Capturas de pantalla
![Página principal](parte-1-pagina-semantica/img/captura-01.png)