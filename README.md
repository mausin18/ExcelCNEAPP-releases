# ExcelCNEAPP — Actualizaciones

Este repositorio público contiene únicamente los **instaladores y archivos de actualización** de ExcelCNEAPP. El código fuente se mantiene en un repositorio privado.

## Descargar

Descarga la última versión desde:

https://github.com/mausin18/ExcelCNEAPP-releases/releases/latest

El archivo recomendado es `ExcelCNEAPP-Setup-<versión>.exe`.

## Instalación

1. Descarga el instalador `.exe`.
2. Ejecútalo y elige la carpeta de instalación.
3. Abre ExcelCNEAPP desde el acceso directo creado.

Windows puede mostrar SmartScreen porque el instalador no está firmado digitalmente. Si descargaste el archivo desde esta página, usa **Más información > Ejecutar de todas formas**.

## Actualizaciones automáticas

La versión instalada comprueba este repositorio al iniciar y cada 6 horas. Cuando hay una versión nueva, la descarga y reinicia la aplicación para instalarla.

El registro de actualizaciones está en:

`%APPDATA%\excelcneapp\updates.log`

## Requisitos

- Windows 10 u 11 de 64 bits.
- No requiere Node.js ni conexión para trabajar con los datos locales.
- La sincronización con Google Sheets requiere una hoja pública y conexión a Internet.
