# Seguridad

## Reporte de vulnerabilidades

No publiques tokens OAuth, archivos `.dpapi`, `credentials.json`, enlaces privados de Drive, datos personales ni archivos de estado en un issue público.

Mientras el proyecto no disponga de un canal público específico de seguridad, conserva cualquier evidencia sensible fuera del repositorio.

## Datos que nunca deben entrar al repositorio

- `credentials.json`
- `token_oauth_beta.json`
- `token_oauth_beta.dpapi`
- `estado_descargas.json`
- `cola_enlaces.json`
- `configuracion.json`
- `revision_manual.txt`
- archivos descargados
- logs personales
- capturas con correos, nombres, IDs o enlaces privados
- builds locales que contengan material no auditado

## Modelo local

DescargadorDrive mantiene sus datos de ejecución bajo `%LOCALAPPDATA%\DescargadorDrive`. Ese directorio no forma parte del repositorio.
