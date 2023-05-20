# > Codigo Limpio

En la década de 1980 comercializó una gran aplicación de software que fue  muy vendida, pero poco a poco las actualizaciones fueron distanciando y la gente dejando  de  usar  el  producto,  ¿por  qué?  La  razón  que  dió  uno  de  los  empleados,  fue  que  comercializaron el software antes de tiempo con fallos en el código, poco después la  empresa desapareció y fue a raíz del mal código, de ahí la importancia del buen código

## Nombres con Sentido

Los  nombres  estan  en  todas  partes,  clases,  variables,  ficheros,  etc.  Elegir  nombres relevantes es de suma importancia, y aunque pareciera algo de sentido común, ni es tan común ni es tan sencillo.  

	Cada vez que encuentre un nombre de alguna variable que se puede mejorar, CAMBIALA!, la  gente que lea su código se lo 
	agradecerá. Los nombres deben revelar nuestras intenciones.

## Funciones

Una función es una sección de un programa que calcula un valor de manera independiente al resto del programa.

	El tamaño de nuestra funcion debe ser reducido para facilitar su comprension.

El objetivo es que el código se pueda leer de arriba hacia abajo, es lo que se denomina la  regla descendente. Que en cada función que vamos bajando se baje en 1 el nivel de  abstracción,  así  solo  quedaría  un  solo  nivel de abstracción en cada función, es algo  complicado de entender, pero es la clave para escribir pequeñas funciones.

El número de argumentos ideal para  una función es cero, luego uno y después dos. Siempre que sea posible hay que evitar la  presencia de tres argumentos. La diferencia entre un método con argumentos y otro que no,  es que cada vez que veamos dicho método tendremos que interpretar el argumento que se  encuentra en otro nivel de abstracción, con 1 es sencillo pero con 2 y con 3 la cosa se  vuelve compleja.

No  es  recomendable  que  las  funciones  tengan  efectos  secundarios,

Las funciones deben hacer algo, o devolver algo, pero no ambas cosas, sería confuso.

## Comentarios

Un comentario bueno puede resultar muy útil, un comentario antiguo y que diga mentiras es  un error, los comentarios se suelen usar cuando somos incapaces de expresarnos en el  código, pero lo ideal es dedicar tiempo a podernos expresar correctamente en el código,  porque un comentario antiguo que no haya sido actualizado puede crear confusión, debido  a que el código probablemente se haya modificado con el tiempo.

	Aunque los comentarios  sean necesarios en ocasiones, debemos dedicar nuestra energía a minimizarlos.

Una de las razones por las que se escriben comentarios es el código incorrecto, creamos  una función o una clase, vemos que es un poco confuso y lo comentamos, mejor dedica  ese tiempo a crear una función o clase con un buen código, con código limpio.

## Formatos

Cuando los usuarios ven nuestro código queremos que se asombren de lo bien hecho que  esta,  que  parezca  un  trabajo  hecho  por  profesionales,  y  no  solo  un masa amorfa y  desordenada de código

	Quiza como desarrollador, lo más importante es que el código funcione, pero lo es mas que se lea bien
	
Esto debido a que la	funcionalidad puede cambiar en la siguiente versión pero la buena o mala legibilidad del código seguirá ahí.

## Objetos y Estructura de Datos

## Procesar Errores

## Limites

## Pruebas de Unidad

Las tres leyes del desarrollo guiado por pruebas son las siguientes:

	1. No debe crear código de producción hasta que haya creado una prueba para ello.

	2. No debe crear más de una prueba que falle, el no compilar se considera un fallo.

	3. No debe crear más código de producción del necesario para superar dicha prueba
	
Hay que tener en cuenta también que, aunque existan cosas que jamás usaríamos en un entorno de producción, si las podríamos usar en un entorno de pruebas, cada entorno tiene sus propias necesidades.

## Clases

	Una clase debe comenzar con el listado de variables y luego con las funciones públicas, pero las funciones que se esten 
	llamando deben colocarse antes.
	
Es importante que nuestras variables y funciones sean privadas, pero no imprescindible,  podemos hacerlas  protected  para que sean accesibles desde una prueba.  

	Las clases deben ser de tamaño justo y reducido
	
en las funciones nos  fijamos en el número de líneas, pero en las clases la medida serán las responsabilidades; las clases tambien deben tener un número reducido de variables de instancia.

Una  clase o un módulo solo debe tener un único motivo para cambiar, si una clase tiene varios  motivos para cambiar, es que tiene demasiadas dependencias, una manera de solucionarlo  es extraer esos métodos en clases pequeñas que se encarguen únicamente de eso.

## Sistemas

No es lo mismo la construcción que el uso que se le va a dar al sistema. Son procesos  totalmente diferentes, cuando construyen un hotel tenemos grúas y obreros, pero cuando este  acabado no habrá grúas y los trabajadores serán diferentes. 

	Los sistemas de software  deben separar el proceso de inicio, de la lógica de ejecución que toma el testigo tras el 
	inicio.
	
El proceso de inicio es un aspecto que toda aplicación debe abordar. La separación de aspectos es una de las técnicas de diseño más antiguas e importantes de nuestra profesión.
Una forma de separar la construcción del uso consiste en trasladar todos los aspectos de la construcción a main o módulos involucrados por main. La función principal crea los objetos y se los pasa a la aplicación para que los utilice. 

## Emergencia

La calidad es lo mas importante en nuestro trabajo, de nada nos sirve que el codigo se ve comlicado e impresionante si no cumple con todas las funciones requeridas, por eso es importante que:

#### Ejecuta todas las pruebas.  

Se puede tener un buen diseño, pero si no existe una forma sencilla de probar el codigo, el esfuerzo sobre el papel  es cuestionable, y un sistema que no se puede verificar no debe implementarse.

	Crear codigos testables hace que diseñemos clases de tamaño reducido y	un solo cometido, lo que nos conduce a obtener 
	mejores diseños.

#### No contiene duplicados.  

Dentro del codigo podrian existir varias funciones que realizan el mismo proceso, pero trabajan con diferentes variables. Esto puede ser corregido para darle una mejor presentacion y un mayor profsionalismo a nuestro codigo.

#### Expresa la intención del programador.  

El codigo funciona de maravilla, pero otro colega programador necesita realizar algunos cambios para cumplir funciones mas especificas de un proyecto, pero, al momento de entrar se topa con muchas variables y funcinoes con nombres a los cuales no les encuentra sentido ni proposito, por lo que no entiende la intencion de cada apartado.

	Por esto mismo es muy importante manejar estructuras y nombres de variables claros para asi poder transmitir facilmente 
	la intencion de cada funcion

#### Minimiza el número de clases y métodos.

El dividir funciones de nuestro codigo en una gran practica, sin embargo, es importante llegar al punto donde sobredividirlo puesto que se perderia la optimizacion inicial.

## Concurrencia

