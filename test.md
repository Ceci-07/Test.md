1️⃣ Responde las siguientes preguntas en la sección de comentarios:
*¿Que es una variable? 

-Es la representación de algun lugar en memoria que vamos a reservar, puede tener diferentes tipos.

*Para que sirve?

-Sirve para guardar datos y estados, asignar ciertos valores de variables a otras.

*¿Cuál es la diferencia entre declarar e inicializar una variable?

-Una variable se declara para indicarle al programa a partir de que lugar empieza a existir, que nombre tendrá y que tipo de datos almacenará. La asignacion de un valor inicial se llama inicializacion.

*¿Cuál es la diferencia entre sumar números y concatenar strings? 

-Sumar numeros es una operación matematica y concatenar es unir strings uno tras otro.

¿Cuál operador me permite sumar o concatenar?

El operador que me permite sumar o contatenar es el signo +. Nos permite sumar numeros cuando lo usamos con los mismos. Pero cuando los string, lo que haces es unir (concatenar).

2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

Nombre "String"
Apellido "String"
Nombre de usuario en Platzi "String"
Edad "Number"
Correo electrónico "String"
Mayor de edad "Boolean"
Dinero ahorrado "Number"
Deudas "Number"

3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

let nombre = "Cecilia";
let apellido = "Mansilla";
let username ="Ceci-07";
let edad = 30;
let email = "ceci....@hotmail.com";
let mayorDeEdad = true;
let dineroAhorrado = 500;
let deudas =20000;

4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

let nombreCompleto = Nombre + ' ' + Apellido;
let dineroReal = deudas - dineroAhorrado;

Funciones

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es una función? 

Las funciones son bloques de código a los que se les asigna un nombre. Dentro del bloque de código de una función podemos encontrar lo mismo que encontramos en un algoritmo común, es decir, sentencias secuenciales, estructuras condicionales y estructuras de repetición.

¿Cuándo me sirve usar una función en mi código?

Cuando necesitamos repetir una acción en nuestro código, en vez de escribir una suma, por ejemplo en cada línea, podemos crear una función que nos permita sumar elementos cada vez que lo necesitemos y solo cambiamos sus parámetros.

¿Cuál es la diferencia entre parámetros y argumentos de una función?

Los parametros son los nombres que aparecen en la definicion de una función. Por otro lado los argumentos son los valores que le pasamos y que por lo tanto recibe una función.

2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

const myPresentation = function(name, lastname, nickname) {
    return console.log(`Minombre es ${name} ${lastname}, 
pero prefiero que me digas ${nickname}`);
}
myPresentation ("Juan David", "Castro Gallego", "juandc");

Condicionales

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es un condicional?

Son reglas que aplicamos para validar si algo es verdadero o falso y podamos generar ciertas acciones

¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias? 

Existen IF(ELSE IF, ELSE)- SWITCH.
En la condición IF puedes evaluar condiciones y dependiendo de si es true o false se ejecutará el bloque de código que esté dentro de esta condicional. Por otro lado con la condición SWITCH se evalúan casos no condicionales (evalúa especificamente valores).

¿Puedo combinar funciones y condicionales? 

Si, se pueden combinar

2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

const tipoDeSuscripcion = "Basic";

switch (tipoDeSuscripcion) {
   case "Free":
       console.log("Solo puedes tomar los cursos gratis");
       break;
   case "Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
       break;
   case "Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
       break;
   case "ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       break;
}

