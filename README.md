# AD. Evaluación inicial
Evaluación inicial sobre bases de datos y programación en Java. **No se trata de averiguar qué sabe hacer ChatGPT, si no de saber qué sabes hacer tú por ti mismo**. Este repositorio contiene un proyecto de NetBeans en Java. 

**_ES OBLIGATORIO QUE REALICES UN COMMIT TRAS RESOLVER CADA UNO DE LOS EJERCICIOS_** Cuando finalices un ejercicio, realiza un commit en tu repositorio con:
- <ins>Summary (resumen).</ins> "Finalizado ejercicio X - Sección Bases de datos/Programación básica/Programación excepciones". 
- <ins>Descripción</ins>. Dificultades encontradas, **pruebas** realizadas, tiempo de resolución, y si lo has resuelto por ti mismo, o si has recibido ayuda de un compañero/profesor/corrección.

## Bases de datos. SQL
Crea un archivo llamado basesDeDatos_TuNombre.sql en la raiz del repositorio. En este documento de texto, completa los siguientes ejercicios:

1.	Escribe la instrucción para crear una tabla “cliente”. Esta tabla tiene los siguientes campos:
    - id_cliente: entero (este campo es el campo clave). Auto incrementado.
    - nombre: cadena de caracteres variable de tamaño máximo 30. No nulo.
    - dirección: cadena de caracteres de tamaño 50. Nulo. Defecto "C/ Sin nombre, S/N"
    - telefono: cadena de caracteres de tamaño 10. No nulo. Único.
    - fecha nacimiento: fecha. Nulo.
    - puntuación. Entero. No nulo. Defecto 5.
3.	Escribe la instrucción para insertar 3 clientes en esa tabla (inventate los valores, que uno se llame Pepe). Una instrucción introducirá valores para todos los campos, y otra solo los campos obligatorios.
4.	Escribe una instrucción para visualizar todos los registros y toda la información de la tabla cliente.
5.	Escribe una isntrucciónara visualizar la dirección de un cliente llamado "Pepe".
6.	Escribe una instrucción para visualizar el nombre de cliente y el teléfono de todos los clientes de la tabla
7.	Escribe una instrucción para actualizar a nulo la dirección del cliente con número de teléfono "967140000"
8.	Escribe una instrucción para eliminar los clientes cuyo nombre sea "Pepe" o cuya puntuación esté entre 2 y 4 (incluidos).

## Programación básica
Utiliza el proyecto de Java de NetBeans que hay en el repositorio para resolver los siguientes ejercicios:

1. Crea una clase llamada programacionBasica.java, la cual contenga una función ejecutable (main). En ésta, escribe el código necesario para mostrar por pantalla el contenido del siguiente array: int numeros={5,3,1,0,7}
2. Crea una clase “Cliente” que tenga las propiedades :
    - id_cliente: entero
    - nombre: cadena de caracteres 
    - dirección: cadena de caracteres 
    - telefono: cadena de caracteres
    - fechaNacimiento: LocalDate
    - puntuación: entero.
3. En la clase Cliente, añade  un método para visualizar la información de un cliente (toString?!).
4. En la clase Cliente, crea un método void pedirDatos() que pida por pantalla todos los datos de un cliente. No hay que hacer control de excepciones.
5. En la clase Cliente, crea un método void guardarDatos() que escriba los datos de un cliente en un archivo cliente<NombreDelCliente>.txt.
6. Crea una clase UsoCliente.java, la cual contenga un menú con varias opciones que se pidan por teclado (0 salir, 1 añadir cliente, 2 mostrar clientes, 3 eliminar cliente). En la opción 1 se añadirá un nuevo cliente y se guardarán en un objeto ArrayList (que deberás crear también en la clase UsoCliente). En la opción 2 se recorrerá el objeto clientes para mostrar los clientes por pantalla.


## Programación con excepciones
1. Crea una clase programacionExcepciones.java, la cual contenga una función ejecutable. En ésta, escribe un programa en el que pidas dos números enteros por pantalla y calcules su división, para mostrar el resultado por pantalla.
2. Añade al programa anterior el control de excepciones para cuando el usuario introduce por consola algo que no es un número. ¿Qué excepción hay que controlar?
3. Añade al programa anterior el control de excepciones para cuando el usuario introduce como divisor un 0. ¿Qué excepción hay que controlar?
4. En la clase Cliente, añade un método que calcule el número de días que el cliente lleva vivo (Fecha de hoy - fecha de nacimiento). Controla qué ocurre cuando la fecha de nacimiento sea nula a través de una excepción, devolviendo cero. ¿Qué excepción hay que controlar?
5. En la clase UsoCliente, añade una opción de menú que acceda al cliente número 100 del array. Si este cliente no existe, controla la excepción para que muestre el mensaje de error: "El cliente seleccionado no existe". ¿Qué excepción hay que controlar?
6. En la clase Cliente, añade un método que transforme el teléfono de una cadena de caracteres a un entero. Si el teléfono tiene símbolos extraños, que la función devuelva 0. ¿Qué excepción hay que controlar?
