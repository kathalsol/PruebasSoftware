# Tarea 4: Propuestas de mejoras de UI y UX para Transferencias y SINPE Móvil

## Base del análisis

Se utilizan los casos de prueba de [Transferencias y SINPE de la Tarea 2](../Tarea2/Transferencias-SINPE.md), su [resumen de funcionalidades críticas](../Tarea2/README.md) y las capturas de [transferencia BN](../Tarea2/Transaccion-BN.png), [aviso SINPE](../Tarea2/Error-SINPE.png) y [transferencias hacia otros bancos](../Tarea2/Transferencia-Otros-Bancos.png).

La Tarea 2 documenta una transferencia BN realizada, la exigencia de cuentas favoritas y el bloqueo de SINPE Móvil sin afiliación. Los casos de otros bancos acreditan el llenado del formulario, pero no describen un comprobante de ejecución; no se se completaron esas transferencias.

## Mejora 1: Reducir pasos de navegación y explicar el requisito de cuentas favoritas

**Hallazgo y evidencia**

CT-010 identifica una página intermedia con una imagen grande y dos enlaces: “Realizar transferencia” y “Consultar transferencias otros bancos”. Además, CT-008, CT-010 y CT-011 indican que se necesita una cuenta favorita previamente creada. En el formulario BN, el destino se elige mediante “Seleccionar cuenta”, sin que la captura explique ese requisito.

**Propuesta de UI y UX**

- Presentar accesos claros a “Entre cuentas BN”, “Hacia otros bancos”, “Desde otros bancos” y “SINPE Móvil”, que conduzcan al flujo correspondiente. Mantener el historial como una acción secundaria visible.
- En la selección del destino, usar “Seleccionar cuenta favorita” y explicar por qué debe registrarse previamente. Si no hay favoritas, mostrar esa situación y la acción “Registrar cuenta favorita”, en lugar de dejar la persona usuaria sin orientación.
- Permitir regresar al formulario después del registro y conservar únicamente un borrador temporal dentro de la sesión autenticada. Mantener las verificaciones actuales para crear favoritas y no ejecutar ninguna transferencia automáticamente al regresar.

**Beneficio esperado**

Reducir pasos que no aportan información y evitar que la persona usuaria descubra tarde un requisito que le impide continuar.

**Criterios de evaluación**

- Elegir “Hacia otros bancos” abre el flujo de transferencia sin atravesar una pantalla meramente decorativa.
- Cuando no existen favoritas, se explica el requisito y se ofrece el acceso al registro.
- Al volver del registro, se puede continuar con el borrador sin omitir validaciones ni enviar dinero; al cerrar la sesión, el borrador se elimina.

## Mejora 2: Mejorar la jerarquía del formulario y la revisión de los datos

**Hallazgo y evidencia**

La captura de transferencia BN presenta cuentas, monto, moneda, detalle, otro depositante y dos campos de correo en un mismo formulario. Las instrucciones de las casillas opcionales son extensas y los enlaces “Límite diario” y “Tipo de cambio” aparecen separados del monto.

**Propuesta de UI y UX**

- Agrupar los campos en “Origen y destino”, “Monto y moneda” y “Opciones adicionales”. Mantener contraídas las opciones de otro depositante y notificación hasta que se activen, con etiquetas distintas para cada correo.
- Mostrar junto al monto el límite aplicable y, cuando haya conversión, el tipo de cambio, su vigencia y el importe que se debitará. Validar los datos con mensajes específicos que conserven lo digitado.
- Reemplazar “Continuar” por “Revisar transferencia”. Antes de la autorización final, presentar un resumen con beneficiario, cuenta parcialmente oculta, banco, moneda, monto y comisiones aplicables, permitiendo volver a editar sin perder el formulario.

**Beneficio esperado**

Reducir la carga visual y facilitar la detección de un destino, una moneda o un monto incorrectos antes de autorizar la operación.

**Criterios de evaluación**

- Se puede completar una transferencia sin recorrer los campos opcionales que no se han activado.
- Un monto inválido genera una explicación junto al campo; los límites y la conversión aplicables son visibles antes de autorizar.
- El resumen coincide con los datos ingresados y permite corregirlos antes del envío. Estas condiciones deben comprobarse en todos los tipos de transferencia donde correspondan.

## Mejora 3: Informar requisitos y estados de la operación sin inducir reintentos

**Hallazgo y evidencia**

CT-009 y su captura muestran el aviso de afiliación a SINPE Móvil después de haber digitado datos de transferencia. El mensaje ofrece “¡AFÍLIATE AQUÍ!” y “SALIR”, pero no explica explícitamente si se realizó algún envío. El resumen de la Tarea 2 también señala pérdida de datos al recargar y retroalimentación limitada durante el procesamiento.

**Propuesta de UI y UX**

- Comprobar la afiliación al abrir SINPE Móvil, antes de solicitar monto y teléfono. Si falta, mostrar “Necesitas afiliarte a BN SINPE Móvil para transferir. No se ha enviado dinero”, con las acciones “Iniciar afiliación” y “Volver a transferencias”.
- Durante el envío, mostrar “Procesando transferencia…” y bloquear nuevos envíos de esa misma operación, sin bloquear la consulta de estado. La protección contra duplicados debe existir también en el procesamiento, no depender solo de deshabilitar un botón.
- Diferenciar operación confirmada, rechazada y resultado pendiente de verificar. Ofrecer comprobante únicamente con confirmación; si se pierde la conexión o se recarga después de enviar, consultar el estado de la operación en lugar de reenviarla. Conservar borradores solo antes del envío y dentro de la sesión autenticada, sin almacenar credenciales ni OTP.

**Beneficio esperado**

Evitar llenar un formulario que no se puede utilizar y reducir la incertidumbre que podría llevar a repetir una transferencia.

**Criterios de evaluación**

- Una persona sin afiliación ve el requisito antes de completar el formulario SINPE y no se inicia ningún envío.
- Un doble clic en la autorización no produce dos operaciones; debe verificarse tanto en la interfaz como en el procesamiento.
- Una interrupción posterior al envío muestra un estado pendiente de verificar y permite consultar el resultado sin reenviar. El éxito y el comprobante solo aparecen después de confirmar la operación.
