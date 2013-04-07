# Bienvenido a Dealer Ergo Go

Como el próximo 1 de Julio de 2013 nos quedamos sin Google Reader, me ha parecido una buena idea empezar a probar Helios haciendo un servicio donde se almacenen todos los feeds de forma semejante a como lo hace Google Reader. Creo que con los blogs tengo un poco de _síndrome de Diógenes_ y el hecho de que haya un sitio donde este todo guardado para cuando me de por buscar al que me _suene haber leido_ me da mucha tranquilidad.

Esto no es más que un juego sin pretensiones. A ver hasta donde llega.

De momento, el modelo solo tiene dos entidades: feed e item.      
Para la extracción de los feeds quiero utilizar el propio _extractor_ de Google Reader ya que siempre devuelve los datos en el mismo formato, independientemente de si la fuente es atom o rss. Un ejemplo de la url sería el siguiente:

[http://www.google.com/reader/api/0/stream/contents/feed/{escaped-url-feed}?n=1000](http://www.google.com/reader/api/0/stream/contents/feed/{escaped-url-feed}?n=1000)

Si sustituimos {escaped-url-feed} por la url del feed que queremos descargar, obtendremos un bonito json.

No es necesario estar autenticado en el servicio de Google Reader así que es una buena aproximación para incluirlo en una aplicación sin complicarnos demasiado la vida. Supongo que también desaparecerá el 1 de Julio pero, con un poco de suerte, publicarán su código fuente un poco antes. </tururu>

Se supone que debería haber un proyecto anexo a este con la integración en iOS. Ahora mismo tengo una aplicación que graba y lee pero que en ocasiones da un error grave al encontrar registros _corruptos_ en la base de datos de Core Data. A ver si lo soluciono y subo el repositorio a GitHub.

Si os interesa probarlo pero no os apetece cimeros la cabeza haciendo despliegues, descargando el repositorio y arrancándolo en vuestra máquina, etc, poneos en contacto conmigo. Os facilitaré un dominio, un usuario y una contraseña para hacer pruebas.
