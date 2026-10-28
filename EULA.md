# Condiciones de uso (EULA) — WinSmartStatus

Última actualización: 28 de octubre de 2026

Al ejecutar WinSmartStatus aceptás estas condiciones. Si no estás de acuerdo, no uses el programa.

## 1. Qué es

WinSmartStatus es una herramienta **gratuita** de diagnóstico de discos para Windows. Lee los datos S.M.A.R.T. del disco, los interpreta y muestra un informe con un veredicto y acciones sugeridas.

## 2. Licencia de uso

Se concede una licencia gratuita, no exclusiva e intransferible para usar el programa, con fines personales o profesionales.

- **Podés** usarlo en todos los equipos que necesites, y compartir el enlace oficial de descarga.
- **No podés** redistribuir, modificar ni vender el ejecutable, ni quitar los avisos de autoría o de licencias de terceros.

## 3. Qué hace en el equipo

Para funcionar, la app:

1. **Pide permisos de administrador**, necesarios para leer los discos físicos.
2. **Extrae `smartctl.exe` a `%TEMP%`** y lo ejecuta como **proceso separado** para leer el S.M.A.R.T.
3. Consulta información del sistema **solo para identificar el disco y su controladora** (WMI, registro de Windows, consultas al driver del disco).
4. Guarda **dos claves en `HKCU\Software\WinSmartStatus`**: si se aceptó el acuerdo de uso y si el envío de datos está habilitado.
5. **Opcionalmente**, y solo cuando el usuario lo pide con el botón correspondiente, ejecuta `defrag <letra> /L` sobre la unidad seleccionada (ReTrim del espacio libre del SSD). No se ejecuta nunca por sí sola.
6. **Se actualiza a sí misma solo con confirmación del usuario**: descarga el nuevo `.exe`, verifica su SHA-256, reemplaza el actual y guarda el anterior. No instala nada más.

No modifica otros programas, no cambia la configuración del sistema, no toca el navegador ni los archivos del usuario.

## 4. Componentes de terceros y licencias

- **`smartctl.exe`** (smartmontools 7.5) y **`drivedb.h`** (base de datos de discos) están bajo **GPL-2.0-or-later**. Se usan como programa separado, invocado por línea de comandos.
- **Runtime de .NET 10**, bajo licencia MIT, empaquetado dentro del `.exe`.

El código propio de WinSmartStatus **no está cubierto por la GPL** (no se enlaza con smartctl: se ejecuta como proceso independiente). El texto de la licencia de smartmontools se muestra dentro de la app, en el diálogo **Privacidad**.

## 5. Datos

El tratamiento de datos se describe en la [política de privacidad](PRIVACIDAD.md). El envío de datos técnicos del disco es opcional y se puede desactivar en cualquier momento.

## 6. Sin garantía

El programa se entrega **"tal cual"**, sin garantía de ningún tipo. El informe es una **ayuda al diagnóstico**: no reemplaza el criterio del técnico, ni un respaldo de los datos, ni el servicio técnico oficial del fabricante.

Un veredicto favorable **no garantiza** que el disco no vaya a fallar. Un veredicto desfavorable **no obliga** a reemplazarlo: es una recomendación basada en los datos que el propio disco informa.

## 7. Límite de responsabilidad

En la medida en que la ley lo permita, Repabase no es responsable por daños directos o indirectos, pérdida de datos o lucro cesante derivados del uso o de la imposibilidad de usar el programa. Es responsabilidad del usuario **mantener respaldos** de su información.

## 8. Cambios

Estas condiciones pueden actualizarse. La versión vigente es siempre la publicada en esta página, con su fecha de actualización.

## 9. Contacto y legislación

Contacto: **info@repabase.com.ar** — [repabase.com.ar](https://repabase.com.ar).
Estas condiciones se rigen por las leyes de la República Argentina.
