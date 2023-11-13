 1. [Enlace a Objetos Globales](#1-objetos-globales)
- 1.1 Objetos globales en JavaScript
- 1.2 Métodos y propiedades de objetos globales

 2. [Propiedades de Tipo Valor](#2-propiedades-de-tipo-valor-1)
- 2.1 globalThis
- 2.2 Infinity
- 2.3 NaN
- 2.4 undefined

 3. [Propiedades de Tipo Función](#3-propiedades-de-tipo-funcin-1)
- 3.1 eval()
- 3.2 isFinite()
- 3.3 isNaN()
- 3.4 parseFloat()
- 3.5 parseInt()
- 3.6 decodeURI()
- 3.7 decodeURIComponent()
- 3.8 encodeURI()
- 3.9 encodeURIComponent()

 4. [Objetos Fundamentales](#4-objetos-fundamentales)
- 4.1 Object
- 4.2 Function
- 4.3 Boolean
- 4.4 Symbol

 5.[ Objetos de Errores](#5-objetos-de-errores)
- 5.1 Error
- 5.2 EvalError
- 5.3 RangeError
- 5.4 ReferenceError
- 5.5 SyntaxError
- 5.6 TypeError
- 5.7 URIError
- 5.8 AggregateError

 6.[ Números y Fechas](#6-nmeros-y-fechas)
- 6.1 Number
- 6.2 BigInt
- 6.3 Math
- 6.4 Date

 7. [Procesamiento de Texto](#7-procesamiento-de-texto)
- 7.1 String
- 7.2 RegExp

 8. Colecciones Indexadas
- 8.1 Array
- 8.2 Int8Array
- 8.3 Uint8Array
- 8.4 Uint8ClampedArray
- 8.5 Int16Array
- 8.6 Uint16Array
- 8.7 Int32Array
- 8.8 Uint32Array
- 8.9 BigInt64Array
- 8.10 BigUint64Array
- 8.11 Float32Array
- 8.12 Float64Array

 9. [Colecciones con Campos Clave](#9-colecciones-con-campos-clave)
- 9.1 Map
- 9.2 Set
- 9.3 WeakMap
- 9.4 WeakSet

 10.[ Datos Estructurados](#10-datos-estructurados)
- 10.1 ArrayBuffer
- 10.2 SharedArrayBuffer
- 10.3 DataView
- 10.4 Atomics
- 10.5 JSON

 11. [Gestión de Memoria](#11-gestin-de-memoria)
- 11.1 WeakRef
- 11.2 FinalizationRegistry

 12. [Abstracción de Control](#12-abstraccin-de-control)
- 12.1 Promise
- 12.2 GeneratorFunction
- 12.3 AsyncGeneratorFunction
- 12.4 Generator
- 12.5 AsyncGenerator
- 12.6 AsyncFunction

 13. [Reflexión](#13-reflexin)
- 13.1 Reflect
- 13.2 Proxy

 14. [Internacionalización](#14-internacionalizacin)
- 14.1 Intl
- 14.2 Intl.Collator
- 14.3 Intl.DateTimeFormat
- 14.4 Intl.DisplayNames
- 14.5 Intl.ListFormat
- 14.6 Intl.Locale
- 14.7 Intl.NumberFormat
- 14.8 Intl.PluralRules
- 14.9 Intl.RelativeTimeFormat

 15. [WebAssembly](#15-webassembly)
- 15.1 WebAssembly
- 15.2 WebAssembly.Module
- 15.3 WebAssembly.Instance
- 15.4 WebAssembly.Memory
- 15.5 WebAssembly.Table
- 15.6 WebAssembly.CompileError
- 15.7 WebAssembly.LinkError
- 15.8 WebAssembly.RuntimeError

 16. [Sentencias](#16-sentencias)
- 16.1 Declaraciones y sentencias en JavaScript

 17. [Control de Flujo](#17-control-de-flujo)
- 17.1 Block
- 17.2 Empty statement
- 17.3 break
- 17.4 continue
- 17.5 if...else
- 17.6 switch
- 17.7 throw
- 17.8 try...catch

 18. [Declaraciones](#18-declaraciones)
- 18.1 var
- 18.2 let
- 18.3 const

 19. [Funciones y Clases](#19-funciones-y-clases)
- 19.1 function
- 19.2 function*
- 19.3 async function
- 19.4 return
- 19.5 class

 20. [Iteraciones](#20-iteraciones)
- 20.1 do...while
- 20.2 for
- 20.3 for...in
- 20.4 for...of
- 20.5 for await...of
- 20.6 while

 21. [Otros](#21-otros)
- 21.1 debugger
- 21.2 export
- 21.3 import
- 21.4 label
- 21.5 with

 22. [Operadores y Expresiones](#22-operadores-y-expresiones)
- 22.1 Expresiones primarias
- 22.2 Expresiones del lado izquierdo
- 22.3 Incremento y decremento
- 22.4 Operadores unarios
- 22.5 Operadores aritméticos
- 22.6 Operadores relacionales
- 22.7 Operadores de igualdad
- 22.8 Operadores de desplazamiento bit a bit
- 22.9 Operadores binarios bitwise
- 22.10 Operadores lógicos bitwise
- 22.11 Operador condicional (ternario)
- 22.12 Operadores de asignación
- 22.13 [a, b] = [1, 2]
- 22.14 {a, b} = {a:1, b:2}
- 22.15 Operador coma

 23. [Funciones](#23-funciones)
- 23.1 argumentos
- 23.2 Funciones flecha
- 23.3 Parámetros por defecto
- 23.4 Parámetros rest

 24. [Misceláneos](#24-miscelneos)
- 24.1 Gramática léxica
- 24.2 Tipos de datos y estructuras
- 24.3 Modo estricto
- 24.4 Características en desuso



# 1. Objetos Globales
## 1.1 Objetos globales en JavaScript

En JavaScript, los objetos globales son aquellos que están disponibles en todo el entorno de ejecución y no están vinculados a un objeto específico. Algunos de los objetos globales comunes incluyen `window` en el contexto del navegador y `global` en el contexto de Node.js.

```javascript
// Ejemplo en un navegador
console.log(window.document); // Accede al objeto document

// Ejemplo en Node.js
console.log(global.process); // Accede al objeto process
```

## 1.2 Métodos y propiedades de objetos globales

Los objetos globales también tienen métodos y propiedades integrados que se pueden utilizar en cualquier parte del código. Algunos ejemplos son `setTimeout`, `setInterval`, y `console`.

```javascript
// setTimeout: Ejecuta una función después de un tiempo específico
setTimeout(() => {
  console.log("¡Hola después de 2 segundos!");
}, 2000);

// console.log: Muestra mensajes en la consola
console.log("Hola, esto es un mensaje de registro");

// setInterval: Ejecuta una función repetidamente cada cierto intervalo de tiempo
setInterval(() => {
  console.log("¡Hola cada segundo!");
}, 1000);
```

Continuaré con el siguiente tema:

# 2. Propiedades de Tipo Valor
## 2.1 globalThis

El objeto `globalThis` es una referencia al objeto global, independientemente del entorno en el que se esté ejecutando el código (navegador, Node.js, etc.). Es una forma consistente de acceder al objeto global.

```javascript
// Uso de globalThis en diferentes entornos
console.log(globalThis); // En un navegador
console.log(globalThis === window); // true en un navegador
console.log(globalThis === global); // true en Node.js
```

## 2.2 Infinity

`Infinity` es un valor numérico que representa el infinito matemático.

```javascript
let infinityValue = Infinity;
console.log(infinityValue); // Imprime Infinity
console.log(1 / 0); // También da Infinity
```

## 2.3 NaN

`NaN` significa "Not a Number" y se utiliza para representar un valor no numérico que no es igual a ningún otro número, incluido a sí mismo.

```javascript
let notANumber = NaN;
console.log(notANumber); // Imprime NaN
console.log(isNaN(notANumber)); // true
```

## 2.4 undefined

`undefined` es un valor primitivo que se asigna automáticamente a las variables que se han declarado pero no se les ha asignado un valor.

```javascript
let undefinedValue;
console.log(undefinedValue); // Imprime undefined
```

# 3. Propiedades de Tipo Función
## 3.1 eval()

La función `eval()` evalúa una cadena de texto como código JavaScript en tiempo de ejecución.

```javascript
let x = 10;
let y = 20;
let result = eval('x + y');
console.log(result); // Imprime 30
```

Es importante usar `eval()` con precaución, ya que puede introducir vulnerabilidades de seguridad si se utiliza con datos no confiables.

## 3.2 isFinite()

La función `isFinite()` verifica si un valor es finito (diferente de `Infinity` o `-Infinity`) y es un número. Devuelve `true` si es así, de lo contrario, devuelve `false`.

```javascript
console.log(isFinite(42)); // true
console.log(isFinite(Infinity)); // false
console.log(isFinite("Hola")); // false
```

## 3.3 isNaN()

La función `isNaN()` verifica si un valor no es un número. Devuelve `true` si el valor no es un número, de lo contrario, devuelve `false`.

```javascript
console.log(isNaN(42)); // false
console.log(isNaN("Hola")); // true
```

## 3.4 parseFloat()

La función `parseFloat()` analiza una cadena y devuelve un número de punto flotante.

```javascript
let floatValue = parseFloat("3.14");
console.log(floatValue); // Imprime 3.14
```

## 3.5 parseInt()

La función `parseInt()` analiza una cadena y devuelve un entero.

```javascript
let intValue = parseInt("42");
console.log(intValue); // Imprime 42
```

## 3.6 decodeURI()

La función `decodeURI()` decodifica un Identificador de Recursos Uniforme (URI) previamente codificado.

```javascript
let encodedURI = "https%3A%2F%2Fwww.example.com%2F";
let decodedURI = decodeURI(encodedURI);
console.log(decodedURI); // Imprime https://www.example.com/
```

## 3.7 decodeURIComponent()

Similar a `decodeURI()`, pero se enfoca en decodificar componentes de un URI.

## 3.8 encodeURI()

La función `encodeURI()` codifica un URI.

## 3.9 encodeURIComponent()

Similar a `encodeURI()`, pero se enfoca en codificar componentes de un URI.

# 4. Objetos Fundamentales
## 4.1 Object

El objeto `Object` es la base de todos los objetos en JavaScript. Proporciona propiedades y métodos que son comunes a todos los objetos.

```javascript
let obj = {
  key1: 'value1',
  key2: 'value2'
};

// Accediendo a las propiedades con notación de punto
console.log(obj.key1); // Imprime 'value1'

// Accediendo a las propiedades con notación de corchetes
console.log(obj['key2']); // Imprime 'value2'

// Métodos de Object
console.log(Object.keys(obj)); // Imprime ['key1', 'key2']
console.log(Object.values(obj)); // Imprime ['value1', 'value2']
```

## 4.2 Function

El objeto `Function` es una función predefinida en JavaScript que se puede utilizar para crear funciones.

```javascript
// Definir una función utilizando la sintaxis de declaración de función
function greet(name) {
  console.log('Hola, ' + name + '!');
}

// Definir una función utilizando la expresión de función
let multiply = function (a, b) {
  return a * b;
};

greet('Juan'); // Imprime 'Hola, Juan!'
console.log(multiply(3, 4)); // Imprime 12
```

## 4.3 Boolean

El objeto `Boolean` es un objeto que envuelve un valor booleano.

```javascript
let boolObj = new Boolean(true);
console.log(boolObj.valueOf()); // Imprime true

let boolPrimitive = true;
console.log(boolPrimitive.valueOf()); // Imprime true
```

## 4.4 Symbol

`Symbol` es un tipo de dato primitivo y también un constructor para objetos símbolo.

```javascript
// Crear un símbolo único
let symbol1 = Symbol('description');
let symbol2 = Symbol('description');

console.log(symbol1 === symbol2); // false, cada símbolo es único
```
# 5. Objetos de Errores
## 5.1 Error

El objeto `Error` representa un error en tiempo de ejecución y se utiliza como base para otros objetos de error.

```javascript
try {
  // Código que puede lanzar un error
  throw new Error('Este es un error personalizado');
} catch (error) {
  console.error(error.message); // Imprime 'Este es un error personalizado'
}
```

## 5.2 EvalError

El objeto `EvalError` indica un error con la función `eval()`.

```javascript
try {
  throw new EvalError('Este es un error de eval');
} catch (error) {
  console.error(error.message); // Imprime 'Este es un error de eval'
}
```

## 5.3 RangeError

El objeto `RangeError` indica un error cuando un valor está fuera del rango permitido.

```javascript
try {
  throw new RangeError('Este es un error de rango');
} catch (error) {
  console.error(error.message); // Imprime 'Este es un error de rango'
}
```

## 5.4 ReferenceError

El objeto `ReferenceError` indica un error cuando se referencia a una variable no definida.

```javascript
try {
  throw new ReferenceError('Este es un error de referencia');
} catch (error) {
  console.error(error.message); // Imprime 'Este es un error de referencia'
}
```

## 5.5 SyntaxError

El objeto `SyntaxError` indica un error de sintaxis.

```javascript
try {
  // Error de sintaxis: falta un punto y coma
  eval('alert("Hola")')
} catch (error) {
  console.error(error.message); // Imprime 'Unexpected identifier'
}
```

## 5.6 TypeError

El objeto `TypeError` indica un error cuando se produce una operación incompatible.

```javascript
try {
  // Intentando llamar a un número como una función
  let num = 42;
  num(); // Esto lanzará un TypeError
} catch (error) {
  console.error(error.message); // Imprime 'num is not a function'
}
```

## 5.7 URIError

El objeto `URIError` indica un error cuando se utiliza funciones relacionadas con URI.

```javascript
try {
  decodeURI('%'); // Esto lanzará un URIError
} catch (error) {
  console.error(error.message); // Imprime 'URI malformed'
}
```

## 5.8 AggregateError

El objeto `AggregateError` representa un error que agrupa varios errores en uno.

```javascript
try {
  throw new AggregateError([
    new Error('Error 1'),
    new RangeError('Error 2'),
    'Mensaje de error adicional'
  ]);
} catch (error) {
  console.error(error.message); // Imprime 'Error 1; Error 2; Mensaje de error adicional'
}
```
# 6. Números y Fechas
## 6.1 Number

El objeto `Number` es un objeto global que permite trabajar con valores numéricos.

```javascript
let num = new Number(42);
console.log(num.valueOf()); // Imprime 42

// Propiedades estáticas de Number
console.log(Number.MAX_VALUE); // Valor máximo representable
console.log(Number.MIN_VALUE); // Valor mínimo representable
console.log(Number.NaN); // Representa "Not a Number"
console.log(Number.POSITIVE_INFINITY); // Infinito positivo
console.log(Number.NEGATIVE_INFINITY); // Infinito negativo
```

## 6.2 BigInt

El objeto `BigInt` permite representar números enteros arbitrariamente grandes.

```javascript
const bigIntValue = BigInt(Number.MAX_SAFE_INTEGER) + BigInt(1);
console.log(bigIntValue); // Imprime un número más grande que el valor máximo seguro de Number
```

## 6.3 Math

El objeto `Math` proporciona funciones y constantes matemáticas.

```javascript
console.log(Math.sqrt(25)); // Raíz cuadrada, imprime 5
console.log(Math.PI); // Constante PI
console.log(Math.random()); // Número aleatorio entre 0 (inclusive) y 1 (exclusivo)
```

## 6.4 Date

El objeto `Date` permite trabajar con fechas y horas.

```javascript
let currentDate = new Date();
console.log(currentDate); // Imprime la fecha y hora actual

// Crear una fecha específica
let specificDate = new Date('2023-11-13T12:00:00Z');
console.log(specificDate);
```

# 7. Procesamiento de Texto
## 7.1 String

El objeto `String` representa una secuencia de caracteres y proporciona métodos para trabajar con texto.

```javascript
let myString = 'Hola, mundo!';

// Obtener la longitud de la cadena
console.log(myString.length); // Imprime 13

// Convertir a mayúsculas
console.log(myString.toUpperCase()); // Imprime 'HOLA, MUNDO!'

// Obtener un carácter en una posición específica
console.log(myString.charAt(0)); // Imprime 'H'

// Buscar la posición de un subcadena
console.log(myString.indexOf('mundo')); // Imprime 7
```

## 7.2 RegExp

El objeto `RegExp` se utiliza para trabajar con expresiones regulares, que son patrones utilizados para realizar búsquedas y manipulación de texto.

```javascript
// Crear una expresión regular para buscar números
let regex = /\d+/;

// Testear si la expresión regular coincide con la cadena
console.log(regex.test('abc123')); // Imprime true

// Encontrar coincidencias en una cadena
console.log('abc123xyz456'.match(regex)); // Imprime ['123']
```
# 8. Colecciones Indexadas
## 8.1 Array

El objeto `Array` representa una colección ordenada de elementos.

```javascript
let fruits = ['Manzana', 'Plátano', 'Uva'];

// Acceder a elementos por índice
console.log(fruits[0]); // Imprime 'Manzana'

// Añadir elementos al final del array
fruits.push('Naranja');

// Iterar sobre elementos
for (let fruit of fruits) {
  console.log(fruit);
}

// Métodos útiles de Array
console.log(fruits.length); // Imprime 4
console.log(fruits.indexOf('Plátano')); // Imprime 1
```

## 8.2 Int8Array, 8.3 Uint8Array, ..., 8.12 Float64Array

Estos son tipos de arrays tipados que permiten trabajar con datos binarios de manera más eficiente.

```javascript
// Crear un Int8Array con longitud 4
let intArray = new Int8Array(4);

// Asignar valores
intArray[0] = 42;
intArray[1] = 10;

console.log(intArray); // Imprime Int8Array [42, 10, 0, 0]
```

## 8.13 BigInt64Array, 8.14 BigUint64Array

Tipos de arrays tipados que trabajan con enteros grandes (BigInt).

```javascript
let bigIntArray = new BigInt64Array([10n, 20n, 30n]);

console.log(bigIntArray); // Imprime BigInt64Array [10n, 20n, 30n]
```
# 9. Colecciones con Campos Clave
## 9.1 Map

El objeto `Map` es una colección de pares clave/valor donde las claves pueden ser de cualquier tipo.

```javascript
let myMap = new Map();

// Agregar elementos
myMap.set('key1', 'valor1');
myMap.set(2, 'valor2');

// Obtener valores por clave
console.log(myMap.get('key1')); // Imprime 'valor1'

// Iterar sobre pares clave/valor
for (let [key, value] of myMap) {
  console.log(key, value);
}
```

## 9.2 Set

El objeto `Set` es una colección de valores únicos.

```javascript
let mySet = new Set();

// Agregar elementos
mySet.add('valor1');
mySet.add('valor2');
mySet.add('valor1'); // No se agregará, ya que los sets solo aceptan valores únicos

// Verificar si un elemento está en el set
console.log(mySet.has('valor1')); // true

// Iterar sobre elementos
for (let value of mySet) {
  console.log(value);
}
```

## 9.3 WeakMap y 9.4 WeakSet

Estas son variantes de `Map` y `Set` respectivamente, pero con algunas diferencias importantes. Los objetos en un `WeakMap` y los valores en un `WeakSet` pueden ser eliminados por el recolector de basura si no hay otras referencias a ellos.

```javascript
let weakMap = new WeakMap();
let weakSet = new WeakSet();

let keyObj = {};
let valueObj = {};

// Agregar elementos a WeakMap
weakMap.set(keyObj, 'valor');

// Agregar elementos a WeakSet
weakSet.add(valueObj);

// Los objetos pueden ser recolectados por el recolector de basura
keyObj = null;
valueObj = null;
```
# 10. Datos Estructurados
## 10.1 ArrayBuffer

El objeto `ArrayBuffer` es un contenedor de datos binarios de longitud fija.

```javascript
let buffer = new ArrayBuffer(16); // Crear un ArrayBuffer de 16 bytes

// Obtener la longitud del ArrayBuffer en bytes
console.log(buffer.byteLength); // Imprime 16
```

## 10.2 SharedArrayBuffer

Similar a `ArrayBuffer`, pero diseñado para ser compartido entre hilos en un entorno de ejecución de múltiples hilos.

```javascript
let sharedBuffer = new SharedArrayBuffer(16);
```

## 10.3 DataView

El objeto `DataView` proporciona una interfaz para leer y escribir datos en un `ArrayBuffer`.

```javascript
let buffer = new ArrayBuffer(4);
let view = new DataView(buffer);

// Escribir un entero de 32 bits en la posición 0
view.setInt32(0, 42);

// Leer el entero de 32 bits desde la posición 0
console.log(view.getInt32(0)); // Imprime 42
```

## 10.4 Atomics

El objeto `Atomics` proporciona operaciones atómicas sobre arreglos `SharedArrayBuffer` que pueden ser compartidos entre hilos.

```javascript
let sharedBuffer = new SharedArrayBuffer(4);
let sharedArray = new Int32Array(sharedBuffer);

// Incrementar el valor en la posición 0 de manera atómica
Atomics.add(sharedArray, 0, 5);

console.log(sharedArray[0]); // Dependiendo del comportamiento concurrente, podría ser 5 u otro valor
```

## 10.5 JSON

El objeto `JSON` proporciona métodos para trabajar con datos en formato JSON.

```javascript
let jsonData = '{"name": "John", "age": 30}';
let parsedData = JSON.parse(jsonData);

console.log(parsedData.name); // Imprime 'John'
```
# 11. Gestión de Memoria
## 11.1 WeakRef

El objeto `WeakRef` permite crear referencias débiles a objetos, lo que significa que no impide que el recolector de basura recolecte el objeto.

```javascript
let obj = { data: 'Información importante' };
let weakRef = new WeakRef(obj);

// Obtener el objeto desde la referencia débil
let retrievedObj = weakRef.deref();

console.log(retrievedObj.data); // Imprime 'Información importante'
```

## 11.2 FinalizationRegistry

El objeto `FinalizationRegistry` permite realizar acciones cuando un objeto es recolectado por el recolector de basura.

```javascript
let registry = new FinalizationRegistry((heldValue) => {
  console.log(`Objeto recolectado: ${heldValue}`);
});

let obj = { data: 'Información sensible' };

// Registrar el objeto para ser observado
registry.register(obj, 'Valor retenido');

// Eliminar la referencia al objeto
obj = null;

// Dependiendo del comportamiento del recolector de basura, el callback puede ejecutarse cuando se recolecta el objeto
```
# 12. Abstracción de Control
## 12.1 Promise

El objeto `Promise` representa un valor que puede estar disponible ahora, en el futuro o nunca.

```javascript
// Crear una promesa
let myPromise = new Promise((resolve, reject) => {
  // Lógica asíncrona, por ejemplo, una solicitud HTTP
  let success = true;

  if (success) {
    resolve('Éxito');
  } else {
    reject('Error');
  }
});

// Manejar el resultado de la promesa
myPromise.then((result) => {
  console.log(result); // Imprime 'Éxito'
}).catch((error) => {
  console.error(error); // Imprime 'Error' si la promesa es rechazada
});
```

## 12.2 GeneratorFunction, 12.3 AsyncGeneratorFunction

Las funciones generadoras (`GeneratorFunction`) y las funciones generadoras asíncronas (`AsyncGeneratorFunction`) permiten pausar y reanudar la ejecución, lo que es útil para escribir código asíncrono de manera más legible.

```javascript
// GeneratorFunction
function* myGenerator() {
  yield 1;
  yield 2;
  yield 3;
}

// Crear un generador
let generator = myGenerator();

console.log(generator.next()); // Imprime { value: 1, done: false }
console.log(generator.next()); // Imprime { value: 2, done: false }
console.log(generator.next()); // Imprime { value: 3, done: false }
console.log(generator.next()); // Imprime { value: undefined, done: true }

// AsyncGeneratorFunction
async function* myAsyncGenerator() {
  yield await Promise.resolve(1);
  yield await Promise.resolve(2);
  yield await Promise.resolve(3);
}

// Crear un generador asíncrono
let asyncGenerator = myAsyncGenerator();

(async () => {
  console.log(await asyncGenerator.next()); // Imprime { value: 1, done: false }
  console.log(await asyncGenerator.next()); // Imprime { value: 2, done: false }
  console.log(await asyncGenerator.next()); // Imprime { value: 3, done: false }
  console.log(await asyncGenerator.next()); // Imprime { value: undefined, done: true }
})();
```

## 12.4 Generator, 12.5 AsyncGenerator, 12.6 AsyncFunction

Estos son los tipos de instancias que se crean cuando se llama a un generador o una función asíncrona.

```javascript
// Generator
let generatorInstance = myGenerator();

// AsyncGenerator
let asyncGeneratorInstance = myAsyncGenerator();

// AsyncFunction
let asyncFunctionInstance = async function () {
  return 'Hola desde una función asíncrona';
};
```
# 13. Reflexión
## 13.1 Reflect

El objeto `Reflect` proporciona métodos estáticos que son equivalentes a algunas operaciones realizadas en objetos.

```javascript
let obj = { prop: 'valor' };

// Obtener todas las claves de un objeto usando Reflect
let keys = Reflect.ownKeys(obj);
console.log(keys); // Imprime ['prop']
```

## 13.2 Proxy

El objeto `Proxy` se utiliza para definir comportamientos personalizados para operaciones fundamentales (por ejemplo, lectura, escritura, enumeración) en un objeto.

```javascript
let target = {};
let handler = {
  get: function (obj, prop) {
    return prop in obj ? obj[prop] : 'No existe';
  }
};

let proxy = new Proxy(target, handler);

console.log(proxy.prop1); // Imprime 'No existe'
```

Los objetos `Reflect` y `Proxy` son poderosos para la manipulación y observación de objetos en tiempo de ejecución.

# 14. Internacionalización
## 14.1 Intl, 14.2 Intl.Collator, ..., 14.9 Intl.RelativeTimeFormat

El objeto `Intl` y sus subobjetos proporcionan soporte para internacionalización y localización de aplicaciones.

```javascript
let number = 1234567.89;

// Formatear un número con formato de moneda
let formattedNumber = new Intl.NumberFormat('es-ES', { style: 'currency', currency: 'EUR' }).format(number);
console.log(formattedNumber); // Imprime '1.234.567,89 €'
```

Esto es especialmente útil para aplicaciones que necesitan manejar formatos de números, fechas y texto en diferentes idiomas y regiones.

# 15. WebAssembly
## 15.1 WebAssembly, 15.2 WebAssembly.Module, ..., 15.8 WebAssembly.RuntimeError

WebAssembly es un formato binario seguro y eficiente diseñado para ejecutarse en navegadores web, pero también puede ejecutarse fuera del navegador.

```javascript
// Crear un módulo de WebAssembly desde código fuente
const sourceCode = '(module (func (result i32) i32.const 42))';
const wasmModule = new WebAssembly.Module(new TextEncoder().encode(sourceCode));

// Crear una instancia de WebAssembly.Module
const wasmInstance = new WebAssembly.Instance(wasmModule);

// Llamar a la función exportada
const result = wasmInstance.exports.func();
console.log(result); // Imprime 42
```
# 16. Sentencias
## 16.1 Declaraciones y sentencias en JavaScript

JavaScript utiliza declaraciones y sentencias para definir el comportamiento de un programa.

```javascript
// Declaración de variable
let x;

// Asignación de valor
x = 42;

// Declaración y asignación en una línea
let y = 10;

// Sentencia condicional if
if (y > 5) {
  console.log('y es mayor que 5');
} else {
  console.log('y no es mayor que 5');
}

// Sentencia de bucle while
let i = 0;
while (i < 3) {
  console.log(i);
  i++;
}
```

Las declaraciones y sentencias son fundamentales para estructurar el flujo de control en un programa JavaScript.

# 17. Control de Flujo
## 17.1 Block, 17.2 Empty statement, ..., 17.8 try...catch

El control de flujo en JavaScript se logra a través de varias sentencias.

```javascript
// Bloque de código
{
  let a = 1;
  let b = 2;
  console.log(a + b);
}

// Sentencia vacía
;

// Sentencia break
for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break;
  }
  console.log(i);
}

// Sentencia continue
for (let i = 0; i < 5; i++) {
  if (i === 2) {
    continue;
  }
  console.log(i);
}

// Sentencia if...else
let condition = true;
if (condition) {
  console.log('La condición es verdadera');
} else {
  console.log('La condición es falsa');
}

// Sentencia switch
let day = 3;
switch (day) {
  case 1:
    console.log('Lunes');
    break;
  case 2:
    console.log('Martes');
    break;
  default:
    console.log('Día no reconocido');
}

// Sentencia throw
function divide(x, y) {
  if (y === 0) {
    throw new Error('No se puede dividir por cero');
  }
  return x / y;
}

// Sentencia try...catch
try {
  console.log(divide(10, 0));
} catch (error) {
  console.error(error.message);
}
```

Estas sentencias controlan cómo fluye el programa y cómo manejar situaciones excepcionales.

# 18. Declaraciones
## 18.1 var, 18.2 let, 18.3 const

En JavaScript, las declaraciones de variables se realizan con `var`, `let` y `const`.

```javascript
// Declaración con var (evitar su uso)
var a = 10;

// Declaración con let (ámbito de bloque)
let b = 20;

// Declaración con const (constante, no puede ser reasignada)
const c = 30;
```

El uso de `let` y `const` es preferible a `var` para evitar problemas relacionados con el ámbito y la reasignación no deseada.

# 19. Funciones y Clases
## 19.1 function, 19.2 function*, ..., 19.5 class

JavaScript admite varias formas de definir funciones y clases.

```javascript
// Declaración de función
function add(x, y) {
  return x + y;
}

// Expresión de función
let multiply = function(x, y) {
  return x * y;
};

// Función flecha
let divide = (x, y) => x / y;

// Función generadora
function* myGenerator() {
  yield 1;
  yield 2;
}

// Declaración de clase
class Rectangle {
  constructor(width, height) {
    this.width = width;
    this.height = height;
  }

  area() {
    return this.width * this.height;
  }
}

// Crear instancia de clase
let myRect = new Rectangle(5, 10);
console.log(myRect.area()); // Imprime 50
```
# 20. Iteraciones
## 20.1 do...while, 20.2 for, ..., 20.6 while

JavaScript ofrece varias formas de realizar iteraciones.

```javascript
// Bucle do...while
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 3);

// Bucle for
for (let j = 0; j < 3; j++) {
  console.log(j);
}

// Bucle for...in (itera sobre propiedades de un objeto)
let person = { name: 'John', age: 30 };
for (let key in person) {
  console.log(key, person[key]);
}

// Bucle for...of (itera sobre elementos de un iterable, como un array)
let colors = ['red', 'green', 'blue'];
for (let color of colors) {
  console.log(color);
}

// Bucle for await...of (para iterar sobre promesas)
async function asyncFunction() {
  let promises = [Promise.resolve(1), Promise.resolve(2), Promise.resolve(3)];
  for await (let result of promises) {
    console.log(result);
  }
}

// Bucle while
let k = 0;
while (k < 3) {
  console.log(k);
  k++;
}
```

Estas estructuras de bucle proporcionan flexibilidad para realizar iteraciones en diferentes situaciones.

# 21. Otros
## 21.1 debugger, 21.2 export, 21.3 import, ..., 21.5 with

JavaScript también incluye algunas construcciones especiales y palabras clave.

```javascript
// Declaración debugger (pausa la ejecución en el depurador)
function debugFunction() {
  let x = 10;
  debugger;
  console.log(x); // La ejecución se pausa aquí y se puede inspeccionar el estado
}

// Declaraciones de import/export (para modularización)
// Módulo 1 (export)
export const PI = 3.14;

// Módulo 2 (import)
import { PI } from './modulo1.js';
console.log(PI);

// Etiqueta de declaración (poco común y desaconsejada)
etiqueta: for (let i = 0; i < 5; i++) {
  if (i === 3) {
    break etiqueta; // Salta fuera del bucle etiquetado
  }
  console.log(i);
}

// Sentencia with (desaconsejada debido a problemas de rendimiento y mantenimiento)
let obj = { x: 10, y: 20 };
with (obj) {
  console.log(x + y); // Imprime 30
}
```

Estas construcciones son menos comunes o desaconsejadas en el código moderno de JavaScript, pero es útil conocerlas.

# 22. Operadores y Expresiones
## 22.1 Expresiones primarias, ..., 22.15 Operador coma

JavaScript utiliza varios operadores y expresiones para realizar operaciones.

```javascript
// Expresiones primarias
let x = 42; // Literal numérico
let str = 'Hola'; // Literal de cadena
let isTrue = true; // Literal booleano
let obj = { key: 'valor' }; // Literal de objeto

// Expresiones del lado izquierdo
let y;
y = 10;

// Operadores de incremento y decremento
let a = 5;
console.log(++a); // Incremento antes de la evaluación, imprime 6
console.log(a--); // Decremento después de la evaluación, imprime 6

// Operadores unarios
let negNumber = -10;

// Operadores aritméticos
let suma = 2 + 3;
let resta = 5 - 2;
let multiplicacion = 4 * 2;
let division = 8 / 4;
let modulo = 9 % 2;

// Operadores relacionales
console.log(5 > 3); // true
console.log('abc' === 'abc'); // true

// Operadores de igualdad
console.log(5 == '5'); // true (coerción de tipo)
console.log(5 === '5'); // false (sin coerción de tipo)

// Operadores de desplazamiento bit a bit
let binaryValue = 0b1010;
console.log(binaryValue << 1); // Desplazamiento a la izquierda, imprime 20

// Operadores binarios bitwise
let bitwiseAND = 5 & 3; // 0101 & 0011 = 0001 (1 en binario)
console.log(bitwiseAND); // Imprime 1

// Operadores lógicos bitwise
let logicalAND = true & false;
console.log(logicalAND); // Imprime false

// Operador condicional (ternario)
let age = 20;
let status = (age >= 18) ? 'Mayor de edad' : 'Menor de edad';

// Operadores de asignación
let z = 7;
z += 3; // Equivalente a z = z + 3
console.log(z); // Imprime 10

// Desestructuración de arrays y objetos
let [p, q] = [1, 2];
let { prop1, prop2 } = { prop1: 'a', prop2: 'b' };

// Operadores coma
let result = (1 + 2, 3 + 4); // La expresión a la derecha de la coma se evalúa, pero el resultado es el de la última expresión
console.log(result); // Imprime 7
```
# 23. Funciones
## 23.1 argumentos, 23.2 Funciones flecha, ..., 23.4 Parámetros rest

JavaScript ofrece diversas funcionalidades relacionadas con la definición y llamada de funciones.

```javascript
// El objeto arguments
function sum() {
  let result = 0;
  for (let i = 0; i < arguments.length; i++) {
    result += arguments[i];
  }
  return result;
}
console.log(sum(1, 2, 3)); // Imprime 6

// Funciones flecha
let add = (x, y) => x + y;

// Parámetros por defecto
function greet(name = 'Usuario') {
  console.log(`Hola, ${name}!`);
}
greet(); // Imprime 'Hola, Usuario!'
greet('John'); // Imprime 'Hola, John!'

// Parámetros rest
function concatenate(separator, ...strings) {
  return strings.join(separator);
}
console.log(concatenate('-', 'a', 'b', 'c')); // Imprime 'a-b-c'
```

# 24. Misceláneos
## 24.1 Gramática léxica, 24.2 Tipos de datos y estructuras, ..., 24.4 Características en desuso

JavaScript tiene algunas características y aspectos misceláneos a tener en cuenta.

```javascript
// Gramática léxica
let _variable = 'Variable con guión bajo';
let $variable = 'Variable con signo de dólar';

// Tipos de datos y estructuras
console.log(typeof 'Hola'); // Imprime 'string'
console.log(Array.isArray([1, 2, 3])); // true

// Modo estricto
'use strict';
// Habilita un conjunto más estricto de reglas y lanzará más errores en situaciones problemáticas

// Características en desuso
// Algunas características y funciones obsoletas están siendo eliminadas o ya no se recomiendan
```
