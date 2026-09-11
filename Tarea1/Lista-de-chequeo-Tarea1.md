# Lista de Chequeo para Tarea # 1

## 1. Accesibilidad Inicial y Carga

- [x] El sitio carga correctamente (sin errores de carga o fallos visibles).
- [x] El contenido principal aparece rápidamente (menos de 5 segundos).
- [x] No hay errores evidentes (mensajes técnicos, 404, pantallas en blanco).
- [x] El sitio es _responsivo_ (se adapta a pantallas móviles/tablets).

## 2. Navegación General

- [x] El menú principal es visible y funcional.
- [x] Los enlaces llevan a las páginas correctas.
- [x] El botón "Inicio" o logo lleva a la página principal.
- [x] Hay forma de volver atrás fácilmente o de reiniciar una acción.
    En el ultimo aspecto, depende de en qué parte de la página estemos,
    en la página principal antes de entrar a Banca en Línea sí, pero al ingresar a
    crear una cuenta o en banca en línea hay algunos casos que es díficil volver atrás o se queda pegada la página

## 3. Flujos Críticos

Después del item se puso una explicación de lo que se encontró en caso de no cumplir con la expectativa.

- [x] Abrir cuenta (campos obligatorios, validación, éxito).
Al intentar abrir una nueva cuenta, pide ingresar fotos de la cédula en donde permite varios formatos como pdf, jpg y png, pero al intentar adjuntar un pdf no lo acepta, entonces no es éxitosa la creación de una cuenta si no se tiene en formato de fotos la cédula. No tuve éxito y por eso no estoy marcando la casilla.
- [x] Inicio de sesión / recuperación de contraseña.
- [x] Cierre de sesión correcto.
- [x] Creación o envío de datos (formularios, publicaciones, etc.).
- [x] Edición de datos existentes (perfil, configuraciones).
- [x] Proceso de pago / transferencias / cobros.
Funciona bien.

## 4. Formularios y Validaciones

- [x] Los campos requeridos están claramente marcados.
- [x] El sistema valida entradas incorrectas (email inválido, números, etc.).
El sistema si valida los números al hacer una transferencia por ejemplo. Se probó también intentando con SINPE movil y el sistema solo acepta 8 dígitos para celular, si se intentan escribir más no lo permite.
- [x] Mensajes de error son comprensibles y útiles.
Diría que en la mayoría de los casos sí, al menos en las pruebas que hice esta vez, entonces por eso lo marco. Pero creo que en veces anteriores han habido mensajes que no he entendido.
- [x] Se pueden corregir errores sin reiniciar todo el formulario.
- [x] Los mensajes de éxito aparecen correctamente.

## 5. Contenido y Usabilidad

- [x] Textos sin errores ortográficos o gramaticales.
- [x] Botones y enlaces tienen nombres claros y consistentes ("Guardar", "Cancelar", etc.).
- [x] Las acciones del usuario tienen retroalimentación (mensajes, animaciones tipo _loaders_).
Casi ninguno tiene mensajes o animaciones, solo se ve que la página se refresca desde la pestaña.
- [x] No se requieren pasos innecesarios o confusos.
En algunos caso sí siento que hay pasos innecesarios como la creación de una cuenta favorita para poder hacer cualquier transferencia o que generan cierta confusión.
- [x] El sistema es intuitivo sin necesidad de instrucciones externas.
Diría que a grandes rasgos sí, pero aún requiere muchos detalles para que sea más usable, el tamaño de las letras y la forma de mostrar cierta información podría mejorarse. Algunas imágenes dentro de procesos como transferencias no tienen mucho sentido, sería mejor mejorar los botones de la par y poner una mejor letra.

## 6. Compatibilidad Básica

- [x] Probar en al menos dos navegadores (Chrome, Firefox, Edge, Safari).
- [x] Probar en dispositivo móvil vs escritorio (modo responsivo o dispositivo real).
- [x] Probar en resolución más baja (ej. 1024x768) y más alta.

## 7. Manejo de Errores y Casos Límite

- [x] ¿Qué ocurre si el usuario deja todo un formulario vacío?
Si se deja todo vacío sale un mensaje diciendo selecciona la cuenta a acreditar para hacer la transferencia, el texto sale a un lado y en color rojo.
- [x] ¿Qué pasa si introduce datos absurdos (nombre de 1000 caracteres, símbolos raros)?
Al intentar poner símbolos raros en un monto de una transferencia no se digitan ni sale ningún pop up diciendo porqué no, sin embargo en el concepto de la transferencia sí sale una ventana que dice que no se aceptan caracteres especiales.
- [x] ¿Qué ocurre si se recarga la página durante una acción?
En el caso de estar haciendo una transferencia, si refresco la página se mantiene en la misma parte, pero se borran los datos del formulario, desde el monto puesto hasta la cuenta a la cual tengo que hacer la transferencia.
- [x] ¿Cómo responde el sistema si se pierde la conexión a Internet?
Al ratito la página se "cae", se pone en blanco con el dinosaurio para jugar por no haber conexión a internet. Y al volver a tener internet, se debe volver a iniciar sesión.

## 8. Seguridad básica visible (sin análisis técnico)

- [x] Las contraseñas no se ven mientras se escriben (excepto si tienen un recurso para poder verlas, e.g. el "ojito").
- [x] No se puede navegar hacia páginas privadas sin haber iniciado sesión.
- [x] El usuario no puede ver información de otros usuarios.
- [x] Después de cerrar sesión, no puedes volver con el botón "atrás".

## 9. Feedback y Soporte

- [x] Los mensajes de ayuda, tooltips o instrucciones están presentes (si aplica).
En algunos casos sí, pero en otras secciones no hay instrucciones si fuera necesario.
- [x] Hay términos y condiciones / políticas de privacidad visibles (si aplica).

## 10. Aspecto General y Estabilidad

- [x] Diseño consistente entre secciones.
La mayoría parecen tener el mismo tipo de letra, y se tiene un diseño consistente en la mayoría, pero hay unas páginas que tienen una imagen grande que no tiene relevancia o no aporta utilidad, al seleccionar transferencias por ejemplo.
- [x] Imágenes y elementos visuales se cargan correctamente.
- [x] El sitio no se desajusta al hacer zoom (Ctrl + o -).
No se desajusta
- [x] No hay "pantallas muertas" sin contenido o acción clara.
