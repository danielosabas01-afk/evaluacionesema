# EMA MAYOREO WEB

Este repositorio prepara la publicación web de EMA MAYOREO.

## Importante: GitHub Pages no ejecuta el servidor de EMA

La versión original usa `web_server.py`, `data_engine.py`, una base SQLite y endpoints `/api/*` para importar Excel, administrar periodos, auditar datos y generar comparativos. GitHub Pages publica archivos estáticos y no puede ejecutar Python ni mantener esa base de datos. Publicar solamente `web/index.html` haría que varias funciones fallen con errores como `Failed to fetch`.

## Publicación prevista

- GitHub Pages: alojamiento público de archivos estáticos y portal del proyecto.
- Servicio Python: necesario para usar la aplicación completa y guardar cambios entre sesiones.
- Datos de ventas: no se incluyen en el repositorio público por defecto; los archivos históricos `.xlsx`, `.db` y los respaldos deben mantenerse privados.

La app original y sus datos deben separarse antes de habilitar una URL pública con acceso a información empresarial. No se debe considerar que todas las funciones están disponibles hasta comprobar el backend y las operaciones de importación.
