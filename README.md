# **Proyecto Integrador: ARGBroker Demo**

## **Integrantes:** 

|         Nombre/es     |        Apellido       |      DNI     |            Correo Electrónico           |                   Github                  |
|-----------------------|-----------------------|--------------|-----------------------------------------|-------------------------------------------|
|    Gabriel            |      Gori             |   27955008           |   gabygori@gmail.com                    |https://github.com/Gaby1980                                    |
|    Gaston Exequiel    |      Carreño          |              |   gastonexc@gmail.com                   |                                           |
|    Ariel Orlando      |      Fernandez        |   33817721   |   lic.arielfernandez.hys@gmail.com      |  [https://github.com/fernandez-ariel](https://github.com/fernandez-ariel) |
|    Alvaro Reinaldo    |      Benicio          |   35821816           |   alvarobenicio765@gmail.com                                      |   https://github.com/alvarobenicio                                        |
|    Luis Gerardo       |      Catalas          |   35581397   |   gerardocatalas@mi.unc.edu.ar          |  [https://github.com/geracatalas](https://github.com/geracatalas)|

### **Descripción del proyecto** 

La empresa tecnológica ISPC Cba se ha inscripto como broker de bolsa para ser intermediario entre los inversores y la Bolsa de Valores de Buenos Aires MERVAL.
Es por ello que le ha solicitado la creación de una aplicación para realizar las transacciones entre los inversores (personas físicas, empresas o instituciones) y otros inversores dentro del Mercado de Valores de Buenos Aires (Merval).

### **¿Qué es una acción de una empresa?**

Una acción representa una participación en la propiedad de una empresa, que incluye un
derecho sobre las ganancias y los activos de la empresa. Como tal, los accionistas son
propietarios parciales de la empresa. Cuando el valor de la empresa aumenta o disminuye,
también sube el valor de sus acciones. Además, este valor aumenta o disminuye de
acuerdo a la oferta y demanda. Es una forma que tienen las empresas para poder
capitalizarse y poder crecer.

### **¿Qué es un Broker?**

Un bróker es un intermediario que ejecuta órdenes de compra y venta de activos en los
mercados financieros. Bróker puede denominarse tanto la empresa que ofrece estos
servicios como el corredor de bolsa particular que realiza las operaciones.

### **¿Cuáles son los distintos perfiles de los inversores?**

El perfil del inversionista se refiere a las características de una persona que guían la manera
en que debiera tomar sus decisiones de inversión, incluido su nivel de tolerancia al riesgo,
en relación a los diversos instrumentos de inversión que existen en el mercado. Tiempo de
duración de la inversión. Algunos de ellos pueden ser conservador, medio o agresivos.

### **Diferencia entre renta fija y variable:**

La renta fija y variable se diferencian en la rentabilidad conseguida con la inversión y el
riesgo asumido. La renta fija garantiza una rentabilidad limitada con un riesgo mínimo,
mientras que la renta variable ofrece mayor rentabilidad pero con un riesgo elevado.
Ejemplo de renta fija: plazo fijo tradicional luego de cierto tiempo estipulado se que me va a
dar una compensación por el dinero que deje inmovilizado en un banco con una tasa fijada
o en su defecto una tasa fijada más un monto variable de acuerdo a la inflación (plazo fijo
UVA).
Ejemplo de renta variable: la acción de una empresa es una renta variable porque no se
cuanto puedo ganar o perder al momento de venderla.

### **Requerimientos Funcionales:**

La aplicación, en su primer etapa, contará con una versión demo (simulación de compra y
venta en la bolsa) que tendrá las siguientes funcionalidades:

1- Partir de un saldo inicial de $1.000.000 (que se asigna al momento de crear un nuevo
usuario/inversor).

2- Brindar un panel para consultar las cotizaciones de las acciones de empresas
Argentinas. Dicho panel deberá mostrar los siguientes datos para cada símbolo/título de
acción:
- Símbolo y nombre de la empresa de la acción. Ej.: (ALUA) Aluminio Argentino S.A
- Último Operado
- Cantidad Compra diaria
- Precio de Compra actual
- Precio Venta actual
- Cantidad Venta diaria
- Apertura (precio de la acción al momento de empezar la operación diaria en la bolsa)
- Mínimo diario
- Máximo diario
- Último Cierre.

3- Permitir comprar y vender acciones a precio del mercado (en la imagen, precio
venta y precio de compra). Es decir que en esta etapa no se va a poder poner un precio
inferior o superior al que se está comercializando en este momento. Por lo general se pide
un precio superior para nuestra venta (hay un porcentaje máximo que se puede pedir) y un
precio inferior para nuestras compras intentando comprar al menor precio y vender al mayor
precio.

4- Brindar un panel (Mi Portafolio) que muestre el total invertido, saldo de la cuenta demo, la
cantidad de acciones compradas con su respectivo símbolo/título, el valor comprometido y,
la Ganancia o Pérdida.

5- La aplicación debe estar en español y operar en $ (pesos) con 2 decimales.

6- Calcular la comisión del broker que es de 1.5% por operación de compra o venta.










