# WinSmartStatus

Herramienta gratuita para diagnosticar discos (SSD, HDD y NVMe) en Windows.
Lee los datos SMART del disco y arma un informe claro: salud, uso, errores y qué hacer.

> *English summary: WinSmartStatus is a free, portable Windows tool that reads S.M.A.R.T. data from the drives installed in a PC and produces a plain-language health report. It is a single executable: no installer, no ads, no bundled offers and no monetization of any kind.*

## Proveedor

- **Producto:** WinSmartStatus
- **Proveedor / marca:** Repabase — [repabase.com.ar](https://repabase.com.ar)
- **Contacto:** info@repabase.com.ar
- **País:** Argentina

## Descargar

**[Última versión](https://github.com/gustavo1234ar/winsmartstatus-releases/releases/latest)**

- Windows 7 SP1 en adelante, 32 y 64 bits (probado en 7, 8.1, 10 y 11).
- **Es un solo archivo `.exe`**: no se instala, no hay que descomprimir nada. Copialo donde quieras y ejecutalo.
- Pide permisos de administrador: los necesita para leer el disco.
- Cada versión publica su **SHA-256** para que puedas verificar el archivo.

## Cómo se usa

1. Ejecutá `WinSmartStatus.exe`.
2. Si aparece el aviso de SmartScreen: **Más información → Ejecutar de todas formas**
   (todavía no está firmado digitalmente).
3. Elegí el disco en la lista, apretá **Analizar** y leé el panel.
4. **Copiar informe** te deja el texto listo para pegar.

## Qué hace

Lee el S.M.A.R.T. de los discos conectados (SATA, NVMe y USB con passthrough) y muestra:

- salud: sectores reasignados y pendientes, errores, temperatura, vida útil restante;
- uso: horas encendido, encendidos, apagados bruscos;
- actividad real de escritura/lectura y amplificación de escritura (WAF) cuando el disco informa los datos necesarios;
- veredicto (OK / ATENCIÓN / CRÍTICO) y acciones concretas.

Es una herramienta de **diagnóstico**: no repara, no borra, no formatea y no modifica los datos del disco.

## Qué no hace

- No se instala ni deja servicios corriendo.
- No muestra publicidad, no incluye ofertas de terceros y no toca el navegador ni la configuración del sistema.
- No accede a tus archivos ni al contenido del disco.
- No afirma infecciones, vulnerabilidades ni problemas del sistema operativo.

## Precio

**Gratis.** Sin versión paga, sin licencias, sin funciones bloqueadas y sin ningún tipo de monetización.

## Componentes de terceros

| Componente | Versión | Licencia | Para qué se usa |
|---|---|---|---|
| `smartctl.exe` (smartmontools) | 7.5, r5714 | GPL-2.0-or-later | Lectura de los datos SMART. Se extrae a `%TEMP%` y se ejecuta como proceso separado. |
| `drivedb.h` (base de discos de smartmontools) | 8.0 + entradas propias | GPL-2.0-or-later | Nombrar correctamente los atributos según el modelo del disco. |
| Runtime de .NET | 10 | MIT | Va empaquetado dentro del `.exe` (archivo único). |

No hay otros componentes: no se usan frameworks de publicidad, telemetría de terceros ni complementos.

## Seguridad y privacidad

- El diagnóstico es de **solo lectura**: no borra ni modifica nada del disco.
- Para mejorar el análisis envía datos SMART del disco (salud, temperatura, errores) y el
  veredicto: **no** sube el número de serie, ni archivos, ni datos personales.
- Se puede desactivar desde **Privacidad** (en la barra de abajo).
- Detalle completo: [Política de privacidad](PRIVACIDAD.md).

## Licencia

Gratis para uso técnico. No es open source: no se permite redistribuir, modificar ni
vender el ejecutable. Incluye smartctl de [smartmontools](https://www.smartmontools.org/) (GPL-2.0+).
Condiciones completas: [EULA](EULA.md).

## Reportar un problema

Abrí un [issue](https://github.com/gustavo1234ar/winsmartstatus-releases/issues) contando:

- qué disco analizaste (marca y modelo),
- qué te resultó raro,
- con qué Windows lo probaste.
