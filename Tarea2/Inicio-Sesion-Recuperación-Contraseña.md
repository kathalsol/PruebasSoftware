# Caso de Prueba 1: Inicio de Sesión desde la página web

## ID

CT-001

## Objetivo

Verificar que se pueda iniciar sesión correctamente desde la página web.

## Precondiciones

- Usuario con una cuenta existente.
- Acceso a un navegador actualizado.
- Conexión estable a Internet.
- Tener la aplicación móvil del BN para acceder al código OTP (One-Time Password).

## Datos de Entrada

- Nombre de usuario: Kathy1234
- Contraseña: Prueba123
- Código OTP válido.

## Pasos

1. Acceder a la página de Banca en Línea.
2. Ingresar el nombre de usuario y la contraseña en el formulario.
3. Hacer clic en el botón "Iniciar sesión".
4. Digitar el código OTP solicitado como segunda verificación.
5. Presionar el botón "Continuar".

## Resultado Esperado

- La persona usuaria es redirigida inicialmente a la página de verificación del código OTP.
- Después de verificar el código, la persona usuaria ingresa a Banca en Línea.
- No aparecen errores visibles.

## Resultado Obtenido

- Se obtuvo el resultado esperado sin errores en el sistema.

## Estado de la prueba

✅ Pasó

## Observaciones

- El código OTP debe utilizarse dentro del periodo de validez indicado por el sistema.

# Caso de Prueba 2: Inicio de Sesión desde la aplicación móvil

## ID

CT-002

## Objetivo

Verificar que una persona usuaria pueda iniciar sesión correctamente desde la aplicación móvil del Banco Nacional.

## Precondiciones

- Usuario con una cuenta existente y acceso habilitado a Banca Móvil.
- Aplicación móvil del Banco Nacional instalada y actualizada.
- Dispositivo móvil asociado a la cuenta.
- Conexión estable a Internet.
- Acceso al número de teléfono registrado para recibir el código de verificación.

## Datos de Entrada

- Nombre de usuario: Kathy1234
- Contraseña: Prueba123

## Pasos

1. Abrir la aplicación móvil del Banco Nacional.
2. Digitar el nombre de usuario y seleccionar el botón "Siguiente".
3. Ingresar la contraseña.
4. Seleccionar un medio para enviar código de verificación, puede ser el número de teléfono o correo.
5. Digitar el código de verificación y presionar el botón "Aceptar".


## Resultado Esperado

- La aplicación acepta las credenciales válidas.
- El sistema solicita numero o correo para enviar código como método adicional de verificación.
- Después de validar el código, BN consultas en la aplicación movil.
- La información de las cuentas pertenece a la persona usuaria autenticada.
- No aparecen errores visibles.

## Resultado Obtenido

- Se obtuvo el resultado esperado y fue posible ingresar correctamente a la aplicación móvil.

## Estado de la prueba

✅ Pasó

## Observaciones

- El código si se selecciona el método del celular llega como un mensaje de texto y la aplicación lo percibe una vez que llega, de forma que aparece arriba en el teclado el código sin necesidad de ir a los mensajes de texto.

# Caso de Prueba 3: Recuperación del nombre de usuario

## ID

CT-003

## Objetivo

Verificar que una persona que olvidó su nombre de usuario pueda recuperarlo mediante la validación de su identidad, su tarjeta y el código enviado al teléfono registrado.

## Precondiciones

- Persona usuaria registrada en Banca en Línea.
- Documento de identificación vigente y asociado a la cuenta.
- Tarjeta de crédito o débito activa y asociada a la persona usuaria.
- Acceso al número de teléfono registrado en el banco.
- Conexión estable a Internet.

## Datos de Entrada

- Tipo de identificación: Cédula de identidad.
- Número de identificación: número de cédula válido asociado a la cuenta.
- Número de cédula solicitado para la segunda validación.
- Dígitos solicitados de una tarjeta de crédito o débito válida.
- Nuevo nombre de usuario que cumpla las reglas de seguridad del sistema.
- Confirmación del nombre de usuario.
- Código de verificación válido enviado al teléfono registrado.

## Pasos

