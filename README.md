# Orbita-Galactica-Base-de-Datos

prompt:
Generame un caso de estudio de una cafeteria(orbita galactica ) ,que permita usarla como contexto para realizar un modelo entidad relacion.

☕ Caso de estudio: Cafetería “Órbita Galáctica”

La cafetería **Órbita Galáctica** vende diferentes tipos de bebidas y alimentos, como cafés, jugos, postres y sándwiches.
Para mejorar la organización del negocio, la cafetería desea crear una base de datos que permita registrar la información de sus **clientes, empleados, productos y pedidos**.
Cuando un cliente realiza una compra, un empleado registra el pedido en el sistema. Cada pedido puede incluir uno o varios productos. De cada producto se registra su nombre, precio y categoría.
La cafetería también desea guardar información básica de sus clientes, como su nombre, teléfono y correo electrónico.
Cada empleado puede registrar varios pedidos, pero cada pedido es registrado por un solo empleado.

## 📌 Entidades principales

### 👤 Cliente

* ID_Cliente
* Nombre
* Teléfono
* Correo

### 👨‍💼 Empleado

* ID_Empleado
* Nombre
* Cargo

### 🧾 Pedido

* ID_Pedido
* Fecha
* Total
* ID_Cliente
* ID_Empleado

### ☕ Producto

* ID_Producto
* Nombre
* Precio
* Categoría

### 📋 Detalle_Pedido

* ID_Detalle
* ID_Pedido
* ID_Producto
* Cantidad



## 🔗 Relaciones

* Un **cliente** puede realizar muchos **pedidos**.
* Cada **pedido** pertenece a un solo **cliente**.
* Un **empleado** puede registrar muchos **pedidos**.
* Cada **pedido** es registrado por un solo **empleado**.
* Un **pedido** puede contener varios **productos**.
* Un **producto** puede aparecer en muchos **pedidos**.
* La entidad **Detalle_Pedido** permite relacionar los pedidos con los productos.


