# Investigacion
Variables estáticas
Prefico “static” se utiliza para la declaración de la variable.
Las variables estáticas en C poseen las siguientes propiedades:
1. No pueden ser accedidas desde otro fichero. Por tanto, los prefijos “extern” y “static” no pueden ser utilizados en la misma declaración.
2. Mantienen su valor a lo largo de toda la ejecución del programa independientemente del ámbito en el que estén definida.
Dichas propiedades derivan los siguientes casos:
•	Si una variable estática está declarada fuera de las funciones, será accesible únicamente por el código que le siga en el mismo fichero de su declaración. 
•	Si una variable estática está declarada en una función, sólo será accesible desde esa función y mantendrá su valor entre ejecuciones de la función. Este comportamiento es contra intuitivo porque estas variables se declaran en el mismo lugar que el resto de variables en una función, pero mientras que estas adquieren valores nuevos con cada ejecución, las estáticas conservan estos valores entre ejecuciones.

Ciclo de vida de las variables
El ciclo de vida de las variables es el tiempo de vida que se refiere al tiempo en el que transcurre desde que existe la variable hasta cuando se destruye.

Memoria dinámica en lengua C
Es la memoria que no puede ser definida, porque no se conoce o se tiene definid el número de variables a considerarse, la forma de solucionar esto en la memoria dinámica, ya que permite solicitar en tiempo de ejecución más memora al sistema operativo. El sistema operativo permite esto gracias al uso de punteros, por la misma naturaleza del proceso nos impide conocer el tamaño de la memoria necesaria en el momento de compilar.

Orientado a objetos

Clase
Las clases son los modelos sobre los cuáles se construirán nuestros objetos. Permiten abstraer los datos y sus operaciones asociadas al modo de una caja negra.

Objeto
Unidad dentro de un programa de computadora que consta de un estado y de un comportamiento. Cada objeto es capaz de recibir mensajes, procesar datos y enviar mensajes a otros objetos de manera similar a un servicio. Un objeto es el resultado de la instanciación de una clase

Instanciación

La instanciación de un programa es una copia de una versión ejecutable del programa que ha sido escrito en la memoria de la computadora. Se creada típicamente por el usuario.


Herencia
Es la transmisión del código entre unas clases y otras. Para soportar un mecanismo de herencia tenemos dos clases: la clase padre y la/s clase/s hija/s. La clase padre es la que transmite su código a las clases hijas. En muchos lenguajes de programación se declara la herencia con la palabra "extends".
class Hija extends Padre{ }
Eso quiere decir que todo el código de la clase padre se transmite, tal cual, a la clase hija. Si lo quieres ver así, es como si tuvieras escrito, línea a línea, todo el código de la class "Padre" dentro de las llaves de la class "Hija". Por eso, la herencia es fundamental para reutilizar código, porque no necesitas volver a incorporar el código de Padre en Hija, sino que realmente al hacer el "extends" es como si ya estuviera ahí.

Sobrecarga
Capacidad de un lenguaje de programación, que permite nombrar con el mismo identificador diferentes variables u operaciones.; además es la posibilidad de tener dos o más funciones con el mismo nombre pero funcionalidad diferente. En otras palabras, dos o más funciones con el mismo nombre realizan acciones diferentes. El compilador usará una u otra dependiendo de los parámetros usados. A esto se llama también sobrecarga de funciones.
Java no permite al programador implementar sus propios operadores sobrecargados, pero sí utilizar los predefinidos como el +. C++, por el contrario si permite hacerlo.

En sobrecimiento (Shadowing)
Es el hecho de que en una clase una variable miembro y una variable local definida en un método miembro, se llamen igual. Básicamente, dado un objeto, no se llama la definición dada por su tipo intrínseco, sino por el aparente. En otras palabras, no hay polimorfismo.

Ciclo de vida; (ruby)

•	Variables de clase 
Son creadas en el momento se crea el objeto que las contiene, son inicializadas por defecto si no se hace de modo explícito; con 0 para números, "false" para booleano, "null" para objetos y son destruidas cuando termina el probrama.

•	Variables de método 
Son creadas cuando la clase se usa por primera vez, se inicializan por defecto si no se hace de modo explícito, con 0 para números, "false" para booleano y "null" para objetos; y suelen existir para el resto del programa (salvo que no esté cargado). 
•	Variables estáticas
Son creadas en la sentencia en la que están definidas, no se inicializan por defecto, contienen datos imprevisibles y se destruyen al salir del bloque.
