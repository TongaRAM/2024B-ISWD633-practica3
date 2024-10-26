### Mi aprendizaje

Antes de realizar la práctica 3, desconocía que los datos generados en un contenedor podían persistir. Pensaba que al eliminar el contenedor, toda la configuración, archivos y datos se perderían. Ahora, después de terminar la práctica, entendí que existe un mecanismo de persistencia llamado **volumen**, que permite almacenar esta información, evitando su pérdida al eliminar el contenedor. 

Los volúmenes se clasifican en:

- **Volumen de host**: monta un directorio del host en el contenedor, requiriendo especificar la ruta.
- **Volumen nombrado**: almacenado en una ubicación específica del host, identificado con un nombre único, sin necesidad de especificar la ruta.
- **Volumen anónimo**: sin nombre específico, ideal para almacenar datos temporales, cuya persistencia depende del contenedor.

Un comando útil en la práctica fue `docker volume inspect <name_volume>`, que proporciona detalles como el **Mountpoint** del volumen.
