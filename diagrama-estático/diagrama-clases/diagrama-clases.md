## Diagrama UML

A continuación se presenta el diagrama UML generado a partir del código WSD anterior, mostrando las clases, sus atributos y métodos, y las relaciones entre ellas.

![Diagrama UML - Carrito de Compras]("C:\Users\USUARIO\diagramas-sistemas\diagrama-estático\diagrama-clases\img\diagrama-clases.png")
Uml

---

## Explicación

1. **Usuario**: Clase base que representa a cualquier usuario del sistema. Incluye métodos básicos como `registrarse()` e `iniciarSesion()`. Esta clase tiene los atributos:
   - `id`: Identificador único de tipo `int`.
   - `nombre`: Nombre del usuario, de tipo `String`.
   - `correo`: Correo electrónico, de tipo `String`.

2. **Administrador**: Subclase de `Usuario`, representa a los administradores del sistema. Su método principal es:
   - `gestionarInventario()`: Permite gestionar los productos en el inventario.

3. **Comprador**: Subclase de `Usuario`, representa a los clientes del sistema. Incluye métodos para:
   - `agregarProductoCarrito()`: Añade productos al carrito de compras.
   - `realizarCompra()`: Inicia el proceso de compra.

4. **Producto**: Representa los productos de la tienda. Incluye atributos como:
   - `id`: Identificador único.
   - `nombre`: Nombre del producto.
   - `descripcion`: Detalles del producto.
   - `precio`: Precio unitario.
   - `stock`: Cantidad disponible.
   - Método `actualizarStock(cantidad)`: Actualiza el stock del producto.

5. **Inventario**: Gestiona la lista de `Producto`. Tiene el método:
   - `verificarStock(productoId)`: Comprueba si hay stock disponible para un producto específico.

6. **Carrito**: Clase que representa el carrito de compras del `Comprador`, con métodos como:
   - `agregarProducto(producto)`: Añade un producto al carrito.
   - `eliminarProducto(productoId)`: Elimina un producto específico del carrito.
   - `calcularTotal()`: Calcula el precio total de los productos en el carrito.

7. **Factura**: Clase para generar un comprobante de compra. Incluye:
   - `id`: Identificador único de la factura.
   - `fecha`: Fecha de la compra.
   - `total`: Monto total de la compra.
   - `generarFactura()`: Genera el comprobante de la compra.

8. **DetalleFactura**: Detalla los productos comprados en la factura. Incluye:
   - `producto`: Producto comprado.
   - `cantidad`: Cantidad adquirida.
   - `precioTotal`: Precio total de ese producto en la factura.

---
