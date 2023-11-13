[](#1-objetos-globales)1\. Objetos Globales
===========================================

[](#11-objetos-globales-en-javascript)1.1 Objetos globales en JavaScript
------------------------------------------------------------------------

En JavaScript, los objetos globales son aquellos que están disponibles en todo el entorno de ejecución y no están vinculados a un objeto específico. Algunos de los objetos globales comunes incluyen `window` en el contexto del navegador y `global` en el contexto de Node.js.

[](#12-métodos-y-propiedades-de-objetos-globales)1.2 Métodos y propiedades de objetos globales
----------------------------------------------------------------------------------------------

Los objetos globales también tienen métodos y propiedades integrados que se pueden utilizar en cualquier parte del código. Algunos ejemplos son `setTimeout`, `setInterval`, y `console`.

Continuaré con el siguiente tema:

[](#2-propiedades-de-tipo-valor)2\. Propiedades de Tipo Valor
=============================================================

[](#21-globalthis)2.1 globalThis
--------------------------------

El objeto `globalThis` es una referencia al objeto global, independientemente del entorno en el que se esté ejecutando el código (navegador, Node.js, etc.). Es una forma consistente de acceder al objeto global.

[](#22-infinity)2.2 Infinity
----------------------------

`Infinity` es un valor numérico que representa el infinito matemático.

[](#23-nan)2.3 NaN
------------------

`NaN` significa "Not a Number" y se utiliza para representar un valor no numérico que no es igual a ningún otro número, incluido a sí mismo.

[](#24-undefined)2.4 undefined
------------------------------

`undefined` es un valor primitivo que se asigna automáticamente a las variables que se han declarado pero no se les ha asignado un valor.

[](#3-propiedades-de-tipo-función)3\. Propiedades de Tipo Función
=================================================================

[](#31-eval)3.1 eval()
----------------------

La función `eval()` evalúa una cadena de texto como código JavaScript en tiempo de ejecución.

Es importante usar `eval()` con precaución, ya que puede introducir vulnerabilidades de seguridad si se utiliza con datos no confiables.

[](#32-isfinite)3.2 isFinite()
------------------------------

La función `isFinite()` verifica si un valor es finito (diferente de `Infinity` o `-Infinity`) y es un número. Devuelve `true` si es así, de lo contrario, devuelve `false`.

[](#33-isnan)3.3 isNaN()
------------------------

La función `isNaN()` verifica si un valor no es un número. Devuelve `true` si el valor no es un número, de lo contrario, devuelve `false`.

[](#34-parsefloat)3.4 parseFloat()
----------------------------------

La función `parseFloat()` analiza una cadena y devuelve un número de punto flotante.

[](#35-parseint)3.5 parseInt()
------------------------------

La función `parseInt()` analiza una cadena y devuelve un entero.

[](#36-decodeuri)3.6 decodeURI()
--------------------------------

La función `decodeURI()` decodifica un Identificador de Recursos Uniforme (URI) previamente codificado.

[](#37-decodeuricomponent)3.7 decodeURIComponent()
--------------------------------------------------

Similar a `decodeURI()`, pero se enfoca en decodificar componentes de un URI.

[](#38-encodeuri)3.8 encodeURI()
--------------------------------

La función `encodeURI()` codifica un URI.

[](#39-encodeuricomponent)3.9 encodeURIComponent()
--------------------------------------------------

Similar a `encodeURI()`, pero se enfoca en codificar componentes de un URI.

[](#4-objetos-fundamentales)4\. Objetos Fundamentales
=====================================================

[](#41-object)4.1 Object
------------------------

El objeto `Object` es la base de todos los objetos en JavaScript. Proporciona propiedades y métodos que son comunes a todos los objetos.

[](#42-function)4.2 Function
----------------------------

El objeto `Function` es una función predefinida en JavaScript que se puede utilizar para crear funciones.

[](#43-boolean)4.3 Boolean
--------------------------

El objeto `Boolean` es un objeto que envuelve un valor booleano.

[](#44-symbol)4.4 Symbol
------------------------

`Symbol` es un tipo de dato primitivo y también un constructor para objetos símbolo.

[](#5-objetos-de-errores)5\. Objetos de Errores
===============================================

[](#51-error)5.1 Error
----------------------

El objeto `Error` representa un error en tiempo de ejecución y se utiliza como base para otros objetos de error.

[](#52-evalerror)5.2 EvalError
------------------------------

El objeto `EvalError` indica un error con la función `eval()`.

[](#53-rangeerror)5.3 RangeError
--------------------------------

El objeto `RangeError` indica un error cuando un valor está fuera del rango permitido.

[](#54-referenceerror)5.4 ReferenceError
----------------------------------------

El objeto `ReferenceError` indica un error cuando se referencia a una variable no definida.

[](#55-syntaxerror)5.5 SyntaxError
----------------------------------

El objeto `SyntaxError` indica un error de sintaxis.

[](#56-typeerror)5.6 TypeError
------------------------------

El objeto `TypeError` indica un error cuando se produce una operación incompatible.

[](#57-urierror)5.7 URIError
----------------------------

El objeto `URIError` indica un error cuando se utiliza funciones relacionadas con URI.

[](#58-aggregateerror)5.8 AggregateError
----------------------------------------

El objeto `AggregateError` representa un error que agrupa varios errores en uno.

[](#6-números-y-fechas)6\. Números y Fechas
===========================================

[](#61-number)6.1 Number
------------------------

El objeto `Number` es un objeto global que permite trabajar con valores numéricos.

[](#62-bigint)6.2 BigInt
------------------------

El objeto `BigInt` permite representar números enteros arbitrariamente grandes.

[](#63-math)6.3 Math
--------------------

El objeto `Math` proporciona funciones y constantes matemáticas.

[](#64-date)6.4 Date
--------------------

El objeto `Date` permite trabajar con fechas y horas.

[](#7-procesamiento-de-texto)7\. Procesamiento de Texto
=======================================================

[](#71-string)7.1 String
------------------------

El objeto `String` representa una secuencia de caracteres y proporciona métodos para trabajar con texto.

[](#72-regexp)7.2 RegExp
------------------------

El objeto `RegExp` se utiliza para trabajar con expresiones regulares, que son patrones utilizados para realizar búsquedas y manipulación de texto.

[](#8-colecciones-indexadas)8\. Colecciones Indexadas
=====================================================

[](#81-array)8.1 Array
----------------------

El objeto `Array` representa una colección ordenada de elementos.

[](#82-int8array-83-uint8array--812-float64array)8.2 Int8Array, 8.3 Uint8Array, ..., 8.12 Float64Array
------------------------------------------------------------------------------------------------------

Estos son tipos de arrays tipados que permiten trabajar con datos binarios de manera más eficiente.

[](#813-bigint64array-814-biguint64array)8.13 BigInt64Array, 8.14 BigUint64Array
--------------------------------------------------------------------------------

Tipos de arrays tipados que trabajan con enteros grandes (BigInt).

[](#9-colecciones-con-campos-clave)9\. Colecciones con Campos Clave
===================================================================

[](#91-map)9.1 Map
------------------

El objeto `Map` es una colección de pares clave/valor donde las claves pueden ser de cualquier tipo.

[](#92-set)9.2 Set
------------------

El objeto `Set` es una colección de valores únicos.

[](#93-weakmap-y-94-weakset)9.3 WeakMap y 9.4 WeakSet
-----------------------------------------------------

Estas son variantes de `Map` y `Set` respectivamente, pero con algunas diferencias importantes. Los objetos en un `WeakMap` y los valores en un `WeakSet` pueden ser eliminados por el recolector de basura si no hay otras referencias a ellos.

[](#10-datos-estructurados)10\. Datos Estructurados
===================================================

[](#101-arraybuffer)10.1 ArrayBuffer
------------------------------------

El objeto `ArrayBuffer` es un contenedor de datos binarios de longitud fija.

[](#102-sharedarraybuffer)10.2 SharedArrayBuffer
------------------------------------------------

Similar a `ArrayBuffer`, pero diseñado para ser compartido entre hilos en un entorno de ejecución de múltiples hilos.

[](#103-dataview)10.3 DataView
------------------------------

El objeto `DataView` proporciona una interfaz para leer y escribir datos en un `ArrayBuffer`.

[](#104-atomics)10.4 Atomics
----------------------------

El objeto `Atomics` proporciona operaciones atómicas sobre arreglos `SharedArrayBuffer` que pueden ser compartidos entre hilos.

[](#105-json)10.5 JSON
----------------------

El objeto `JSON` proporciona métodos para trabajar con datos en formato JSON.

[](#11-gestión-de-memoria)11\. Gestión de Memoria
=================================================

[](#111-weakref)11.1 WeakRef
----------------------------

El objeto `WeakRef` permite crear referencias débiles a objetos, lo que significa que no impide que el recolector de basura recolecte el objeto.

[](#112-finalizationregistry)11.2 FinalizationRegistry
------------------------------------------------------

El objeto `FinalizationRegistry` permite realizar acciones cuando un objeto es recolectado por el recolector de basura.

[](#12-abstracción-de-control)12\. Abstracción de Control
=========================================================

[](#121-promise)12.1 Promise
----------------------------

El objeto `Promise` representa un valor que puede estar disponible ahora, en el futuro o nunca.

[](#122-generatorfunction-123-asyncgeneratorfunction)12.2 GeneratorFunction, 12.3 AsyncGeneratorFunction
--------------------------------------------------------------------------------------------------------

Las funciones generadoras (`GeneratorFunction`) y las funciones generadoras asíncronas (`AsyncGeneratorFunction`) permiten pausar y reanudar la ejecución, lo que es útil para escribir código asíncrono de manera más legible.

[](#124-generator-125-asyncgenerator-126-asyncfunction)12.4 Generator, 12.5 AsyncGenerator, 12.6 AsyncFunction
--------------------------------------------------------------------------------------------------------------

Estos son los tipos de instancias que se crean cuando se llama a un generador o una función asíncrona.

[](#13-reflexión)13\. Reflexión
===============================

[](#131-reflect)13.1 Reflect
----------------------------

El objeto `Reflect` proporciona métodos estáticos que son equivalentes a algunas operaciones realizadas en objetos.

[](#132-proxy)13.2 Proxy
------------------------

El objeto `Proxy` se utiliza para definir comportamientos personalizados para operaciones fundamentales (por ejemplo, lectura, escritura, enumeración) en un objeto.

Los objetos `Reflect` y `Proxy` son poderosos para la manipulación y observación de objetos en tiempo de ejecución.

[](#14-internacionalización)14\. Internacionalización
=====================================================

[](#141-intl-142-intlcollator--149-intlrelativetimeformat)14.1 Intl, 14.2 Intl.Collator, ..., 14.9 Intl.RelativeTimeFormat
--------------------------------------------------------------------------------------------------------------------------

El objeto `Intl` y sus subobjetos proporcionan soporte para internacionalización y localización de aplicaciones.

Esto es especialmente útil para aplicaciones que necesitan manejar formatos de números, fechas y texto en diferentes idiomas y regiones.

[](#15-webassembly)15\. WebAssembly
===================================

[](#151-webassembly-152-webassemblymodule--158-webassemblyruntimeerror)15.1 WebAssembly, 15.2 WebAssembly.Module, ..., 15.8 WebAssembly.RuntimeError
----------------------------------------------------------------------------------------------------------------------------------------------------

WebAssembly es un formato binario seguro y eficiente diseñado para ejecutarse en navegadores web, pero también puede ejecutarse fuera del navegador.

[](#16-sentencias)16\. Sentencias
=================================

[](#161-declaraciones-y-sentencias-en-javascript)16.1 Declaraciones y sentencias en JavaScript
----------------------------------------------------------------------------------------------

JavaScript utiliza declaraciones y sentencias para definir el comportamiento de un programa.

Las declaraciones y sentencias son fundamentales para estructurar el flujo de control en un programa JavaScript.

[](#17-control-de-flujo)17\. Control de Flujo
=============================================

[](#171-block-172-empty-statement--178-trycatch)17.1 Block, 17.2 Empty statement, ..., 17.8 try...catch
-------------------------------------------------------------------------------------------------------

El control de flujo en JavaScript se logra a través de varias sentencias.

Estas sentencias controlan cómo fluye el programa y cómo manejar situaciones excepcionales.

[](#18-declaraciones)18\. Declaraciones
=======================================

[](#181-var-182-let-183-const)18.1 var, 18.2 let, 18.3 const
------------------------------------------------------------

En JavaScript, las declaraciones de variables se realizan con `var`, `let` y `const`.

El uso de `let` y `const` es preferible a `var` para evitar problemas relacionados con el ámbito y la reasignación no deseada.

[](#19-funciones-y-clases)19\. Funciones y Clases
=================================================

[](#191-function-192-function--195-class)19.1 function, 19.2 function\*, ..., 19.5 class
----------------------------------------------------------------------------------------

JavaScript admite varias formas de definir funciones y clases.

[](#20-iteraciones)20\. Iteraciones
===================================

[](#201-dowhile-202-for--206-while)20.1 do...while, 20.2 for, ..., 20.6 while
-----------------------------------------------------------------------------

JavaScript ofrece varias formas de realizar iteraciones.

Estas estructuras de bucle proporcionan flexibilidad para realizar iteraciones en diferentes situaciones.

[](#21-otros)21\. Otros
=======================

[](#211-debugger-212-export-213-import--215-with)21.1 debugger, 21.2 export, 21.3 import, ..., 21.5 with
--------------------------------------------------------------------------------------------------------

JavaScript también incluye algunas construcciones especiales y palabras clave.

Estas construcciones son menos comunes o desaconsejadas en el código moderno de JavaScript, pero es útil conocerlas.

[](#22-operadores-y-expresiones)22\. Operadores y Expresiones
=============================================================

[](#221-expresiones-primarias--2215-operador-coma)22.1 Expresiones primarias, ..., 22.15 Operador coma
------------------------------------------------------------------------------------------------------

JavaScript utiliza varios operadores y expresiones para realizar operaciones.

[](#23-funciones)23\. Funciones
===============================

[](#231-argumentos-232-funciones-flecha--234-parámetros-rest)23.1 argumentos, 23.2 Funciones flecha, ..., 23.4 Parámetros rest
------------------------------------------------------------------------------------------------------------------------------

JavaScript ofrece diversas funcionalidades relacionadas con la definición y llamada de funciones.

[](#24-misceláneos)24\. Misceláneos
===================================

[](#241-gramática-léxica-242-tipos-de-datos-y-estructuras--244-características-en-desuso)24.1 Gramática léxica, 24.2 Tipos de datos y estructuras, ..., 24.4 Características en desuso
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

JavaScript tiene algunas características y aspectos misceláneos a tener en cuenta.