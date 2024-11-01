# Diagrama de Estados

![Diagrama de Estados]("C:\Users\USUARIO\diagramas-sistemas\diagrama-dinámico\diagrama-estados\diagrama-estados.png")

El Diagrama de Estados muestra los diferentes estados posibles en los que puede encontrarse el carrito de compras y cómo cambia de un estado a otro en respuesta a las acciones del usuario. Este diagrama es fundamental para comprender el ciclo de vida del carrito y cómo el sistema maneja las distintas etapas de una compra.

## Descripción de los Estados y Transiciones

1. **Vacío**: Este es el estado inicial del carrito cuando no contiene ningún producto. Al iniciar sesión o comenzar una sesión de compra, el carrito está vacío y espera que el usuario agregue productos.

2. **Con Productos**: Cuando el usuario agrega al menos un producto al carrito, cambia al estado "Con Productos". En este estado, el usuario puede continuar agregando más artículos, revisar los que ya están, o eliminar aquellos que no desea comprar.

3. **Pago en Proceso**: Cuando el usuario decide proceder al pago, el carrito entra en el estado "Pago en Proceso". En este estado, el sistema verifica la disponibilidad de los productos y prepara la información necesaria para la transacción de pago.

4. **Compra Realizada**: Si el proceso de pago se completa correctamente, el carrito pasa al estado final de "Compra Realizada". En este estado, el sistema confirma la transacción y vacía el carrito, listo para un nuevo ciclo de compra.

## Flujo de Estados

- **Vacío → Con Productos**: Esta transición ocurre cuando el usuario agrega el primer producto al carrito.
- **Con Productos → Vacío**: Si el usuario decide eliminar todos los productos del carrito, este vuelve al estado "Vacío".
- **Con Productos → Pago en Proceso**: Cuando el usuario decide realizar el pago, el carrito pasa al estado "Pago en Proceso".
- **Pago en Proceso → Compra Realizada**: Tras completar exitosamente el pago, el carrito pasa al estado "Compra Realizada" y el sistema genera la confirmación de compra.

Este diagrama ayuda a entender el comportamiento del carrito en función de las acciones del usuario y los cambios de estado que resultan de las interacciones en el sistema. Identifica claramente cada transición y los eventos que llevan a esos cambios, lo que permite anticipar posibles problemas o excepciones en el flujo de compra.
