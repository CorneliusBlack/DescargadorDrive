# DescargadorDrive

**DescargadorDrive** es un gestor gratuito de descargas para Google Drive orientado a Windows. Permite organizar enlaces de archivos y carpetas, seleccionar contenido, conservar el progreso entre sesiones y descargar contenido público o contenido privado que el propio usuario haya autorizado mediante Google OAuth.

## Versión

**1.0.0**

## Funciones principales

- Cola persistente de enlaces.
- Selección de archivos dentro de carpetas.
- Reanudación y reintentos.
- Estado individual por archivo.
- Descargas públicas mediante `gdown`.
- Acceso opcional a archivos privados/autorizados mediante la API oficial de Google Drive.
- OAuth 2.0 oficial con permiso de solo lectura.
- Protección local de la autorización mediante Windows DPAPI.
- Desconexión y revocación de la autorización.
- Notificaciones y sonidos configurables.
- Datos de usuario almacenados fuera de `Program Files`.

## Privacidad

DescargadorDrive no solicita ni almacena la contraseña de Google. La autenticación se realiza directamente con Google.

Cuando el usuario decide conectar Google Drive, la aplicación solicita actualmente el permiso:

`https://www.googleapis.com/auth/drive.readonly`

Este permiso permite consultar y descargar archivos de Google Drive a los que la cuenta autorizada tenga acceso. La aplicación no solicita permiso para modificar ni eliminar archivos de Drive.

Los archivos descargados y el estado de la aplicación permanecen localmente en el equipo del usuario. Consulta [PRIVACY.md](PRIVACY.md) para más detalles.

## Distribución pública y OAuth

El código fuente no incluye tokens de usuario, sesiones OAuth, archivos DPAPI, colas, estados, historial de descargas ni configuraciones personales.

La configuración OAuth de desarrollo tampoco debe publicarse como si fuera una credencial personal. Para una distribución pública, el proyecto OAuth de producción debe configurarse y verificarse conforme a las políticas vigentes de Google antes de ofrecer autenticación a usuarios externos.

## Instalación

La versión de Windows se distribuye mediante un instalador. Python no es necesario para ejecutar el binario compilado.

Los datos modificables del usuario se almacenan en:

`%LOCALAPPDATA%\DescargadorDrive`

y se conservan al actualizar o desinstalar la aplicación, salvo que el usuario los elimine manualmente.

## Desarrollo

- Python
- Tkinter
- gdown
- Google Drive API
- Google OAuth 2.0
- Windows DPAPI
- PyInstaller
- Inno Setup

## Autoría

**Idea, diseño funcional y dirección del proyecto: Cornelius Black**

Desarrollado con asistencia de inteligencia artificial de OpenAI.

Este proyecto fue desarrollado mediante un proceso colaborativo humano-IA. La idea, requisitos, decisiones funcionales, pruebas y validación fueron dirigidos por Cornelius Black, utilizando inteligencia artificial como herramienta de apoyo para arquitectura, programación, diagnóstico y documentación.

© 2026 Cornelius Black.

## Distribución

DescargadorDrive se distribuye gratuitamente. Si resulta útil y alguien desea agradecer el trabajo realizado, puede hacerlo de manera totalmente voluntaria. Usar el programa no requiere ningún agradecimiento, aporte ni contraprestación.

## Estado

**DescargadorDrive 1.0.0 · Producción validada**
