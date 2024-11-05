# Diagrama de Perfil - Sistema de Carrito de Compras

![Diagrama de Perfil]("C:\Users\USUARIO\diagramas-sistemas\diagrama-estático\diagrama-perfil\diagrama-perfil.png")

## Descripción
El diagrama de perfil define las clases personalizadas del sistema de carrito de compras mediante el uso de estereotipos, los cuales ayudan a diferenciar las responsabilidades y tipos de elementos dentro del sistema. Este diagrama extiende la semántica de UML y adapta los elementos para representar mejor el contexto del sistema de compras.

### Componentes y Estereotipos
- **Actor (`<<actor>>`)**:
  - **Usuario**: Representa a los actores que interactúan con el sistema (Administrador o Comprador).

- **Role (`<<role>>`)**:
  - **Administrador**: Usuario responsable de gestionar productos y stock en el sistema.
  - **Comprador**: Usuario que representa al cliente y utiliza el sistema para realizar compras.

- **Entity (`<<entity>>`)**:
  - **Producto**: Elemento clave en el sistema de compras, con detalles como precio y stock.
  - **Inventario**: Representa la disponibilidad de productos y sus niveles de stock.
  - **Carrito**: El contenedor de productos que selecciona el Comprador.

- **Document (`<<document>>`)**:
  - **Factura**: Documento que refleja la compra realizada por el Comprador.
  - **DetalleFactura**: Documento con el desglose de productos, cantidades y precios en la compra.

## Propósito del Diagrama
Este diagrama es útil para personalizar y detallar las diferentes partes del sistema, distinguiendo claramente entre roles, actores, entidades y documentos. Esto mejora la comprensión de los elementos que interactúan en el sistema y ayuda a mantener un código más claro y organizado.

## Beneficios
Al visualizar los estereotipos, el equipo de desarrollo y los stakeholders pueden comprender de inmediato los roles y tipos de elementos dentro del sistema. Esto facilita la asignación de responsabilidades y promueve un desarrollo modular.
