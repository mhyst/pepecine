# pc - pepecine bash webscrapper

## Introducción

Se trata de un pequeño web scrapper escrito en bash cuyo objetivo es extraer enlaces de una película de pepecine.


### Funcionamiento

Simplemente invocar "pc cadena de búsqueda", donde "cadena de búsqueda" puede ser un nombre completo o parcial.

Una vez en ejecución, el script permitirá al usuario la selección de película y enlace de forma interactiva. A continuación, el script tratará de reproducir automáticamente la peli con el reproductor mpv, lo cual funcionará solo si el servicio de streaming es compatible con youtube-dl. Esto convierte a youtube-dl en una dependencia deseable aunque no obligatoria, ya que también se puede abrir el enlace en el navegador. También, si se desea, con una modificación sencilla en la última línea del script, se puede utilizar el reproducor vlc o cualquier otro.

Además de las dependencias que veremos más abajo, el script no requiere ninguna configuración previa. Simplemente copiarlo a /usr/local/bin o a la carpeta bin de tu carpeta personal y está funcionando.


### Ejemplos de uso:

>pc la ventana indiscreta
>pc ventana


## Dependencias

* curl (obligatoria)
* youtube-dl (deseable)
* mpv (deseable)


## Consideraciones finales

Debido a las limitaciones de pepecine, solo se devuelven doce resultados como máximo, por lo que no se recomienda utilizar una cadena de búsqueda demasiado genérica. Otra cosa que hace pepecine es que si no encuentra nada relevante, aún así te da sugerencias como si fuesen resultados normales. El usuario deberá tenerlo en cuenta.