1. Acceder a la página de inicio de sesión de Banca en Línea.
2. Seleccionar la opción "Olvidé mi usuario".
3. Seleccionar el tipo de identificación.
4. Digitar el número de identificación.
5. Presionar el botón "Continuar".
6. Ingresar nuevamente el número de cédula solicitado por el sistema.
7. Digitar los números solicitados de la tarjeta de crédito o débito asociada.
8. Presionar el botón "Continuar".
9. Digitar una nuevo nombre de usuario.
10. Digitar nuevamente para confirmarlo.
11. Solicitar o esperar el código de verificación enviado al teléfono registrado.
12. Ingresar el código recibido.
13. Presionar el botón "Continuar".

## Resultado Esperado

- El sistema valida el tipo y el número de identificación.
- El sistema valida la cédula y los dígitos solicitados de la tarjeta.
- El código de verificación se envía únicamente al teléfono registrado.
- El sistema acepta el nuevo nombre cuando cumple las reglas de seguridad y coincide con su confirmación.
- La persona puede utilizar el nuevo usuario y la nueva contraseña para iniciar sesión.
- No se muestran públicamente los datos completos de la tarjeta ni información sensible.

## Resultado Obtenido

- El resultado es el esperado

## Estado de la prueba

✅ Pasó

## Observaciones

- Se debe comprobar que un número de identificación o una tarjeta que no estén asociados a la cuenta no permitan continuar.
- También se debe comprobar el comportamiento cuando el código enviado al celular es incorrecto o ha vencido.

# Caso de Prueba 4: Restablecimiento de contraseña olvidada

## ID

CT-004

## Objetivo

Verificar que una persona que olvidó su contraseña pueda establecer una nueva mediante la validación de su identidad, su tarjeta y el código enviado al teléfono registrado.

## Precondiciones

- Persona usuaria registrada en Banca en Línea.
- Nombre de usuario válido.
- Documento de identificación vigente y asociado a la cuenta.
- Tarjeta de crédito o débito activa y asociada a la persona usuaria.
- Acceso al número de teléfono registrado en el banco.
- Conexión estable a Internet.

## Datos de Entrada

- Nombre de usuario válido.
- Tipo de identificación: Cédula de identidad.
- Número de identificación: número de cédula válido asociado a la cuenta.
- Número de cédula solicitado para la segunda validación.
- Dígitos solicitados de una tarjeta de crédito o débito válida.
- Nueva contraseña que cumpla las reglas de seguridad del sistema.
- Confirmación de la nueva contraseña.
- Código de verificación válido enviado al teléfono registrado.

## Pasos

1. Acceder a la página de inicio de sesión de Banca en Línea.
2. Seleccionar la opción "Olvidé mi contraseña".
3. Ingresar el nombre de usuario, si el sistema lo solicita.
4. Seleccionar el tipo de identificación.
5. Digitar el número de identificación.
6. Presionar el botón "Continuar".
7. Ingresar nuevamente el número de cédula solicitado por el sistema.
8. Digitar los números solicitados de la tarjeta de crédito o débito asociada.
9. Presionar el botón "Continuar".
10. Digitar una nueva contraseña que cumpla las reglas de seguridad.
11. Digitar nuevamente la contraseña para confirmarla.
12. Solicitar o esperar el código de verificación enviado al teléfono registrado.
13. Ingresar el código recibido.
14. Presionar el botón "Continuar".

## Resultado Esperado

- El sistema valida el tipo y el número de identificación.
- El sistema valida la cédula y los dígitos solicitados de la tarjeta.
- La nueva contraseña es aceptada únicamente si cumple las reglas de seguridad y coincide con su confirmación.
- El código de verificación se envía al teléfono registrado y es validado correctamente.
- El sistema confirma que la contraseña fue restablecida.
- La contraseña anterior deja de funcionar.
- La persona usuaria puede iniciar sesión con la nueva contraseña.
- No se muestran públicamente los datos completos de la tarjeta ni información sensible.

## Resultado Obtenido

- El resultado es el esperado.

## Estado de la prueba

✅ Pasó

## Observaciones

- Se debe comprobar el rechazo de contraseñas débiles o que no coincidan.
- También se debe comprobar el comportamiento cuando la identificación, la tarjeta o el código de verificación sean incorrectos.
