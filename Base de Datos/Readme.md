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

| Nombre Atributo | Tipo |Descripción|
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

| Nombre Atributo | Tipo |Descripción|
| ------ |------|------|
| cuentabancaria | |identificador de registro de la cuenta|
| cbu_cvu |PK |clave bancaria única de la cuenta|
| banco |  |nombre del banco al que pertenece la cuenta|
| titular |  |titular de la cuenta|
| cuit | FK |cuit del titular de la cuenta - Clave foránea con usuarios |

###### precio mercado

| Nombre Atributo | Tipo |Descripción|
| ------ |------|------|
| idAccion | PK |identificador de acción clave primaria compuesta|
| fechaHora |PK |fecha y hora del precio de la acción clave primaria compuesta|
| precioCompra |  |precio de compra del mercado|
| precioVenta|  |precio de venta del mercado|

###### transacción

| Nombre Atributo | Tipo |Descripción|
| ------ |------|------|
| idTransaccion | PK |identificador de la trasacción realizada|
| cuit |FK |cuit del usuario que realiza la transacción - clave foránea  |
| idAccion | FK |identificador de la acción - clave foránea |
| tipoTransaccion|  |precio de venta del mercado|
| cantidad ||cantidad de acciones compradas en la operación|
|precio ||valor de compra o venta de la operación|
| fechaOperacion ||fecha y hora en la que se registra la operación en el sistema|
| comision ||monto de comisión sobre la venta|

###### acción

| Nombre Atributo | Tipo |Descripción|
| ------ |------|------|
| idAccion | PK |identificador del la acción en el sistema|
| simbolo||símbolo de la acción en el mercado |
| idEmpresa| FK |indentificador de la empresa - Clave foránea|
| ultimoOperado ||muestra el último precio operado|
|cantidadComprada||muestra la cantidad de acciones compradas en el día|
| precioCompra ||muestra el precio de compra en el MERVAL |
| precioVenta ||muestra el precio de venta en el MERVAL|
| cantidadVendida||muestra la cantidad de acciones vendidas en el día|
| precioApertura ||muestra el precio de apertura del día|
| precioMinimo ||muestra el precio más bajo operado|
| precioMaximo ||muestra el precio más alto operado|
| ultimoCierre ||muestra el precio al cierre de la jornada|
| montoOperado ||muestra la suma total de las transacciones realizadas|

###### empresa

| Nombre Atributo | Tipo |Descripción|
| ------ |------|------|
| idEmpresa | PK |identificador del la empresa en el sistema|
| nombre||razón social de la empresa |
| sector||sector al cual pertenece la empresa|


## Relaciones
- Usuarios – cuenta bancarias (1:N) : Un usuario puede tener varias cuentas bancarias para ingresar dinero y realizar la compra, cada cuenta bancaria pertenece a un solo usuario.
- Usuarios-portafolio (1:1): Un usuario tiene un solo portafolio y cada portafolio pertenece a un solo usuario.
- Usuario-Transacciones (1:N): Un usuario realiza varias transacciones y cada transacción es realizada por solo un usuario.
- Precio Mercado-Transacciones (1:N): cada transacción se registra de acuerdo al precio de la acción en el momento y varias transacciones pueden registrarse con el precio de una acción en un momento determinado.
- Portafolio-Transacciones (1:N): Un portafolio puede estar compuesto por varias transacciones y cada transacción se corresponde a un solo portafolio.
- Acciones-Transacciones (1:N): Cada transacción se corresponde a una única acción especifica y una acción puede registrarse en varias transacciones.	
- Acciones-Empresas (1:N): Una acción pertenece a una sola empresa y una empresa puede emitir varias acciones.

