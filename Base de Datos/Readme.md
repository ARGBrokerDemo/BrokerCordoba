## Identificación de Entidades

- Usuarios: Tabla que registra los usuarios de la aplicación y sus datos personales.
- Cuenta Bancaria: Tabla que registras los datos de las cuentas bancarias pertenecientes a los usuarios.
 - Portafolio: Tabla que registra la tenencia de acciones por parte de los usuarios. 
 - Precio merado: Tabla que registra los precios de las acciones en el MERVAL en determinado momento.
- Transacciones: Tabla que registras las operaciones de compra y venta de acciones por parte de los usuarios.
- Acciones: Tabla que registra los datos de las acciones y sus precios
- Empresas: Tabla que registra los datos de las empresas que cotizan en bolsa.


## Descripción tablas:
###### Usuarios

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

###### cuenta bancaria

| Nombre Atributo | Tipo |Explicación|
| ------ |------|------|
| cuentabancaria | |identificador de registro de la cuenta|
| cbu_cvu |PK |clave bancaria única de la cuenta|
| banco |  |nombre del banco al que pertenece la cuenta|
| titular |  |titular de la cuenta|
| cuit | FK |cuit del titular de la cuenta - Clave foránea con usuarios |

###### precio mercado

| Nombre Atributo | Tipo |Explicación|
| ------ |------|------|
| idAccion | PK |identificador de acción clave primaria compuesta|
| fechaHora |PK |fecha y hora del precio de la acción clave primaria compuesta|
| precioCompra |  |precio de compra del mercado|
| precioVenta|  |precio de venta del mercado|

###### transacción

| Nombre Atributo | Tipo |Explicación|
| ------ |------|------|
| idTransaccion | PK |identificador de la trasacción realizada|
| cuit |FK |cuit del usuario que realiza la transacción - clave foránea  |
| idAccion | FK |identificador de la acción - clave foránea |
| tipoTransaccion|  |precio de venta del mercado|
| cantidad ||cantidad de acciones compradas en la operación|
|precio ||valor de compra o venta de la operación|
| fechaOperacion ||fecha y hora en la que se registra la operación en el sistema|
| comision ||monto de comisión sobre la venta|
