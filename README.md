# pc - pepecine bash webscrapper

## Introducción

Se trata de un pequeño web scrapper para extraer enlaces de una película de pepecine.

Simplemente invocar "pc cadena de búsqueda", donde "cadena de búsqueda" puede ser un nombre completo o parcial. Debido a las limitaciones de pepecine, solo se devuelven doce resultados como máximo, por lo que no se recomienda buscar cosas como "a". Otra cosa que hace pepecine es que si no encuentra nada relevante, aún así te da sugerencias como si fuesen resultados normales. El usuario deberá tenerlo en cuenta.
Es interactivo.

El script reproduce automáticamente la peli con mpv, lo cual funcionará solo si el servicio de streaming es compatible con youtube-dl.
Esto convierte a youtube-dl en una dependencia deseable aunque no obligatoria, ya que también se puede abrir el enlace en el navegador. 

Además de las dependencias, el script no requiere configuración previa. Simplemente copiarlo a /usr/local/bin o a la carpeta bin de tu carpeta personal y está funcionando.

## Dependencias

* curl (obligatoria)
* youtube-dl (deseable)
* mpv (deseable)
