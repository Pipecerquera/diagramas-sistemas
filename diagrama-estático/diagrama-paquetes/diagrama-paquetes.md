# Diagrama de Paquetes - Sistema de Carrito de Compras

![Diagrama de Paquetes]("C:\Users\USUARIO\diagramas-sistemas\diagrama-estático\diagrama-paquetes\diagrama-paquetes.png")

## Descripción
El diagrama de paquetes organiza el sistema en módulos lógicos para mejorar la comprensión y modularidad de la arquitectura. Esto es particularmente útil en un sistema de carrito de compras, donde existen múltiples funcionalidades específicas que deben agruparse de manera lógica y modular para facilitar el desarrollo y mantenimiento.

### Componentes del Diagrama
1. **Usuario**: Este paquete agrupa todas las clases relacionadas con los diferentes tipos de usuarios. Contiene:
   - **Usuario**: Clase base para cualquier usuario del sistema.
   - **Administrador**: Subclase de Usuario, encargada de funciones como la gestión del inventario.
   - **Comprador**: Subclase de Usuario, representando al cliente que puede agregar productos al carrito y realizar compras.

2. **Producto**: Este paquete se centra en la gestión de productos y su disponibilidad:
   - **Producto**: Clase que representa un producto específico con atributos como nombre, descripción y precio.
   - **Inventario**: Clase que permite verificar el stock de cada producto.

3. **Carrito**: Agrupa funcionalidades relacionadas con el carrito de compras.
   - **Carrito**: Clase que permite agregar, eliminar productos y calcular el total de una compra.

4. **Compra**: Incluye las clases relacionadas con el proceso de compra.
   - **Factura**: Clase para generar comprobantes de compra.
   - **DetalleFactura**: Clase para detallar cada producto en la factura.

## Propósito del Diagrama
Este diagrama es crucial para establecer una organización lógica en el sistema de carrito de compras. Agrupar clases en paquetes facilita la modularidad del código y simplifica la identificación de funcionalidades, especialmente en proyectos grandes o con múltiples desarrolladores.

## Beneficios
Al observar las agrupaciones, los desarrolladores pueden identificar rápidamente las clases relevantes dentro de un módulo específico (como gestión de productos o compras) y trabajar de manera más organizada.

