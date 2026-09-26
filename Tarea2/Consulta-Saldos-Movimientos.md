# Caso de Prueba 1: Revisión de Saldo Cuenta Bancaria

## ID

CT-005

## Objetivo

Verificar que se pueda observar bien el saldo de la cuenta bancaria y tener acceso a ver el detalle de los movimientos.

## Precondiciones

- Haber iniciado sesión a Banca en línea
- Tener una cuenta bancaria activa

## Datos de Entrada

- Para iniciar sesión en Banca en línea.
- Nombre de usuario: Kathy1234
- Contraseña: Prueba123
- Código OTP válido.

## Pasos

1. Acceder a la página de Banca en Línea.
2. Ingresar el nombre de usuario y la contraseña en el formulario.
3. Hacer clic en el botón "Iniciar sesión".
4. Digitar el código OTP solicitado como segunda verificación.
5. Presionar el botón "Continuar".
6. Seleccionar el botón "Cuentas" de la barra superior.
7. En la sección Corrientes y Ahorros, seleccionar la opción Saldos y Movimientos.

## Resultado Esperado

- Se puede visualizar correctamente el saldo y la cuenta bancaria.
- Aparece en la misma página una opción para ver los movimientos de la cuenta si quisieramos.

## Resultado Obtenido

- Se obtuvo el resultado esperado sin errores en el sistema.

## Estado de la prueba

✅ Pasó

## Observaciones

- Se observa que en la misma página despliegan información para hacer un ahorro programado, administrar el dinero con Sobres y también transferir o hacer pagos, lo cual es mucha información en el mismo lugar. 

# Caso de Prueba 2: Revisión de Movimientos Bancarios en un rango de días específico

## ID

CT-006

## Objetivo

Verificar que se pueda observar los movimientos bancarios de un rango definido de días.

## Precondiciones

- Haber iniciado sesión a Banca en línea
- Tener una cuenta bancaria activa
- Tener transacciones en el rango de días definido para poder observarlas.

## Datos de Entrada

- Para iniciar sesión en Banca en línea.
- Nombre de usuario: Kathy1234
- Contraseña: Prueba123
- Código OTP válido.

## Pasos

1. Acceder a la página de Banca en Línea.
2. Ingresar el nombre de usuario y la contraseña en el formulario.
3. Hacer clic en el botón "Iniciar sesión".
4. Digitar el código OTP solicitado como segunda verificación.
5. Presionar el botón "Continuar".
6. Seleccionar el botón "Cuentas" de la barra superior.
7. En la sección Corrientes y Ahorros, seleccionar la opción Saldos y Movimientos.
8. En la opción de Detalles y Movimientos
9. Se selecciona la cuenta y se pone la fecha inicial y final de las transacciones a ver y se selecciona el botón "Procesar".
10. Se despliega la tabla con las trasacciones en la fecha seleccionadas.

## Resultado Esperado

- Se puede visualizar correctamente el saldo y la cuenta bancaria.
- Después de seleccionar el rango de fechas
- Se visualiza la tabla con las transacciones

## Resultado Obtenido

- Se obtuvo el resultado esperado sin errores en el sistema.

## Estado de la prueba

✅ Pasó

## Observaciones

- Si no hay transferencias en el rango seleccionado igual muestra una tabla con ningún valor.

# Caso de Prueba 3: Revisión de Movimientos Bancarios seleccionando "mayor igual a" qué monto.

## ID

CT-007

## Objetivo

Verificar que se pueda observar las transacciones bancarias  mayores que el monto establecido en el sistema dentro del rango de días seleccionado.

## Precondiciones

- Haber iniciado sesión a Banca en línea
- Tener una cuenta bancaria activa
- Tener transacciones en el rango de días definido para poder observarlas (opcional).

## Datos de Entrada

- Para iniciar sesión en Banca en línea.
- Nombre de usuario: Kathy1234
- Contraseña: Prueba123
- Código OTP válido.

## Pasos

1. Acceder a la página de Banca en Línea.
2. Ingresar el nombre de usuario y la contraseña en el formulario.
3. Hacer clic en el botón "Iniciar sesión".
4. Digitar el código OTP solicitado como segunda verificación.
5. Presionar el botón "Continuar".
6. Seleccionar el botón "Cuentas" de la barra superior.
7. En la sección Corrientes y Ahorros, seleccionar la opción Saldos y Movimientos.
8. En la opción de Detalles y Movimientos
9. Se selecciona la cuenta y se pone la fecha inicial y final de las transacciones a ver.
10. Se puede seleccionar el monto "menor igual a", "mayor igual a" y "igual a" (para este caso se escogío mayor igual a)y se digita el valor del monto. Luego se selecciona el botón "Procesar".
10. Se despliega la tabla con las trasacciones en la fecha seleccionadas y con la condición seleccionada.

## Resultado Esperado

- Se puede eleccionar el rango de fechas
- Se visualiza la tabla con las transacciones y con el rango de valores según la seleccion realizada.
- El valor digitado no pueden ser letras o caracteres extraños.

## Resultado Obtenido

- Se obtuvo el resultado esperado sin errores en el sistema.

## Estado de la prueba

✅ Pasó

## Observaciones

- No hay.

# Caso de Prueba 4: Revisión de Movimientos Bancarios seleccionando "igual a" qué monto.

## ID

CT-008

## Objetivo

Verificar que se pueda observar las transacciones bancarias iguales que al monto establecido en el sistema dentro del rango de días seleccionado.

## Precondiciones

- Haber iniciado sesión a Banca en línea
- Tener una cuenta bancaria activa
- Tener transacciones en el rango de días definido para poder observarlas (opcional).

## Datos de Entrada

- Para iniciar sesión en Banca en línea.
- Nombre de usuario: Kathy1234
- Contraseña: Prueba123
- Código OTP válido.

## Pasos

1. Acceder a la página de Banca en Línea.
2. Ingresar el nombre de usuario y la contraseña en el formulario.
3. Hacer clic en el botón "Iniciar sesión".
4. Digitar el código OTP solicitado como segunda verificación.
5. Presionar el botón "Continuar".
6. Seleccionar el botón "Cuentas" de la barra superior.
7. En la sección Corrientes y Ahorros, seleccionar la opción Saldos y Movimientos.
8. En la opción de Detalles y Movimientos
9. Se selecciona la cuenta y se pone la fecha inicial y final de las transacciones a ver.
10. Se puede seleccionar el monto "menor igual a", "mayor igual a" y "igual a" (para este caso se escogío igual a)y se digita el valor del monto. Luego se selecciona el botón "Procesar".
10. Se despliega la tabla con las trasacciones en la fecha seleccionadas y con la condición seleccionada.

## Resultado Esperado

- Se puede eleccionar el rango de fechas
- Se visualiza la tabla con las transacciones y con el rango de valores según la seleccion realizada.
- El valor digitado no pueden ser letras o caracteres extraños.

## Resultado Obtenido

- Se obtuvo el resultado esperado sin errores en el sistema.

## Estado de la prueba

✅ Pasó

## Observaciones

- No hay.