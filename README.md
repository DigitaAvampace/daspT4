Para examenes
# Examen Interactivo sobre el Tema 4 de Digitalización

Este proyecto es una aplicación web interactiva que permite a los usuarios seleccionar y realizar exámenes relacionados con el Tema 4 de Digitalización. Los exámenes se cargan dinámicamente desde archivos JSON ubicados en el repositorio.

## Estructura del Proyecto

- **index.html**: Archivo principal que contiene la estructura HTML, estilos y lógica JavaScript para cargar y evaluar los exámenes.
- **indice.json**: Archivo JSON que lista los exámenes disponibles.
- **examenes/**: Carpeta que contiene los archivos JSON de cada examen (por ejemplo, `Examen_1_IA_Produccion.json`, `Examen_2_IA_Produccion.json`, etc.).
- **.nojekyll**: Archivo vacío (opcional) que previene que GitHub Pages procese el sitio con Jekyll, asegurando que se sirvan los archivos tal como están.

## Instrucciones de Uso

### Uso Local

1. **Clonar el Repositorio:**

   Abre una terminal y ejecuta:

   ```bash
   git clone https://github.com/DigitaAvampace/daspT4.git

   cd daspT4
# Para Python 3.x
python3 -m http.server

Despliegue en GitHub Pages
Configurar GitHub Pages:

Ve a la pestaña Settings de tu repositorio en GitHub.
Dirígete a la sección Pages.
Selecciona la rama main (o la rama que contenga tu index.html) y la carpeta raíz (o la carpeta correcta).
Agregar el Archivo .nojekyll:

Para evitar que GitHub Pages procese tu sitio con Jekyll (lo cual puede afectar la estructura de archivos estáticos), crea un archivo vacío llamado .nojekyll en la raíz del repositorio.

Realizar Commit y Push:

Asegúrate de que todos los cambios (incluido el .nojekyll) estén comprometidos y subidos a la rama configurada para GitHub Pages.

Verificar el Sitio:

Una vez completado el proceso, GitHub Pages publicará tu sitio y podrás acceder a él mediante la URL indicada en la sección Pages de la configuración del repositorio.

Solución de Problemas
Los exámenes no se cargan al hacer clic en los botones:

Verifica en la consola del navegador (F12) si hay errores de red o problemas con la estructura de los archivos JSON.
Asegúrate de que la variable baseUrl en index.html esté configurada correctamente para apuntar a la ruta donde se encuentran los archivos JSON.
Revisa que la estructura de los archivos JSON (tanto en indice.json como en los exámenes) coincida con lo esperado (por ejemplo, que existan las propiedades "preguntas", "respuestas_correctas" y "banco_explicaciones").
Build cancelado en GitHub Actions:

Asegúrate de que la configuración del workflow en GitHub Actions esté correcta.
Comprueba si se requiere agregar el archivo .nojekyll para evitar problemas con Jekyll.
Revisa los logs de GitHub Actions para identificar mensajes de error específicos y ajustar la configuración según sea necesario.
Notas Adicionales
El archivo indice.json puede utilizar rutas con o sin un slash inicial. Si utilizas rutas con slash inicial, asegúrate de que baseUrl no termine en slash para evitar dobles barras en la URL.
Se han incluido mensajes de depuración (console.log) en index.html para facilitar la identificación de problemas durante el proceso de carga de exámenes.
Contribuciones
Si deseas contribuir a este proyecto, por favor abre un issue o un pull request describiendo las mejoras o correcciones que propones.
