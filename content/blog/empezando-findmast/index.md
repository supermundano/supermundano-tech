---
title: Empezando Findmast 🤓
date: "2020-08-27T11:22:03"
description: "Empezamos el proyecto para encontrar partes de mástiles. Estudiamos como vamos a hacerlo y las herramientas a utilizar."
---

## Qué vamos a necesitar para desarrollar Findmast

La idea de esta aplicación es que alguien pueda subir una parte de su mástil roto (la que tenga intacta) y pueda subirlo a la plataforma para que otra gente pueda encontrarlo y que los usuarios puedan ponerse en contacto para acordar quién se queda la parte que toque. 

Ya sé que el nicho es super reducido y que lo más seguro es que no lo utilice prácticamente nadie, pero la idea es que el proyecto nos sirva para aprender a desarrollar una app completa en JAMStack y si de paso la utiliza alguien pues mejor que mejor...

Un poco más de información de lo que es JAMStack en freecodecamp: https://www.freecodecamp.org/news/what-is-the-jamstack-and-how-do-i-host-my-website-on-it/

Entonces, lo que vamos a necesitar va a ser lo siguiente:

1. Sitio web con un listado de partes de mástil o mástiles completos
2. Que se pueda filtrar el listado de mástiles con diversos parámetros
3. Que usuarios puedan darse de alta y hacer login en la plataforma para poner sus datos
4. Que los usuarios puedan subir mástiles con información y **fotos** 

En principio *'solo'* esto.

Para resolverlo y después de un primer estudio de posibilidades, vamos a utilizar lo siguiente:

1. [Gatsby](https://www.gatsbyjs.com/) como generador del sitio (SSG)
2. [Sanity](https://sanity.io/) como Headless CMS  
  https://henrique.codes/insane-quest-perfect-cms-sanity/  
  https://www.sanity.io/blog/headless-cms-explained  
  https://headlesscms.org/  
3. [Netlify](https://www.netlify.com/) como cloud host y acceso de usuarios con [Netlify Identity](https://docs.netlify.com/visitor-access/identity/). Seguramente utilicemos algo más pero de momento nos centraremos en eso.
4. [Github](https://github.com/supermundano/findmast) para control de versiones y enlazaremos el repositorio para que el sitio se genere automáticamente cada vez que hacemos una subida a la rama master
5. [Cloudinary](https://cloudinary.com/) para gestión de las imágenes. Esto no lo tengo del todo claro ya que no se si será mejor subir directamente a S3 o un Space en Digital Ocean. Lo iremos viendo...
6. [FaunaDB](https://fauna.com/) como base de datos en cloud.


## Inicio del proyecto

Montamos el sitio con el starter Hello World de Gatsby https://www.gatsbyjs.com/starters/gatsbyjs/gatsby-starter-hello-world/, totalmente vacío para empezar de cero y tener que hacerlo todo a mano. Lo conectamos a Netlify y Github para que se haga un build en cada subida a master.

Et voilà: [Findmast](https://findmast.com)

## Cosas que hemos aprendido hoy

* Crear un sitio con Gatsby
* Subir el sitio a Netlify a través de un repo de Github
* El infinito mundo del JAMStack...

Para el siguiente día nos meteremos con el layout inicial. No vamos a utilizar ningún framework tipo Tailwind, Bulma o Bootstrap. Lo vamos a hacer 100% a pelo, con un mockup básico en un papel y a disfrutar :D

> Y de momento a documentarse, y no poco... 

