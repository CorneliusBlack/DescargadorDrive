# Política de privacidad de DescargadorDrive

**Última actualización: 10 de octubre de 2026**

## 1. Alcance

Esta política describe cómo DescargadorDrive trata la información cuando el usuario utiliza la aplicación de escritorio para Windows.

## 2. Inicio de sesión con Google

La conexión con Google Drive es opcional. La autenticación se realiza mediante el sistema OAuth oficial de Google. DescargadorDrive no solicita, recibe ni almacena la contraseña de la cuenta de Google.

## 3. Datos de Google Drive

Cuando el usuario conecta su cuenta, DescargadorDrive solicita actualmente el permiso de solo lectura `https://www.googleapis.com/auth/drive.readonly`.

La finalidad de este acceso es permitir que el usuario consulte carpetas y archivos de Google Drive a los que ya tiene acceso y descargue localmente los elementos que seleccione.

DescargadorDrive no utiliza este permiso para modificar, subir o eliminar archivos de Google Drive.

## 4. Almacenamiento

La aplicación guarda localmente datos necesarios para su funcionamiento, como configuración, cola de enlaces, estado de descargas y autorización OAuth protegida mediante Windows DPAPI.

Estos datos se almacenan en `%LOCALAPPDATA%\DescargadorDrive`.

Los archivos descargados se guardan en la ubicación elegida por el usuario.

## 5. Transmisión y terceros

DescargadorDrive se comunica con Google únicamente cuando es necesario para autenticar al usuario y consultar o descargar contenido autorizado mediante los servicios de Google.

La aplicación no vende datos personales ni utiliza los datos obtenidos desde las APIs de Google para publicidad.

La aplicación no está diseñada para enviar a un servidor propio del desarrollador el contenido descargado desde Google Drive.

## 6. Uso limitado de datos de Google

Los datos obtenidos mediante las APIs de Google se utilizan exclusivamente para proporcionar las funciones visibles de consulta y descarga solicitadas por el usuario. El uso de estos datos debe mantenerse de acuerdo con la Google API Services User Data Policy y sus requisitos de Limited Use.

## 7. Desconexión

El usuario puede utilizar la función de desconexión de Google dentro de DescargadorDrive. La aplicación intenta revocar la autorización OAuth y elimina de su almacenamiento local la autorización protegida asociada.

El usuario también puede administrar el acceso de aplicaciones de terceros desde su Cuenta de Google.

## 8. Eliminación de datos locales

El usuario controla los datos almacenados localmente. La desinstalación conserva deliberadamente `%LOCALAPPDATA%\DescargadorDrive` para permitir actualizaciones o reinstalaciones sin perder el progreso. Si desea eliminar completamente los datos locales, puede borrar esa carpeta después de cerrar la aplicación y revocar previamente el acceso de Google si corresponde.

## 9. Seguridad

La autorización OAuth local se protege mediante Windows DPAPI. Ningún mecanismo de seguridad puede garantizar riesgo cero, por lo que las futuras versiones deben mantener actualizadas sus dependencias y revisar cualquier cambio en el tratamiento de datos.

## 10. Cambios

Los cambios relevantes en el acceso, uso, almacenamiento o intercambio de datos deberán reflejarse en una versión actualizada de esta política antes de distribuir la funcionalidad correspondiente.

## 11. Autoría pública

DescargadorDrive es un proyecto de Cornelius Black desarrollado mediante colaboración humano-IA.

Esta política evita publicar información personal del desarrollador. Los datos de contacto que eventualmente exija una plataforma de distribución u OAuth deberán configurarse de forma separada y deliberada para ese propósito.
