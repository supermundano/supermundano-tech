---
title: Menudo lío llevamos 🧐
date: "2021-01-29T21:12:03"
description: "Descartamos todo lo que habíamos decidido que íbamos a utilizar y empezamos de cero..."
---

Bueno, la idea de hacer la aplicación Findmast sigue ahí, pero después de tanto tiempo sin tocar el desarrollo me entra la duda de si hacerlo con otra plataforma. He llegado a este punto porque no he parado de escuchar y leer artículos sobre las bondades de [Nextjs](https://nextjs.org/) y la verdad que creo que voy a descartar lo empezado con Gatsby...

La razón es bastante sencilla: en findmast.com habrá contenido que puede que no esté renderizado, es decir, si consigo implementar la subida de partes de mástiles por parte de los usuarios, si lo hiciera con Gatsby, cada vez que alguien subiera un artículo tendría que regenerar todo el site. En cambio con Nextjs tengo la posibilidad de generar la página de ese artículo del lado del servidor, de manera que haya una especie de generación incremental.

Después de tanto tiempo y un par de cursos con Wes Bos, prefiero empezar con esta plataforma. Con lo que en principio y si nada se tuerce, utilizaremos el siguiente stack:

1. [Nextjs](https://nextjs.org/) como generador del sitio SSG + SSR
2. Contenidos en [Sanity](https://sanity.io) o GraphCMS
3. Para la autenticación de usuarios utilizaremos [NextAuth](https://next-auth.js.org/)
4. [Github](https://github.com/supermundano/findmast) para control de versiones y enlazaremos el repositorio para que el sitio se genere automáticamente cada vez que hacemos una subida a la rama master
5. Tengo bastante claro que utilizaremos Netlify functions para poder hacer las subidas de formularios a Sanity, pero es posible que optemos por otra vía. Haríamos algo como esto: https://github.com/sanity-io/netlify-form-sanity

Desconozco si necesitaríamos un servidor externo para subir las fotos o si deberíamos dejarlo todo en Sanity. Demasiadas ideas y mucho trabajo por delante...

Voy a desarrollarlo todo en local para ver que se puede hacer y luego decidiré la plataforma a la que subirlo todo según los tiers gratuitos que tengan y los precios al escalar. 

En fin, toca reiniciar!! 

3... 2... 1...

