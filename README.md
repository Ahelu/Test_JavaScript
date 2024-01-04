# Test de JavaScript 🚀

## Instrucciones para tomar esta prueba

* Evalúa muy críticamente tu conocimiento.<br>
* Si logras resolver la prueba, no importa cuánto te cueste, puedo asegurarte que tienes todo para continuar a las siguientes clases.<br>
* Si no lo logras, absolutamente nadie puede juzgarte, solo tú. Anota los temas clave donde puedes mejorar y estudia vigorosamente.<br>
* Es completamente válido hacer búsquedas en Google, cursos y tutoriales, incluso usar tu cuaderno de notas sin importar si es físico o virtual.

<p align=center> Recuerda, "el éxito no se mide por cuánto tiempo te toma aprender, esa métrica es relativamente inútil". 
<br>¡Mucha suerte!🫰</p> <br>

## Variables y operaciones<br>
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
* ¿Qué es una variable y para qué sirve?<br>
Un espacio reservado en la memoria en el cual se almacena un valor. Una variable puede declarse usando let, const y var. Las palabras reservadas Let & const nacen a partir de ES6 permiten declarar variables de tipo scope, que quiere decir que dependiendo del scope es su accesibilidad.<br>

* ¿Cuál es la diferencia entre declarar e inicializar una variable?<br>
Una variable que se declara no contiene un valor, simplemente se le nombra. Al asignar un tipo y valor a la variable se está "inicializando".<br>

* ¿Cuál es la diferencia entre sumar números y concatenar strings?<br>
El sumar implica realizar una operación aritmetica. El concatenar simplemente une dos valores. Además, en Js esto puede modificar el tipo de variable que obtenemos. Ejem."let suma = 7 + 7;" la variable suma será de tipo number, "let suma = 7 + '4' " la variable suma será de tipo string, "let suma = '7' + '7' " la variable suma será un string.<br>

* ¿Cuál operador me permite sumar o concatenar?<br>
El operador de suma " + "<br>

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:
let Nombre = "Berenice"  -> String. <br>
let Apellido = "Urbina"  -> String. <br>
let Nombre_de_usuario_Platzi = "BereU"  -> String. <br>
let Edad = 30  -> Number. <br>
let Correo_electrónico = "bere_Urbi@gmail.com"  -> String. <br>
let Mayor_de_edad = true / false  -> Boolean. <br>
let Dinero_ahorrado = 1000  -> Number. <br>
let Deudas = 500  ->Number. <br>

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.
```jsx
let Nombre = "Berenice"
let Apellido = "Urbina"
let Nombre_de_usuario_Platzi = "BereU"
let Edad = 30 
let Correo_electrónico = "bere_Urbi@gmail.com"
let Mayor_de_edad = true
let Dinero_ahorrado = 1000
let Deudas = 500
```

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:
let Nombre completo (nombre y apellido)
Dinero real (dinero ahorrado menos deudas)
```jsx
let Nombre = "Berenice";
let Apellido = "Urbina";
let Dinero_ahorrado = 1000;
let Deudas = 500;

console.log(`Mi nombre completo es ${Nombre} ${Apellido}`);

let Dinero_real = Dinero_ahorrado - Deudas;

console.log(`Mi dinero actual es: ${Dinero_real}`);
```
<br>

## Funciones<br>
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
* ¿Qué es una función?<br>
Es un fragmento de codigo que podemos reutilizar, para esto hacemos lo que se conoce como "llamado a la función" en la sección del código en donde la requerimos.
Una función acepta variables como "parametros" que podemos usar en las operaciones u acciones contenidas en la función, como resultado, retorna un valor a través de "return".<br>

* ¿Cuándo me sirve usar una función en mi código?<br>
Cuando existe un fragmento de codigo que describe una operación u acción que podría volver a repetirse en otra sección del código. Esto es reutilizar código. De igual manera podemos usar las funciones en acciones más complejas como "el instanciar objetos".<br>

* ¿Cuál es la diferencia entre parámetros y argumentos de una función?<br>
Son terminos que pueden fácilmente confundirse. Un parámetro es la variable que se declara entre los parentesis de la función(parameto) y el argumento es el valor que se envía através dé.<br>

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:
```jsx
const name="Juan David";
const lastname ="Castro Gallego";
const nickname ="JuanDC";

MinameIs(name,lastname,nickname);

function MinameIs(name,lastname,nickname){
   let completeName = name + " " + lastname;
   return (`Mi nombre es ${completeName} pero prefiero que me digas ${nickname}.`);
};
```
<br>

