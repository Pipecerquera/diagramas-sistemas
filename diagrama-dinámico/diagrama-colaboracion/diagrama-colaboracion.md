# Diagrama de Colaboración

![Diagrama de Colaboración]("C:\Users\USUARIO\diagramas-sistemas\diagrama-dinámico\diagrama-colaboracion\diagrama-colaboracion.png")

## Descripción
El Diagrama de Colaboración muestra las interacciones entre objetos en el proceso de compra de un producto en el sistema de carrito de compras. Los objetos `Usuario`, `Carrito`, `Producto`, `Factura`, y `DetalleFactura` interactúan para realizar la transacción.

## ¿Para qué sirve?
Este diagrama es esencial para comprender cómo fluyen los mensajes y colaboran los objetos en el sistema durante un proceso específico, en este caso, la compra de un producto. Ayuda a visualizar la secuencia de acciones y la colaboración entre componentes en el sistema para completar una tarea.

## Código
Aquí tienes el código en PlantUML para generar este diagrama:

```plaintext
@startuml
actor Usuario as usuario
participant "Carrito" as carrito
participant "Producto" as producto
participant "Factura" as factura
participant "DetalleFactura" as detalleFactura

usuario -> carrito : "Agregar producto"
carrito -> producto : "Verificar disponibilidad"
carrito -> detalleFactura : "Generar detalle"
carrito -> factura : "Crear factura"
factura -> detalleFactura : "Añadir detalles de compra"
@enduml
