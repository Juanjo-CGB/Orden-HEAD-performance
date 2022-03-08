# Optimización orden HEAD

Cómo ordenar las etiquetas HTML dentro de la sección <head> para obtener el máximo rendimiento en tu proyecto o sitio web.

## Construido con

**HTML:** Estructura HEAD

## Descripción

El <head> es la parte más grande que bloquea el renderizado de una página web. Es un elemento al que los desarrolladores front-end le prestamos menos atención, pero es realmente importante y necesario conocer cómo cargar nuestros estilos, fuentes o scripts porque afectan directamente a la experiencia de usuario. ¡Y todo va en el <head>!

## Código

```html
<head>
    <meta charset="UTF-8"> <!--Codificación de caracteres usada-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!--Área disponible en la pantalla del navegador-->
    <title>Orden Óptimo HEAD</title> <!--Título de la página-->
    <link rel="preconnect" href="..."> <!--Peticiones a las DNS-->
    <script async src="..."></script> <!--Scripts que manipulan o interaccionan con el DOM antes de DOMContentLoaded y/o que no tienen dependencias con otros scripts-->
    <!--EVITAR-->
    <!--<style>@import url("css/layout.css");</style> --- CSS que incluya @import-->
    <!--<script></script> --- JS Síncrono-->
    <link rel="stylesheet" href="..."> <!--CSS Síncrono-->
    <link rel="preload" href="..."> <!--Precarga de elementos-->
    <script defer src="..."></script> <!--Scripts que manipulan o interaccionan con el DOM después de DOMContentLoaded y/o que tienen dependencias con otros scripts-->
    <!--Resto de etiquetas (SEO meta tags, iconos, etc.)-->
    <meta name="description" lang="es" content="..." />
    <link rel="shortcut icon" type="image/png" href="..."/>
</head>
```

## Autor

[@Juanjo-CGB](https://github.com/Juanjo-CGB)
