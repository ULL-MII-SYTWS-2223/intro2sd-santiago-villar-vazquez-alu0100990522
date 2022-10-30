![Open in Codespaces](https://classroom.github.com/assets/open-in-codespaces-abfff4d4e15f9e1bd8274d9a39a0befe03a0632bb0f153d0ec72ff541cedbe34.svg)

bundle install

rake serve


Despliegue del sitio web en github pages : https://ull-mii-sytws-2223.github.io/intro2sd-santiago-villar-vazquez-alu0100990522/

Para añadir un post al documento deberemos añadir un nuevo archivo .md en la carperta _post con el formato AÑO/MES/DIA-NOMBRE.md

Tambien se modifico el archivo _config.yml, donde cambiaremos el tema de la página modificando (minimal_mistakes_skin) y luego en (baseurl) modificaremos la ruta de nuestra web, asi como un poco el perfil del usuario que muestra. 

Para la instalación del netlify seguiremos los pasos propuestos por esta web: 

https://www.netlify.com/blog/2020/04/02/a-step-by-step-guide-jekyll-4.0-on-netlify/

Tendremos que hacer publico este repositorio github para poder conectarlocon netlify, configurar como se despliega y lanzarlo

![interfaz_gitpod](assets/images/netlify.PNG)


Para la creacion de una nueva collection deberemos de crear una nueva carpeta , en nuestro caso sera _books y en el archivo _config.yml añadiremos lo siguiente

```bash
collections:
  books:
    output: true
    permalink: /:collection/:path/
    
    
  defaults:  
    # _books
  - scope:
      path: ""
      type: books
    values:
      layout: single
      author_profile: false
      share: true
      comments: true

```

tambien deberemos de crear una nueva pagina en _pages para books.
