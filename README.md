## Proyecto: Base de Datos NoSQL para Tienda Online (MongoDB)

Este proyecto implementa una base de datos NoSQL en MongoDB para una Tienda Online, permitiendo gestionar clientes, productos y pedidos.
El sistema simula el funcionamiento básico de un comercio electrónico, donde los clientes realizan compras, los productos mantienen inventario y los pedidos registran el detalle de la transacción.
```
Estructura del Proyecto
TiendaOnline-MongoDB/
── README.md                 → Descripción general del proyecto
── queries/
 01_insert_clients.mongo        → Inserción de clientes
 02_insert_products.mongo       → Inserción de productos
 03_insert_orders.mongo         → Inserción de pedidos
 10_basic_queries.mongo         → Consultas básicas CRUD
 20_filters_operators.mongo     → Consultas con filtros y operadores
 30_aggregations.mongo          → Consultas de agregación
```
## Estructura de la Base de Datos: TiendaOnline
```
La base de datos contiene tres colecciones principales:
```
## clientes
Guarda la información de cada cliente registrado, incluyendo:
```
nombre
correo
teléfono
dirección (subdocumento)
fecha de registro
estado activo
```
## productos
Contiene el inventario disponible en la tienda:
```
nombre
categoría
precio
stock
disponibilidad
```
## pedidos
Registra las compras realizadas por los clientes:
```
cliente_id
fecha del pedido
productos (arreglo)
total del pedido
estado del pedido
```

## Ejecución del Proyecto

## Para ejecutar los scripts de este proyecto:

1️ Abre tu MongoDB Shell (mongosh) conectado a Atlas
```
mongosh "mongodb+srv://USUARIO:CLAVE@cluster0.aqemnnm.mongodb.net/TiendaOnline"
```
2 Ejecuta las inserciones
```
mongosh --file queries/01_insert_clients.mongo
mongosh --file queries/02_insert_products.mongo
mongosh --file queries/03_insert_orders.mongo
```
3 Realizas las consultas 
```
10_basic_queries.mongo         → Consultas básicas CRUD
 20_filters_operators.mongo     → Consultas con filtros y operadores
 30_aggregations.mongo          → Consultas de agregación
```


 20_filters_operators.mongo     → Consultas con filtros y operadores
 30_aggregations.mongo          → Consultas de agregación
