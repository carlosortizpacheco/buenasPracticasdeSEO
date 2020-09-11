# Buenas Practicas de SEO

## Qué es SEO?
- Es la optimizacion de un sitio web para lograr la indexación en los motores de búsqueda y así mejorar su visibilidad en los resultados orgánicos.
+ Qué logramos con el SEO?
  + Mejora posición de keywords
  + Aumento de tráfico
- Resultados y trabajo a mediano-largo plazo.
- Titulo; caracteres entre 55-65
- Descripción; caracteres entre 155-165

### SEO OnPage y OffPage
+ SEO OnPage
  + Dominio
    + Canonical
    + Redirecciones
  + Estructura de Urls
    + jerarquia (niveles de la URL)
    + Urls amigables (no caracteres extraños)
    + breadcrumbs
  + Contenido Enriquecido
    + Microdatos
    + Fragmentos destacados
  + Infraestructura del sitio
    + solucion 404
    + protocolo HTTPS
    + memoria cache
    + CDN 
    + Favicon
  + Optimización de contenido (keyword)
    + metadada
    + etiquetas
    + Url optimizada
    + anchor text
    + keyword en contenido
  + Indexación
    + sitemap.xml (que quiero que analice google)
    + robots.txt (que no quiero que analice google)
    + search console
    + analytics (medir implementaciones)
  + Social media
    + vinculacion a redes
    + SMO - Youtube
    + opengraph
+ SEO OffPage
  + Link Building
  + SEO Local (google my business)
  + Mención en redes sociales

### Optimizar Contenido
+ Hay dos escenarios de optimización de contenido:
  + Creado
    + Búsqueda de keywords indexadas
    + Keyword research
    + Seleccion de keywords
    + Optimización de contenido en el sitio
  + Nuevo
    + Búsqueda de keywords indexadas
    + Keyword research
    + Seleccion de keywords
    + Optimización de contenido en el sitio
- Piramide invertida; como escribir para internet. En el primer parrafo colocar Quien?,Que?,Cuando?,Como?,Por que?


### Keyword planner
- Hay que crear una campaña en google ad
+ **keyword long tail**, esta compuesta de varias keywords
  + Es más facil posicionar keywords long tail que keywords golden y muy generales
  + Luego de haber posicionado keywords long tail por un buen tiempo es más fácil llegar a posicionar golden keywords.
  + Generamos tráfico con 5 keywords diferentes, con esta keyword long tail en una landing page.

### Optimización de Etiquetas
- Metadata; titulo y descripción
- Etiquetas H: H1(única), H2, etc.
- Url optimizada
- keywords en contenido
- Anchor text

```html
<title>Venta de Juegos PS4 baratos en Bogotá | Clic Actualizado</title>
<meta name='description' content='Clic actualizado tiene para ti venta de juegos baratos
 para diferentes consolas como PS4, Xbox y Nintendo, envíos gratis en Bogotá. Compra online Aqui!'>
<h1>Venta de Juegos</h1>
<h2>Estos son los 3 juegos destacados para PS4 de esta semana en Bogotá</h2>
```
### Optimización de imágenes
```html
<img src='' alt='Juego PS4 Gran Turismo'>
```
- Optimizar el peso de las imágenes; no debe pesar mas de 300kb las imágenes grandes (imágenes de fondo)
- imágenes pequeñas, no deben de pesar más de 150kb.
- tinypng.com; página para reducir el tamaño de las imagenes.

### Canonical y Redirecciones 301
- Canonical; le digo a google que esta es la única Url que va a indexar.
```html
<head>
  <link 
    rel='canonical'
    href='https://clicactualizado.com'/>
</head>
```
+ Para implementar una redireccion 301?
  + Al fichero .htaccess de tu hosting o servidor debes agregar el código que obtienes de la página siguiente: https://www.infranetworking.com/redireccion-301-302
  

### Tipos de redirecciones
- **301**; Se trata de una redirección permanente, contenido eliminado o movido de manera perpetua.
- **302**; Se trata de una redirección un poco más ambigua y se utiliza para hacer redirecciones temporales (direcciones para promociones-black friday etc.).
