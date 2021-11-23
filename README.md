# eCommerceRopa-Parcial2

GRUPO 1.

- GOZALVEZ, Franco
- MORENO, Lucas Exequiel
- PIRIZ, Carla

 // SENTENCIAS GENERATE MODELO // 

npx sequelize model:generate --name Domicilio --attributes calle:string,numero:string,codigo_postal:string,localidad:string,provincia:string

npx sequelize model:generate --name Puntodeventa --attributes domicilio:string,cuit:string,ingresos_brutos:string

npx sequelize model:generate --name Marca --attributes nombre:string

npx sequelize model:generate --name Categoria --attributes nombre:string

npx sequelize model:generate --name Usuario --attributes name:string,dni:string,email:string,contraseña:string,usuario:string,domicilioId:integer

npx sequelize model:generate --name Factura --attributes fecha:string,tipo:string,total:string,usuarioId:integer,puntodeventaId:integer

npx sequelize model:generate --name Detallefactura --attributes cantidad:integer,subtotal:string,total:string,facturaId:integer

npx sequelize model:generate --name Producto --attributes stock:string,desc:string,precio:string,nombre:string,prodimg:string,categoriaId:integer,marcaid:integer,detallefacturaId:integer

npx sequelize model:generate --name Talle --attributes tipo:string,medidas:string,productoId:integer,producto_categoriaid:integer
