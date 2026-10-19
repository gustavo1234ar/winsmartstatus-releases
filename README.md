# WinSmartStatus

Herramienta gratuita para diagnosticar discos (SSD, HDD y NVMe) en Windows.
Lee los datos SMART del disco y arma un informe claro: salud, uso, errores y qué hacer.

## Descargar

**[Última versión](https://github.com/gustavo1234ar/winsmartstatus-releases/releases/latest)**

- Windows 7 en adelante, 32 y 64 bits (probado en 8.1 y en 10/11).
- **No se instala**: es un solo archivo `.exe` portable.
- Pide permisos de administrador: los necesita para leer el disco.

## Cómo se usa

1. Guardá el archivo donde quieras y abrilo.
2. Si aparece el aviso de SmartScreen: **Más información** → **Ejecutar de todas formas**
   (todavía no está firmado digitalmente).
3. Elegí el disco en la lista, apretá **Analizar** y leé el panel.
4. **Copiar informe** te deja el texto listo para pegar.

## Seguridad y privacidad

- El diagnóstico es de **solo lectura**: no borra ni modifica nada del disco.
- Para mejorar el análisis envía datos SMART del disco (salud, temperatura, errores) y el
  veredicto: **no** sube el número de serie ni archivos.
- Se puede desactivar desde **Privacidad** (en la barra de abajo).

## Reportar un problema

Abrí un [issue](https://github.com/gustavo1234ar/winsmartstatus-releases/issues) contando:

- qué disco analizaste (marca y modelo),
- qué te resultó raro,
- con qué Windows lo probaste.

## Licencia

Gratis para uso técnico. No es open source: no se permite redistribuir, modificar ni
vender el ejecutable. Incluye smartctl de [smartmontools](https://www.smartmontools.org/) (GPL-2.0+).

## SHA256

sha256:3c7580b20eba458ea8bc10f017e8e9c66edd8512be3bf16f8fcbd22916521ddc
