## Identificación de Entidades

- Usuarios: Tabla que registra los usuarios de la aplicación y sus datos personales.
- Cuenta Bancaria: Tabla que registras los datos de las cuentas bancarias pertenecientes a los usuarios.
 - Portafolio: Tabla que registra la tenencia de acciones por parte de los usuarios. 
 - Precio merado: Tabla que registra los precios de las acciones en el MERVAL en determinado momento.
- Transacciones: Tabla que registras las operaciones de compra y venta de acciones por parte de los usuarios.
- Acciones: Tabla que registra los datos de las acciones y sus precios
- Empresas: Tabla que registra los datos de las empresas que cotizan en bolsa.


## Descripción tablas:
Usuarios

| Nombre Atributo | Tipo |Explicación|
| ------ |------|------|
| idUsuario | |identificador único del usuario|
| nombreRazonsocial | |nombre o razon social del usuario|
| cuit | PK |identificador único tabla|
| domicilio |  |domicilio del usuario|
| celular |  |numero de teléfono del usuario|
| email |  |dirección de correo electrónico del usuario|
| perfil|  |pefil inversor usuario|
| contraseña |  |Contraseña del usuario|
| fecha alta |  |fecha el alta en el sistema del usuario|
