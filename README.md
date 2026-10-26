# Joan Garvin Cardona · Portfolio

Portfolio personal publicado en **https://joangarvin.github.io/**.

Presenta Travseeker, Búsqueda por similitud y AirTrack, la formación en Ingeniería Informática en la UPC, las competencias técnicas y los enlaces de contacto profesional.

## Organización del código

La página usa HTML, CSS y JavaScript sin un framework ni un proceso de compilación.

El HTML sigue el mismo orden que la página: cabecera, presentación, tecnologías, proyectos, sobre mí, contacto y pie. Los comentarios marcan los bloques principales.

La hoja de estilos comienza con las variables de color, tipografía y espaciado. Después agrupa las reglas por componente y termina con las adaptaciones para pantallas de distintos tamaños y la preferencia de movimiento reducido. Las variables tienen nombres según su función, como `--color-text`, `--font-heading` y `--page-gutter`.

El JavaScript solo actualiza el año del pie de página.

## Editar

- `index.html`: contenido, proyectos y enlaces.
- `travseeker.html`: ficha pública de Travseeker, con contexto, aportación, arquitectura y capturas.
- `assets/`: logo de Travseeker y capturas públicas de la aplicación.
- `styles.css`: diseño adaptable a móvil, tableta y escritorio.
- `script.js`: actualización del año del pie de página.
- `Joan_Garvin_Cardona_CV.pdf`: versión pública del currículum, sin teléfono.

Sitio estático sin dependencias, rastreadores ni formularios que almacenen datos. Los enlaces de correo abren el cliente de correo del visitante.

## Vista local

Desde esta carpeta, con Python 3 instalado:

```sh
python3 -m http.server 8765
```

Abrir http://localhost:8765.

## Publicación

GitHub Pages publica la rama `main`, carpeta raíz `/`. Los cambios en esta rama actualizan automáticamente la web. `.nojekyll` permite servir los archivos estáticos directamente.

## Contenido

Basado en el CV proporcionado por Joan y en la documentación de los proyectos. Travseeker tiene una ficha pública con capturas reales de su aplicación y un enlace a https://travseeker.com/. Su código fuente se mantiene privado. Las capturas se tomaron el 26 de octubre de 2026 sin iniciar sesión y no contienen información de usuarios. Los gráficos de los otros proyectos son ilustrativos. AirTrack no enlaza a un repositorio porque no se facilitó un enlace verificado.

## Formato

Se usan dos espacios, archivos UTF-8 y finales de línea LF. `.editorconfig` configura el editor y `.prettierrc.json` mantiene un formato consistente.

Para formatear los archivos, desde esta carpeta:

```sh
npx prettier@3.9.10 --write index.html travseeker.html styles.css script.js favicon.svg README.md .prettierrc.json
```

Para comprobar el formato sin modificar archivos:

```sh
npx prettier@3.9.10 --check index.html travseeker.html styles.css script.js favicon.svg README.md .prettierrc.json
```

Estos comandos requieren Node.js y npm. Prettier solo se utiliza para desarrollar; el portfolio publicado no lo necesita.
