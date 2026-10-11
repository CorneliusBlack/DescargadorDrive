# Preparación OAuth para distribución pública

DescargadorDrive 1.0.0 utiliza actualmente:

`https://www.googleapis.com/auth/drive.readonly`

Este permiso permite consultar y descargar archivos de Drive a los que el usuario tenga acceso.

## Antes de habilitar OAuth para usuarios externos

1. Mantener separado el proyecto OAuth usado durante desarrollo/pruebas.
2. Crear/configurar el proyecto OAuth destinado a producción.
3. Configurar la identidad pública de la aplicación como DescargadorDrive.
4. Publicar una página principal accesible públicamente.
5. Publicar la política de privacidad en el mismo dominio de la página principal.
6. Declarar exactamente los scopes utilizados por la aplicación.
7. Explicar que DescargadorDrive es una aplicación de escritorio para seleccionar y descargar localmente archivos autorizados por el propio usuario.
8. Explicar que no solicita contraseña de Google y no modifica ni elimina archivos.
9. Documentar que el contenido descargado no se envía a un servidor propio del desarrollador.
10. Completar el proceso de verificación que Google determine aplicable antes de anunciar OAuth como disponible públicamente.

No publicar el OAuth de pruebas como solución de producción.
