# Introducción

Proyecto para la creación de textos básicos con Asciidoc.

Usa este proyecto modificando únicamente el archivo `book.adoc`

## Requisitos

Debes tener instalado **Asciidoctor**, una herramienta desarrollada en Ruby que permite convertir contenido AsciiDoc a HTML5, DocBook 5 y otros formatos. Para ello, se recomienda [instalar Asciidoc FX](http://www.asciidocfx.com/). 

Asciidoc FX es un editor de documentos asciidoc (`*.adoc`) multiplataforma que pemite ver en tiempo real el resultado. Asciidoc FX permite crear  fácilmente contenidos en PDF, HTML, Epub, Mobi, Odt, Docbook, ... Dispone además de una serie de extensiones muy interesantes, como por ejemplo las que permiten trabajar con UML, hacer presentaciones HTML con Reveal.js o Deck.js, destacado de sintaxis de código fuente, símbolos matemáticos, y demás.

No obstante, también puedes instalar Asciidoctor directamente [instalando la gema asciidoctor](http://asciidoctor.org/) con este comando

```
gem install asciidoctor
```

## Consideraciones

* Las imágenes se guardarán en la carpeta `images`.

* Si el objetivo es generar un documento HTML a partir del archivo `*.adoc`, se pueden incluir videos para poder verlos. En cambio, si el objetivo es generar un documento PDF no se pueden incluir videos. Por tanto, el video de Youtube incluido en la última página producirá un error si se genera un PDF. Basta con comentarlo si se quiere generar el PDF.

```
/// video::2goMtz_vdtM[youtube, width=800, height=500]
```

## Ejemplo

En la carpeta [`samples`](samples/) puedes encontrar un ejemplo de documento, tanto el fuente (`*a.doc`) como el resultado en HTML (`*.html`). En dicho ejemplo no se podrá generar el PDF ya que contiene código Javascript para cargar fragmentos de código alojados en GitHub.