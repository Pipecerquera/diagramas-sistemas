# Diagrama de Objetos

![Diagrama de Objetos]("C:\Users\USUARIO\diagramas-sistemas\diagrama-estático\diagrama-objetos\diagrama-objetos.png")

## Descripción
El Diagrama de Objetos representa instancias específicas de clases en el sistema de carrito de compras en un momento dado. Este ejemplo muestra a un `Usuario` específico, `Daniel`, quien realiza una compra de un producto llamado `Laptop`, generando una `Factura` y un `DetalleFactura`.

## ¿Para qué sirve?
Este diagrama es útil para visualizar el estado y las relaciones entre instancias de objetos en un punto particular del tiempo. Esto ayuda a entender cómo interactúan las entidades en el sistema en una situación real, mostrando, por ejemplo, cómo un `Usuario` puede realizar una compra y cómo esta se refleja en los objetos `Factura` y `DetalleFactura`.

## Código
Aquí tienes el código en PlantUML para generar este diagrama:

```plaintext
@startuml
object usuario1 {
    nombre: "Daniel"
    rol: "Comprador"
}

object producto1 {
    nombre: "Laptop"
    precio: "1200.00"
    stock: 5
}

object factura1 {
    id: "F001"
    fecha: "2024-10-30"
    total: "1200.00"
}

object detalleFactura1 {
    cantidad: 1
    subtotal: "1200.00"
}

usuario1 --> detalleFactura1 : "Realiza compra"
detalleFactura1 --> producto1 : "Referencia al producto"
detalleFactura1 --> factura1 : "Pertenece a factura"
@enduml
