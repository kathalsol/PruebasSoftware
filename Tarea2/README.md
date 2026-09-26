# Tarea 2

# Funcionalidades críticas

## Funcionalidades críticas

Con base en los resultados obtenidos en la lista de chequeo de la Tarea 1, se identificaron las siguientes cuatro funcionalidades críticas del sistema de Banca en Línea del Banco Nacional de Costa Rica:

### 1. Inicio de sesión y recuperación de contraseña

La persona usuaria debe poder ingresar de manera segura a Banca en Línea y recuperar el acceso si olvida sus credenciales. Esta funcionalidad es crítica porque, si falla, no se puede utilizar ningún otro servicio bancario, como consultar cuentas o realizar transferencias.

El sistema también debe impedir el acceso a páginas privadas sin autenticación y evitar que, después de cerrar sesión, sea posible volver a ellas utilizando el botón “Atrás” del navegador. Un fallo en estos controles podría bloquear el acceso legítimo o exponer información financiera confidencial.

Ver archivo Inicio-Sesion-Recuperación-Contraseña.md, en el mismo se encuentran las pruebas de esta funcionalidad.

### 2. Consulta de saldos y movimientos

La persona usuaria debe poder consultar correctamente el saldo disponible y los movimientos realizados en sus cuentas. Esta función permite verificar depósitos, retiros, pagos y transferencias, por lo que representa una parte esencial de cualquier plataforma bancaria.

Un fallo podría mostrar información financiera incorrecta y provocar decisiones equivocadas, reclamos o pérdida de confianza en el banco. Aunque esta función no aparece evaluada explícitamente en la lista de chequeo, debería incluirse en pruebas posteriores debido a su importancia.

Ver archivo Consulta-Saldos-Movimientos.md, en el mismo se encuentran las pruebas de esta funcionalidad.

### 3. Transferencias, pagos y SINPE Móvil

La persona usuaria debe poder transferir dinero y realizar pagos de forma correcta, segura y sin duplicaciones. En la lista de chequeo se comprobó que el proceso funciona y que el sistema valida datos como el número telefónico utilizado para SINPE Móvil y el monto de la transferencia.

Sin embargo, también se identificaron aspectos que podrían afectar este flujo:

- Es necesario crear una cuenta favorita para efectuar ciertas transferencias.
- Al recargar la página se borran los datos introducidos en el formulario.
- La retroalimentación visual durante el procesamiento es limitada.
- Algunos mensajes o pasos podrían resultar confusos.

Un fallo podría enviar dinero a una cuenta incorrecta, duplicar una transacción, procesar un monto equivocado o impedir que la persona usuaria cumpla una obligación financiera.

Ver archivo Transferencias-SINPE.md, en el mismo se encuentran las pruebas de esta funcionalidad.

### 4. Pagos

La persona usuaria debe poder completar correctamente hacer pagos a servicios.

Ver archivo Pagos.md, en el mismo se encuentran las pruebas de esta funcionalidad.