const tipoDeSuscripcion = "Expert";
if (tipoDeSuscripcion == 'free') {
    console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion == 'Basic'){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if (tipoDeSuscripcion == 'Expert'){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else if(tipoDeSuscripcion == 'ExpertPlus') {
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏
```js
const (tipoDeSuscripcion) = "Basic";

if(free){
    console.log("Solo puedes tomar los cursos gratis");
} else if (Basic){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if (Expert){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else (ExpertPlus){
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}
```

con if unicamente
```js
const (tipoDeSuscripcion) = "Basic";

if(tipoDeSuscripcion === "free"){
    console.log("Solo puedes tomar los cursos gratis");
} if (tipoDeSuscripcion === "Basic"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} if (tipoDeSuscripcion === "Expert"){
    console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} if (tipoDeSuscripcion === "ExpertPlus"){
    console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}
```
con arrays 

```js
const tipoDeSuscripción = { 
Free:'solo puedes tomar los cursos gratis',
Basic: 'puedes tomar casi todos los cursos de Platzi durante un mes',
Expert :'puedes tomar casi todos los cursos de Platzi durante un año',
ExpertPlus: 'tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año',
};



let userDeSuscription = "Expert";
    for (let i=0; i < tipoDeSuscripción.length; i++) {
      if (userDeSuscription == tipoDeSuscripción[i]) {
          console.log(`Si estas suscrito al plan ${tipoDeSuscripción[i]} en el cual ${infoSuscripción[i]}`)
      }
    }
 ```
Ciclos

1️⃣ Responde las siguientes preguntas en la sección de comentarios:
¿Qué es un ciclo?

 Son aquellos que son utilizados para realizar tareas repetitivas con base en una condicion. Tipicamente devuelven true o false al ser evaluados. El bucle continua ejecutandose hasta que la condicion devuelva false

¿Qué tipos de ciclos existen en JavaScript?

While, do while y for.

¿Qué es un ciclo infinito y por qué es un problema?

Un ciclo infinito es aquel que nos permite ejecutar un bloque de código varias veces seguidas, es un error que consiste en realizar un ciclo que se repite de forma indefinida ya que su condición para finalizar nunca se cumple.

¿Puedo mezclar ciclos y condicionales?

Si, se puede mezclar.Aunque los ciclos son una especie de condicionales nada nos impide agregar más condicionales dentro del ciclo.

2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while

for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}

con while
let i = 0
while (i < 5) {
    console.log("El valor de i es: " + i);
    i++;
}
let i = 10;
while (i  >= 2) {
    console.log("El valor de i es: " + i);
    i--;
}

3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2.
Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.
```js
let respuesta;

while (respuesta != '4'){
    let pregunta = prompt ('¿Cuánto es 2 + 2?')
    respuesta = pregunta;
}
```

Listas

1️⃣ Responde las siguientes preguntas en la sección de comentarios:

¿Qué es un array?

Es una estructura de datos de tipo objeto que guarda mas valores adentro como numeros, string, objetos, booleanos.

¿Qué es un objeto?

Es un entidad independiente con propiedades y tipos.

¿Cuándo es mejor usar objetos o arrays?

Las dos son muy utiles y pueden almacenar gran cantidad de datos. Los objetos suelen ser utiles cuando necesitamos almacenar gran cantidad de datos que van a ser accedidos por medio de variables.

¿Puedo mezclar arrays con objetos o incluso objetos con arrays?

Sí, y de esta forma los arrays pueden tener objetos como elementos; podemos usar el spread operator para convertir arrays en objetos.

2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
```js
consol verduras = ["Zapallo", "Zanahoria", "Brócoli", "Batata"]

console.log(verduras[0]);
```

3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```js
console.log(verduras);
```

4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

consol miMoto = {
    marca: "Yamaha",
    modelo: "Xmax 300",
    annio: "2000",
}

miMoto
{marca: 'Yamaha', modelo: 'Xmax 300', annio: '2000'}

miMoto.marca
'Yamaha'

miMoto.annio
'2000'

var miMoto = {
    marca: "Yamaha",
    modelo: "Xmax 300",
    annio: "2000",
    detalledelaMoto: function () {
        console.log (`Moto ${this.modelo} ${this.annio}`)}
    };


miMoto.detalledelaMoto();
VM757: Moto Xmax 300 2000