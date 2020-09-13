![](https://img.shields.io/static/v1?label=technology&message=SEO&color=blue)
![](https://img.shields.io/static/v1?label=technology&message=Analytics&color=red)
![](https://img.shields.io/static/v1?label=technology&message=SearchConsole&color=red)
![](https://img.shields.io/static/v1?label=technology&message=TagManager&color=red)
![](https://img.shields.io/static/v1?label=school&message=platzi&color=green)
![](https://img.shields.io/static/v1?label=course&message=CursoDeBuenasPrácticasDeSEO&color=green)

# Buenas prácticas de SEO

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


### Vinculación de Tag Manager, analytics y Search Console
- Ya con una cuenta de GMail ir a Tag Manager, colocar los datos de la página y pegar el código que dan en el `head` y en el `body`
- Crear cuenta de analytics
- Search Console; enfocado a lo orgánico. Esta dentro de Analytics > Adquisición.
- Porcentaje de rebote; relación de personas que entran a la página y se salen luego luego.
- Conocer desde que navegador se mete más la gente. Varia por país (España, Bing).
- CTR; relación entre clic e impresiones.

### Indexación con Sitemap.xml y Robots.txt
- sitemaps.org; 
```html
<urlset >
  <url>
    <loc>http://www.example.com</loc> /*La Url de mi página*/
    <lastmod>2020-01-01</lastmod> /*cuando se modificó por última vez*/
    <changefreq>monthly</changefreq> /*Cada cuanto tiempo quiero que indexe la página*/
    <priority>0.8</priority> /*puedo dar prioridad a distintas partes de la página*/
  </url>
```
 ```html
<sitemapindex xmlns='htts://sitemaps.org/schemas/sitemap/0.9' >
  <sitemap>
    <loc>http://www.example.com/sitemap1.xml.gz</loc> /*La Url de mi página, en ingles*/
    <lastmod>2020-01-01</lastmod> /*cuando se modificó por última vez*/
  </sitemap>
  <sitemap>
    <loc>http://www.example.com/sitemap2.xml.gz</loc> /*La Url de mi página, en español*/
    <lastmod>2020-01-01</lastmod> /*cuando se modificó por última vez*/
  </sitemap>
</sitemapindex>
```
- **xml-sitemaps.com**, sirve para generar un xml, para indicarle que indexe lo que le indico.
+ **tools.seobook.com/**, sirve para generarl el robots.txt (para que no indexe lo que le indique).
  + `Disallow: /playstation/*`; no indexa todo lo que esta dentro de playstation
  + `Disallow: /playstation$`; no indexa playstation, pero si lo que esta adentro de playstation.

### 404; Personalizada y solución de enlaces rotos (screaming frog)
- Meter la Url de mi página, screaming frog la escanea y ya veo donde hay 404. Estos los debo de solucionar lo más pronto posible.

### HTTPS, GZIP, Caché, CDN Y Favicon
- La infraestructura mejora los tiempos de carga y mejoramos la experiencia de usuario.
+ **HTTPS**
  + Protocolo de seguridad de la transferencia de datos de hipertexto - **versión segura de HTTP.**
  + Utiliza un cifrado basado en la seguridad de textos SSL/TLS para crear un canal cifrado.
  + La información sensible (usuario y claves de paso normalmente) no pueda ser usada por un atacante que intercepte la transferencia de datos de la conexión, lo único que obtendrá será un flujo de datos cifrados imposible de descifrar.
+ **GZIP**
  + Activar la compresión Gzip puede mejorar la velocidad entre un 30% y un 70%.
  + Ahorro de ancho de banda / transferencia: nuestro sitio web enviará archivos comprimidos.
  + Velocidad del sitio.
  + Soporte en todos los navegadores actuales.
+ **Memoria Caché**
  + Evitamos tener que colver a cargar toda la web desde cero y consumir recursos del servidor innecesarios.
  + Si entras 2 veces en la misma página web y cuentas con memoria caché, el sitio cargará mucho más rápidp porque ese archivo estará almacenado en la memoria del PC, en vez del servidor de la web.
+ **CDN**; Content Delivery Network
  + Permite que los contenidos se sirvan lo más rápidp posible y aumente la velodidad de un sitio.
  + Es una red de servidores distribuidos de forma estratégica en diferentes partes del mundo.
  + *Ventajas*:
    + Alta velocidad y rendimiento
    + Ahorro de recursos
    + Mayor seguridad
+ **Favicon**
  + Imagen cuadrada de 16*16 o 32*32 de cualquier formato
  + Extensión *.ico*
  
 ```html
<link rel='icon' type='ico' href='/imagenes/favicon.ico' />
```

### Jerarquía con Urls amigables y optimizadas
+ Dominio **https://www.clicactualizado.com**
  + 1 Nivel **/juegos**
  + 2 Nivel **/juegos/playstation**
  + 3 Nivel **/juegos/playstation/minecraft**
+ Anatomia de una Url
  + https://www.clicactualizado.com/juegos/playstation/minecraft
  + Protocolo (https://)
  + Subdominio (www)
  + Dominio (clicactualizado)
  + TLD; Top Level Domain (.com)
  + Subcarpetas (juegos/playstation)
  + Páginas (minecraft)
- Separar las palabras con guiones medios.
- No deben tener caracteres especiales (tíldes, mayúsculas, signos)

### Bread Crumbs (migajas de pan)
- Muy importante para el tema de las Urls.
- Mecanismo que informa al usuario su localización dentro de la estructura jerárquica del sitio web.
- Mejor Navegabilidad y UX.
- Disminuye la tasa de rebote.
- Es un elemento en el HTML que me muestra la ruta para llegar a esa página: `juegos / playstation / minecraft`

### Microdatos
+ **Schema**
  + El marcado de datos estructurado es la forma de dotar de información semántica a una página web para que los *bots* o arañas que indexan la información la puedan entender y clasificar.
  + Qué marcados podemos lograr:
    + Artículos
    + Eventos
    + Recetas
    + Productos
    + BreadCrumb
    + Páginas de FAQ
    + Organización
    + Persona
    + Video
    + Review
- schema.org; pagina para ver los tipos más comunes de schemas.
- searchConsole; web tools > herramientas de pruebas.
- Pruebas de datos estructurados
- se incluye en el <head>:

```html
<script type='application/ld+json'>

</script>
```
### Fragmentos Destacados
+ Cluster que Google tiene en cuenta
  + Titulos con preguntas
  + H2 y H3, buena jerarquía
  + Listas en el primer párrafo del contenido
  + Tablas, columnas y filas
  + Estar en la primera página

### Vinculación de redes
- Utilizar OpenGraph Generator
- Es lo que se muestra cuando copiamos el link y lo pegamos en alguna red social.

### Alertas y buenas prácticas 
- Se utiliza *Page speed insights*
- Se coloca la Url de nuestra página, para que haga la evaluación.
- Se puede inspeccionar la página > auditar. Califica la página.

### SEO Local
- Google mybusiness, se crea la empresa.
- Aquí se configura la ubicación de mi tienda en fisico.

### Link Building
- Enlaces de nuestra página en otras páginas.
- Buscar quién está escribiendo de nosotros, pero no nos ha enlazado.
- Crear alertas de temas relacionados.
- Sugerir generación de contenido nuevo.
- Buscar nuestra página en el buscador y ver que otras páginas estan hablando de nosotros. Entrar a esas páginas y checar si tienen un link en el texto de nuestra página. Si no, tratar de contactarlos y negociar para que hagan el link building.
- Google Alerts; lo configuro para que me avise acerca de keywords, que me interesen, en contenido de otras páginas.

### Crear un diagnostico SEO
+ Estos son los aspectos SEO para tomar en cuenta:
  + Dominio
    + Canonical
    + Redirecciones
  + Indexación
    + Analytics
    + Search Console
    + Sitemap.xml
    + Robots.txt
  + Infraestructura
    + Solucion 404
    + HTTPS
    + GZip
    + Caché
    + CDN y Favicon
  + Estructura de Urls
    + Urls amigables y Jerarquía
    + Bread Crumbs
  + Optimización de contenido
    + Metadata, titulo y descripción
    + Etiquetas H, H1 única
    + Url optimizada
    + keywords en contenido
    + Anchor text
  + Contenido enriquecido
    + Microdatos
    + Fragmentos destacados
  + Social Media
    + Vinculación de redes
    + SMO - Youtube
    + OpenGraph
  + Tiempos de carga
    + Status y alertas para mejorar.
- Entrar a la página *SEO site checkup*, escanea la página en cuanto a SEO y la califica.
- Lo ideal es que un sitio no pese más de 33 kb.

### Analisis de SEO de la competencia (Benchmark)
- Identificar que esta haciendo mejor la competencia, copiarlo y mejorarlo despues.
- Utilizar  *SEO site checkup*

### Crear Reportes con Data Studio
- Se necesita cuenta de GMail
- Crear fuentes de datos (analytics, youtube, searchconsole); para crear la conexión de datos.
- Crear dashbard tipo Qliksense.

### Administración de tareas SEO constantes.
- Trabajo constante
- Debo de medir constantemente para saber que esta funcionando.
+ Monitoreo de tareas
  + Medición:
    + Tráfico orgánico (sesiones, usuarios, landing pages)
    + Posición de la keywords
    + Page Speed
    + DA y PA (Autoridad de Dominio y Autoridad de Página)
    + Indexación
    + Actualización de Sitemap
    + Envio de indexación de páginas nuevas
    + Enlaces rotos

### Recomendaciones finales
- SIEMPRE realizar un diagnóstico, al recibir una cuenta, para tener un punto cero.
- Contar con herramientas necesarias para medir y monitorear.
- Realizar benchmark y tomar las buenas prácticas de la competencia.
- Organizar de las tareas más importantes a las menos.
- Estrategias de SEO son de mediano-largo plazo.
- Tener claros los objetivos de la empresa o negocio.
- Identificar a las personas encargadas de cada labor.