## Condicionales
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
* ¿Qué es un condicional?<br>
	Se trata una sentencia que nos permiten evaluar o validar datos. Podemos obtener dos resultados: True o False. De ser verdadero se ejecutarán
	ciertas acciones. De igual forma para casos contrarios, es decir, de tipo false.<br>

* ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?<br>
	* Condicional IF: Nos ayuda a evaluar si una condición es verdadera o falsa. Su acción o resultado depende de un valor booleano= true / false.<br>
	* Condicional SWITCH: Nos permite evaluar un cierto numero de opciones o condiciones en base a un valor dado. Similar a if pero con la ventaja de 	poder evaluar diversos casos en una misma sentencia.<br>
	
* ¿Puedo combinar funciones y condicionales?<br>
	Sí. Las funciones son fragmentos de codigo que podemos reutilizar. Los codicionales son sentencias o estructuras de codigo que evaluan un valor. Ejem. Cuando queremos validar si un dato es cierto o falso; si el valor es verdadero se desencadenaran las acciones definidas para los casos de "true". Todo esto podemos contenerlo en una función.

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:
* Switch:
```jsx
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
```
* If y Else if:
```jsx
if(tipoDeSuscripcion == "Free"){  
       console.log("Solo puedes tomar los cursos gratis")
 }else if(tipoDeSuscripcion == "Basic"){
       	console.log("Puedes tomar casi todos los cursos de Platzi durante un mes")
 	}else if(tipoDeSuscripcion == "Expert"){
		console.log("Puedes tomar casi todos los cursos de Platzi durante un año")
		}else if(tipoDeSuscripcion == "ExpertPlus"){
			console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año")
			}else{
			   	console.log("El tipo de suscripción es incorrecta")
				}
```
### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).
* If:
```jsx
if(tipoDeSuscripcion == "Free"){  
	console.log("Solo puedes tomar los cursos gratis");}
if(tipoDeSuscripcion == "Basic"){
	console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");}
if(tipoDeSuscripcion == "Expert"){
	console.log("Puedes tomar casi todos los cursos de Platzi durante un año");}
if(tipoDeSuscripcion == "ExpertPlus"){
	console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");}		
```
💡 Bonus: si ya eres una experta o experto en el lenguaje, te desafío a comentar cómo replicar este comportamiento con arrays u objetos y un solo condicional. 😏
```jsx
//Trabajado con una función y un condicional.
function Suscripciones(tipo){
	switch (tipo) {
		case "Free":
       			return ("Solo puedes tomar los cursos gratis");
       		break;
   		case "Basic":
       			return ("Puedes tomar casi todos los cursos de Platzi durante un mes");
       		break;
   		case "Expert":
       			return ("Puedes tomar casi todos los cursos de Platzi durante un año");
       		break;
   		case "ExpertPlus":
       			return ("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
       		break;
	}
}


//Trabajado con un objeto, una función y un condicional.
let Suscripciones={ 
	Free:"Solo puedes tomar los cursos gratis",
	Basic:"Puedes tomar casi todos los cursos de Platzi durante un mes",
	Expert:"Puedes tomar casi todos los cursos de Platzi durante un año",
	ExpertPlus:"Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"
};

//#1
function BuscarSuscripcion(suscripcion){
	if (Suscripciones[suscripcion]){
		return Suscripciones[suscripcion];
	}else{
		return console.warn ("Suscripción no encontrada");
	}	
}

//#2
let Imprimir= Suscripciones[suscripcion] || "El plan no existe";
console.log(Imprimir)

//#3
Suscripciones[suscripcion]? console.log(Suscripciones[suscripcion]): "El plan no existe";



//Trabajado con un array de objetos, rrecorrido de array y condicional.
let Suscripciones=[ 
 {Free:"Solo puedes tomar los cursos gratis"},
 {Basic:"Puedes tomar casi todos los cursos de Platzi durante un mes"},
 {Expert:"Puedes tomar casi todos los cursos de Platzi durante un año"},
 {ExpertPlus:"Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año"}
];

//#1
let suscripcion= String(prompt("Cuál es su suscripción?"));

let beneficio= Suscripciones.find(function(tipo){
	if(tipo[suscripcion]){
	return (tipo[suscripcion])}
});

console.log(beneficio);


//#2
let suscripcion= String(prompt("Cuál es su suscripción?"));

Suscripciones.find(function(tipo){
	if(tipo[suscripcion]){
	console.log (tipo[suscripcion])}
});
		
```

