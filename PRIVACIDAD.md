# Política de privacidad — WinSmartStatus

Última actualización: 28 de octubre de 2026

## 1. Quién es el responsable

**Gustavo Rul** (GitHub [@gustavo1234ar](https://github.com/gustavo1234ar)) — contacto: **gustavorul@gmail.com**.
WinSmartStatus es un programa gratuito y portable para Windows que diagnostica discos mediante S.M.A.R.T.

## 2. Resumen en una línea

La app funciona **en tu equipo**. Solo envía datos técnicos del disco, **sin datos personales y sin archivos**, y **solo si esa opción está habilitada** (se puede desactivar en cualquier momento).

## 3. Qué datos se tratan en tu equipo (no salen de ahí)

Para hacer el informe, la app lee y guarda **localmente**:

- modelo, número de serie, firmware y capacidad del disco;
- atributos S.M.A.R.T. (salud, temperatura, horas de uso, errores, desgaste);
- el informe generado y un resumen del análisis.

Eso queda en tu PC, en la carpeta de historial de la aplicación. No se accede a tus archivos, a nombres de archivos ni al contenido del disco.

## 4. Qué se envía, si está habilitado

Cuando la opción de envío está activa, la app manda al servidor del desarrollador (**repabase.com.ar**) un JSON con:

- los datos S.M.A.R.T. del disco (los mismos del punto 3);
- el veredicto y las métricas calculadas;
- un **identificador no reversible** derivado del número de serie (no se envía el serial en claro);
- contexto del análisis: si el disco estaba por USB, el modo de la controladora, el modelo de controladora y la fecha del escaneo.

**No se envía:** tus archivos, nombres de archivos, contenido del disco, tu nombre de usuario de Windows, tu IP como dato almacenado, ni ningún dato personal.

**Para qué:** comparar la evolución del mismo disco entre tomas, detectar patrones por modelo y corregir reglas de interpretación que estén mal. Es un fin estadístico y de mejora del diagnóstico.

**Dónde:** servidor propio del desarrollador, `repabase.com.ar`. No se comparte con terceros ni se vende.

## 5. Consentimiento y control

- La primera vez que abrís la app aparece un acuerdo de uso que informa de esto; sin aceptarlo la app no arranca.
- El envío se puede **desactivar o volver a activar** en cualquier momento desde el enlace **Privacidad** de la barra inferior.
- En ese mismo diálogo hay un botón **"Ver qué se envía"** que muestra exactamente el JSON que se manda, campo por campo.

## 6. Actualizaciones

La app consulta a la API pública de GitHub si hay una versión nueva. Esa consulta no envía datos del disco; GitHub ve la IP de origen como en cualquier visita a un sitio web. La descarga de la actualización la decide el usuario y el archivo se verifica con su SHA-256 antes de reemplazar el anterior.

## 7. Conservación y borrado

Los datos enviados se conservan para poder comparar la evolución del disco en el tiempo. Podés pedir la eliminación de todos los datos asociados a un disco escribiendo a **gustavorul@gmail.com**: se borran y se confirma por correo.

## 8. Publicidad y perfilado

No hay publicidad, no hay perfilado de usuarios, no se usan cookies ni identificadores de seguimiento, y no se comparte información con anunciantes.

## 9. Menores

La app es una herramienta técnica y no está dirigida a menores. No se recogen datos personales de ninguna persona.

## 10. Cambios

Si esta política cambia, se actualiza la fecha del encabezado y el cambio se describe en las notas de la versión correspondiente.
