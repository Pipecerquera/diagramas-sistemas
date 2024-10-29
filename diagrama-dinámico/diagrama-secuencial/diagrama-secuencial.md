# Diagrama de Secuencia - Agregar Producto y Realizar Compra

Este diagrama de secuencia representa el proceso que ocurre cuando un comprador agrega un producto a su carrito y realiza una compra en el sistema de tienda en línea.
![Diagrama de Secuencia - Carrito de Compras]("C:\Users\USUARIO\diagramas-sistemas\diagrama-dinámico\diagrama-secuencial\diagrama-secuencial.png")


## Descripción del Proceso

1. **Comprador**: Solicita agregar un producto a su carrito a través de la interfaz web.
2. **Interfaz Web**: Recibe la solicitud y la envía al controlador del carrito.
3. **Controlador Carrito**: Verifica con el inventario si hay stock del producto solicitado.
4. **Inventario**: Confirma la disponibilidad del producto.
5. **Carrito**: Agrega el producto al carrito y consulta sus detalles.
6. **Producto**: Proporciona sus detalles para que se agregue al carrito correctamente.
7. **Factura**: Cuando el comprador decide realizar la compra, se genera la factura con los detalles correspondientes.
8. **DetalleFactura**: Registra los detalles específicos de cada producto en la factura.

## Propósito del Diagrama

Este diagrama permite visualizar el flujo de interacción entre el comprador, el carrito de compras, el inventario, y otros componentes necesarios para completar una compra. Es útil para entender cómo el sistema valida el stock, organiza el carrito, y genera un comprobante de compra.

