## Semana 2 Core-Code
### Objetitivo de la semana: 
Aprender acerca de de JavaScript

### Sub topicos de la semana:
* Tipos de datos

    * undefined
       > Una variable a la que no se le ha asignado valor, o no se ha declarado en absoluto (no se declara, no existe) son de tipo undefined. Un método o sentencia también devuelve undefined si la variable que se está evaluando no tiene asignado un valor.

        ```javascript
        let x;
        x === undefined ?
        console.log("No tiene un valor asignado: < ", x," >") :
        console.log("Si tiene un valor asignado: < ",x," >")
        ```




    * null
        >El valor null es un literal de Javascript que representa intencionalmente un valor nulo o "vacío". Es uno de los valores primitivos de Javascript.

        ```javascript
            function getvowels(str){
            const vowels = str.match(/[aeiou]/gi);
            vowels === null ? console.log(0) :
            console.log(vowels.length)
            }
            console.log(getvowels('Angel'));

            //salida esperada = 2
        ```  

    * var 
        >La sentencia var declara una variable, opcionalmente inicializándola con un valor.

        ```javascript
        var name_var = "nombre"  
        ```
    * let
        >La instrucción let declara una variable de alcance local con ámbito de bloque(block scope), la cual, opcionalmente, puede ser inicializada con algún valor.

        ```javascript
        let nombre = "LUNA"

        function ImprimirNombre(nombre){
        nombre = "ADA ABIGAIL!"
        if (nombre === null ){
            console.log("nombre Esta definido pero  es de valor nulo")
        }else{
            console.log("El valor de nombre es:",   nombre)
            }
        }
        console.log(ImprimirNombre(nombre))  
        ```
    * const
        >Las variables constantes presentan un ámbito de bloque (block scope) tal y como lo hacen las variables definidas usando la instrucción let, con la particularidad de que el valor de una constante no puede cambiarse a través de la reasignación. Las constantes no se pueden redeclarar.

        ```javascript
        function PrintPi(){
        const Pi = 3.1416
        console.log(Pi = "hola")}
        console.log(PrintPi())
        //TypeError: Assignment to constant     variable.  
        ```
* Operadores
    * Aritmeticos:
        | Perador | Nombre | Proposito| Ejemplo|
        |---|---|---|---|
        | + | Adición | Suma dos número juntos |6 + 9 
        | - | Resta | Resta el número de la izquierda del de la deracha |20 - 15
        | * | Multiplicación | Multiplica dos números juntos |3 * 7  
        | / | División | Divide el número de la izquiera por el de la derecha |10 / 5
        | % | Sobrante(Modulo) | Retorna el restante despues de dividir el número de la izquierda en porciones enteras del de la derecha |8 / 3 (Retorna 2, como 3 está 2 veces en 8, quedando 2 de resto)
    * TypeOf
        > El operador typeof se usa en cualquiera de los siguientes modos:
        El operador typeof se usa en cualquiera de los siguientes modos:
        typeof operando
        typeof (operando)
        El operador typeof devuelve una cadena que indica el tipo del operando sin evaluarlo. operando es la cadena, variable, palabra clave u objeto para el que se devolverá su tipo. Los paréntesis son opcionales.            