# Diagrama de Tiempo - Sistema de Carrito de Compras

![Diagrama de Tiempo]("C:\Users\USUARIO\diagramas-sistemas\diagrama-dinámico\diagrama-tiempo\diagrama-tiempo.png")

## Descripción
Este diagrama de tiempo, en formato de secuencia, representa cómo cambian los estados de los principales objetos en un sistema de carrito de compras a medida que el usuario interactúa con el sistema y progresa en el flujo de compra. Este enfoque secuencial nos permite visualizar los momentos clave en los que el sistema actualiza los estados de cada objeto durante el proceso de compra.

### Cambios de Estado
1. **Producto**:
   - **Disponible**: El estado inicial del producto, indicando que está listo para ser agregado al carrito.
   - **Reducir Stock**: Cuando el comprador agrega el producto al carrito, el stock del producto se reduce para reflejar la cantidad disponible restante.

2. **Carrito**:
   - **Vacío**: Estado inicial del carrito, indicando que no tiene productos agregados.
   - **Producto Añadido**: Cuando el comprador selecciona un producto, el estado del carrito cambia para reflejar que contiene productos.

3. **Pedido**:
   - **Sin Pedido**: Estado inicial antes de que el comprador confirme la compra.
   - **Pedido Creado**: Al finalizar la compra, se crea el pedido y el estado refleja que el pedido está listo para ser procesado.

## Propósito del Diagrama
Este diagrama es útil para comprender el ciclo de vida de los objetos `Producto`, `Carrito` y `Pedido` a medida que cambian de estado en el sistema. Estos cambios de estado permiten ver cómo el sistema refleja las acciones del usuario y aseguran que cada objeto tenga el estado correcto en cada paso del proceso de compra.

## Beneficios
El diagrama facilita la comprensión de cómo los objetos principales en el sistema se actualizan durante el flujo de compra. Este enfoque ayuda a los desarrolladores a identificar cuándo y dónde ocurren las transiciones de estado, promoviendo una mejor gestión y seguimiento del ciclo de vida de los objetos.
