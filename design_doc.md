# Titulo: Sistema de Reviews
---
## Overview: Problema a resolver
 La empresa "RandomCameraReviews" necesita un sistema que permita que fotografos profesionales suban "reviews" de Camaras fotograficas, para que cualquier persona desde cualquier parte del mundo pueda buscar los los reviews y comprarlas a travez de su portal.



### Alcance(Scope)
La empresa cuenta con un equipo de developers especializado en frontEnd que realizara un portal para que los editores suban los "reviews" y los usuarios puedan verlos. Por lo que se solicita que se les proporciones un sistema, incluyendo API que permita  realizar lo siguiente:

* Subir reviews de Camaras fotograficas
* Obtener el contenido de los reviews para mostrarlo en vistas del portal en sus versiones web y mobile.
* Manejo de usuarios para editores (no incluye visitantes que leen los reviews)

Tambien se sabe que la empresa "RandomCameraReviews" planea distribuir mayormente en America del Sur donde esta su mercado mas grande, pero tambien tienen ventas en norte america, Europa, y muy pocas en Asia.

#### Casos de uso
* Como editor me gustaria poder subir una review de una camara
* Como editor me gustaria poder subir una review de un lente para las camaras
* Como usuario no registrado me gustaria poder leer reviews.

#### Out of Scope (casos de uso No Soportados)
* Como usuario no registrado me gustaria poder subir una review de una camara.
* Como usuario no registrado me gustaria poder dejar feedback en comentarios.
* Como usuario no registrado me gustaria poder compartir una review en redes sociales.
* Como editor registrado me gustaria poder quitar una review previamente subida
* Como editor registrado me gustaria poder comentar otras reviews.
---
## Arquitectura

### Diagramas
poner diagramas de secuencia, uml, etc

### Modelo de datos
Poner diseño de entidades, Jsons, tablas, diagramas entidad relación, etc..

---
## Limitaciones
Lista de limitaciones conocidas. Puede ser en formato de lista.
* Llamadas del API que permiten subir un review, no exceden los limites de latencia de 500ms.
* No se soporta mas de X llamadas por segundo
* Llamdas al API que permite obtener los review para lectura, deben de tener una latencia menor a 100ms.
---
## Costo
Descripción/Análisis de costos
Ejemplo:
"Considerando N usuarios diarios, M llamadas a X servicio/baseDatos/etc"
* 1000 llamadas diarias a serverless functions. $XX.XX
* 1000 read/write units diarias a X Database on-demand. $XX.XX
Total: $xx.xx (al mes/dia/año)