## Ciclos<br>
### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
* ¿Qué es un ciclo?<br>
	Se trata de una sentencia o sintaxis que permite repetir una misma acción (líneas de codigo) un numero determinado de veces hasta cumplir un ciclo.<br>

* ¿Qué tipos de ciclos existen en JavaScript?<br>
	* Condicional FOR: Permite repetir un ciclo un determinado numero de veces hasta cumplir con una condición dada. <br>
	* Condicional FOR of: Derivado del FOR. Permite repetir una acción o ciclo evaluando los valores de cada elemento. Ejem. Un array dónde, a 	diferencia del for es complejo el poder acceder al indice de los elementos.<br>
	* Condicional WHILE: Toma caracteristicas similares al FOR y el IF. Repite un ciclo un número determinando de veces, siempr ey cuando la condición 	dada se cumpla. Es decir que sea verdadera.<br>
* ¿Qué es un ciclo infinito y por qué es un problema?<br>
	Es un ciclo en el que la condición dada (para que este pueda ejecutarse) es siempre verdadera, por ende no encuentra un final y repide las acciones 	contenidas de forma infinita. Es un problema puesto que implica que alguna variable o condición está mal implementada. <br>
* ¿Puedo mezclar ciclos y condicionales?<br>
	Van de la mano. Para que un ciclo pueda ejecutarse debe estar cumpliendo una condición. Al menos en la mayoría de los casos. Una vez que esta 	condición deja de ser verdadera el ciclo termina.
<br><br>

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:
* For:
```jsx
for (let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

for (let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}
```
* While:
```jsx
let i=0;
while(i<5){
	console.log("El valor de i es: " + i);
	i++
}

let i=10;
while(i>=2){
	console.log("El valor de i es: " + i);
	i--
}
```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es 2 + 2. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.
```jsx
let r=0;
while(r!=4){
 	r= Number(prompt("¿Cuánto es 2 + 2?:"));
 	if(r==4){
		console.log("Felicidades ya sabes contar, 2 + 2 = 4");
	}
}
```

## Listas<br>

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:
* ¿Qué es un array?<br>
	Es una estructura que permite almacenar datos que pueden localizarse por índices. Es un tipo de dato objeto y sus elementos principales son los indices y sus elementos. Ejem. Array= [elemt1,]<br>
 
* ¿Qué es un objeto?<br>
	Es la representación de un objeto físico o de la vida real pero llevado a la programación. Y como todo objeto, tiene propiedades o caracteristicas. Un objeto Se trata de una estructura que permite almacenar valores separados por comas. Ejem. Carro={propiedad:,}<br>
 
* ¿Cuándo es mejor usar objetos o arrays?<br>
	En un array los elementos principales son los indices y los elementos, es decir, valores simples. En el caso de los objetos se trata de estructuras que almacenan valores más complejos llamados propiedades y que a su vez contienen más valores.<br>
 
* ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?<br>
	Sí. Un array es capaz de almacenar uno o más elementos incluso si estos son de tipo objeto. A su vez, un objeto puede almacenar distintos tipos de valores y estructuras incluyendo arrays y funciones.<br>

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.
```jsx
let array=[1,2,3,4,5];

ImprimeArray(array);

function ImprimeArray(arrays){
	console.log(arrays[0])	
}
```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno.
```jsx
let array=[1,2,3,4,5];

ImprimeArray(array);

//#1
function ImprimeArray(arrays){
	arrays.forEach(function(array){
		console.log(array)
	});	
}

//#2
function ImprimeArray(arrays){
	for(elemento of arrays){
		console.log(elemento);
	}	
}
```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno.

```jsx
let auto= {
	tipo:"Jaguar", 
	año: 1999, 
	color:"rojo"
};

ImprimeObjeto(auto);

function ImprimeObjeto(objeto){
	for(elemento in objeto){
		console.log(objeto[elemento]);
	}	
}
```
