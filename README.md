# ExcelCNEAPP — Actualizaciones

Este repositorio público contiene únicamente los **instaladores y archivos de actualización** de ExcelCNEAPP. El código fuente se mantiene en un repositorio privado.

## Descargar

Descarga la última versión desde:

https://github.com/mausin18/ExcelCNEAPP-releases/releases/latest

El archivo recomendado es `ExcelCNEAPP-Setup-<versión>.exe`.

Versión actual: **[v1.1.0](https://github.com/mausin18/ExcelCNEAPP-releases/releases/tag/v1.1.0)**.

## Novedades de 1.1.0

- Colaboración LAN en tiempo real: nombres, celda activa, cursor y cambios por celda.
- Escritura opcional en Google Sheets mediante un Web App de Apps Script.
- Sincronización optimizada por parches de celda.
- Plantilla de Apps Script incluida en la app.

## Instalación

1. Descarga el instalador `.exe`.
2. Ejecútalo y elige la carpeta de instalación.
3. Abre ExcelCNEAPP desde el acceso directo creado.

Windows puede mostrar SmartScreen porque el instalador no está firmado digitalmente. Si descargaste el archivo desde esta página, usa **Más información > Ejecutar de todas formas**.

## Verificar el instalador

Archivo: `ExcelCNEAPP-Setup-1.1.0.exe`

SHA-256:

```text
71855beef14e06dc8b6808970ba0988235da33510db58c6e28136f445c84bb50
```

SHA-512:

```text
c7cbd315989e91a07f3b004e71cda95da18174503c1f418bca8993e88b01a8d0286ff7bfb97e44c9a4d4e4d64f77bf77be56bd7f6a5f45728f36b931e63d1f6a
```

Puedes comprobarlo en PowerShell:

```powershell
Get-FileHash .\ExcelCNEAPP-Setup-1.1.0.exe -Algorithm SHA256
```

El hash debe coincidir exactamente. También puedes descargar `SHA256SUMS.txt` desde la release y comparar el instalador, el blockmap y `latest.yml`.

## Actualizaciones automáticas

La versión instalada comprueba este repositorio al iniciar y cada 6 horas. Cuando hay una versión nueva, la descarga y reinicia la aplicación para instalarla.

`latest.yml` incluye el SHA-512 que usa `electron-updater` para validar la descarga. El registro de actualizaciones está en:

`%APPDATA%\excelcneapp\updates.log`

## Requisitos

- Windows 10 u 11 de 64 bits.
- No requiere Node.js ni conexión para trabajar con los datos locales.
- La colaboración LAN requiere que los equipos estén en la misma red y permite la app en el Firewall de Windows.
- La lectura de Google Sheets requiere una hoja pública y conexión a Internet.
- La escritura en Google Sheets requiere desplegar el Web App de Apps Script incluido en la app.

## Código fuente

El código fuente no se publica en este repositorio. Aquí solo se distribuyen los instaladores, actualizaciones y hashes de verificación.
