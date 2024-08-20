# ![logo javascript](./img/logo_javascript.png) _JavaScript_ con Jon Mircha ![logo javascript](./img/learning.png)

![logo javascript](./img/logo_javascript_1.png) es un lenguaje de programación versátil y popular que se utiliza principalmente para el desarrollo web. Permite a los desarrolladores agregar interactividad y funcionalidades dinámicas a las páginas web. Aquí están los puntos clave:

1. **Lenguaje de Script:** Originalmente diseñado para ejecutarse en el navegador web, permitiendo la manipulación del contenido HTML y la interacción con el usuario.

1. **Lenguaje Orientado a Objetos y Basado en Prototipos:** JavaScript soporta la programación orientada a objetos mediante prototipos, lo que significa que los objetos pueden heredar propiedades y métodos de otros objetos.

1. **Funciona en el Navegador y en el Servidor:** Aunque tradicionalmente se usa en el navegador, JavaScript también se puede ejecutar en el servidor mediante entornos como Node.js.

1. **Interactividad Web:** Permite crear elementos interactivos como formularios dinámicos, animaciones, y actualizaciones en tiempo real sin necesidad de recargar la página.

1. **Sintaxis Similar a C:** La sintaxis de JavaScript es similar a la de lenguajes como C, C++, y Java, lo que facilita el aprendizaje para quienes están familiarizados con esos lenguajes.

1. **Eventos y Manipulación del DOM:** JavaScript puede responder a eventos del usuario (como clics y desplazamientos) y manipular el Documento Object Model (DOM) para cambiar el contenido y la estructura de las páginas web.

1. **Evolución y Ecosistema:** JavaScript ha evolucionado con estándares modernos (ES6 y versiones posteriores) y tiene un amplio ecosistema de bibliotecas y frameworks como React, Angular, y Vue.js que facilitan el desarrollo de aplicaciones web complejas.

## Escritura de Código

### Identificadores

Son nombres que se le dan a las variables, funciones, o elementos como clases y objetos para poder referirse a ellos en el código y deben comenzar con:

```js
- Una leta: o, a, e
  var a = 2
- Un signo de dolar: $a
  var $a = 5
- Un guión bajo: _
  var _a = 8
- variable que inicia con la letra n y se le asgina el nombre numero:
  var numero = 125
- Nunca con números ni caracteres especiales o palabras reservadas
```

Si se emplean numeros, caracteres especiales o palabras reservadas (como `let, function, etc`), JavaScript nos mostrará un error de sintáxis.

```js
var -a = 8 // SyntaxError: Unexpected token '-'
```

En este caso nos da un error de sintáxis, dado que se uso un caracter especial (**`-`**).

---

### Para nombrar los **_Archivos_**:

- usa **snake_case**: `mi_archivo_javascript.js`

---

### Para nombrar las **_Constantes_**:

- usa **UPPER_CASE**:

```js
const UNA_CONSTANTE = "Soy una constante";

PI = 3.1415926;
```

**Nota:** El identificador se escribe todo en mayúscula y si tiene más de dos palabras se separan con guión bajo.

---

### Para nombrar las **_Clases_**:

- Usa **UpperCamelCase**:

```js
class SerHumano { = (nombre, genero) {
  this.nombre = nombre;
  this.genero = genero;
  }

  miNombreEs () {
    return `Mi nombre es ${this.nombre}`;
  }

}
```

**Nota:** En este caso el identificador debe llevar la primera letra de cada palabra en mayúscula.

---

### Usa **lowerCamelCase**:

- Para nombrar un **_Objeto_**:

```js
const unObjeto = {
  nombre: "Jonathan",
  email: "jonmircha@gmail.com",
};
```

- Para nombrar valores **_Primitivos_**:

```js
let unaCadena = "Hola Mundo";
(unNumero = 19), (unBoolean = true);
```

- Para nombrar **_Funciones_**:

```js
function Hola Mundo(nombre) {
  alert('Hola mundo ${nombre}');
}
  holaMundo("Jonathan");
```

- Para nombrar **_Instancias_**:

```js
const ajax = new XHLHttpRequest(),
  jon = new SerHumano("Jonathan", "Hombre");
```

**Nota** : En el caso que el identificador sea una sola palabra, esta inicia en minúscula, en el caso que este compuesta por más de dos palabras, estas deben llevar la primera letra de la primera palabra en minúscula y la primera letra de las demás palabras en mayúscula.

---

### _Palabras Reservadas_

```js
A: abstract
B: boolean, break, byte
C: case, catch, char, class, const, continue
D: debugger, default, delete, do, double
E: else, enum, export, extends
F: false, final, finally, float, for, function
G: goto
I: if, implements, import, in, instanceof, int, interface
L: let, long
N: native, new, null
P: package, private, protected, public
R: return
S: short, static, super, switch, synchronized
T: this, throw, throws, transient, true, try, typeof
V: var, volatile, void
W: while, with
```

**Nota**: JavaScript no permite el uso de palabras reservadas para los identificadores.

---

## Ordenamiento de Código

Recomendación para tener una buena estructura y organización de nuestro código.

1. **Importación de Módulos**
1. **Declaración de Variables**
1. **Declaración de Funciones**
1. **Ejecución de Código**

## Tipos de datos en _JavaScript_

**Primitivos**: Se accede directamente al valor.

- string
- number
- boolean
- null
- undefined
- Nan

**Compuestos**: Se accede a la referencia del valor.

- object ={}
- array =[]
- function () {}
- class {}
- etc

---

## **Objeto GLobal**

El objeto global en JavaScript es un objeto especial que está disponible en todo el entorno de ejecución y que actúa como un contenedor para todas las variables, funciones y objetos globales. Dependiendo del entorno en el que te encuentres (navegador, Node.js, etc.), el objeto global tiene diferentes nombres:

- **En un navegador**: El objeto global es `window`. Todo lo que declares en el ámbito global (fuera de cualquier función) se convierte en una propiedad del objeto `window`.
- En **Node.js**: El objeto global es `global`. Las variables y funciones globales se añaden como propiedades de `global`.

Por ejemplo, si declaras una variable global en un entorno de navegador:

```javascript
var miVariable = 42;
```

Esta variable se puede acceder también como:

```javascript
console.log(window.miVariable); // 42
```

El objeto global facilita el acceso y manipulación de recursos compartidos en todo el entorno de ejecución.

## Cadena de Caracteres (String)

En JavaScript, un String es una cadena de caracteres, es decir, una serie de letras, números o símbolos encerrados entre comillas. Las comillas pueden ser simples ('...'), dobles ("..."), o backticks (\`...`).

Ejemplos:

- 'Hola' es un String.
- "123" también es un String.
- \`Esto es un String` es otro ejemplo de String.

Los Strings se usan para representar texto y se pueden manipular con diversas funciones y métodos en JavaScript. Por ejemplo, puedes unir dos Strings con el operador +:

```js
let saludo = "Hola" + " Mundo"; // 'Hola Mundo'
```

Los objetos _**String**_ tienen propiedades y métodos:

1. Son caracteristicas que definen o describen algo relacionado con el objeto(brindan información del objeto). Se pueden leer, pero no modificar.

- _length_: Retorna el número de caracteres en el String.

```js
let texto = "Hola, mundo!";
console.log(texto.length); // 12
```

2. Los Métodos son funciones que se pueden ser llamadas para realizar diversas operaciones (acciones que el objeto hace). Los métodos terminan con parentesis.

- _charAt(index)_: Retorna el carácter en la posición especificada por index.

```js
let texto = "Hola, mundo!";
console.log(texto.charAt(3)); // "a"
```

## Template String

Un template string (o template literal) es una característica de JavaScript que permite crear cadenas de texto más flexibles y fáciles de leer, especialmente cuando necesitas incluir variables o expresiones dentro de la cadena.

_Características de los Template Strings_

1. _Comillas Invertidas_: Se crean utilizando comillas invertidas
   `` en lugar de comillas simples o dobles.

1. _Interpolación de Variables_: Puedes insertar variables y expresiones directamente en el string usando la sintaxis ${}.

1. _Múltiples Líneas_: Permiten escribir strings que abarcan múltiples líneas sin necesidad de concatenación.

Ejemplos

**Interpolación de Variables**

En lugar de concatenar variables con el operador +, los template strings te permiten incluirlas directamente dentro de la cadena.

```js
let nombre = "Juan";
let edad = 30;

let mensaje = `Hola, mi nombre es ${nombre} y tengo ${edad} años.`;
console.log(mensaje); // "Hola, mi nombre es Juan y tengo 30 años."
```

**Expresiones**

Puedes realizar cálculos u otras expresiones directamente dentro de ${}.

```js
let a = 5;
let b = 10;

let resultado = `La suma de 5 y 10 es ${a + b}.`;
console.log(resultado); // "La suma de 5 y 10 es 15."
```

**Múltiples Líneas**

Los template strings permiten escribir texto en varias líneas sin necesidad de usar caracteres especiales como \n.

```js
let textoLargo = `Este es un texto
que abarca múltiples
líneas.`;
console.log(textoLargo);
```

Este código generará:

```js
Este es un texto
que abarca múltiples
líneas.
```

**Ventajas de los Template Strings**

- **Legibilidad**: Al usar template strings, el código se vuelve más limpio y fácil de leer, especialmente cuando se combinan múltiples variables o se crean strings largos.

- **Flexibilidad**: Te permite incluir expresiones complejas dentro de un string sin necesidad de concatenar varias partes.

Los template strings son una poderosa herramienta en JavaScript que simplifica la creación y manipulación de cadenas de texto. ¡Son especialmente útiles para construir mensajes dinámicos o para trabajar con HTML en JavaScript!

## Números (Numbers)

### Booleans

### Null, Undefined, NaN

**_Null_**: Valor primitivo que representa una variable que no tiene valor. Pero es un valor dado intencionalmente por el programador, para indicar que una variable no se le ha asignado un valor.

```js
let nulo = null;
console.log(nulo);
```

**_Undefined_**: Es un valor primitivo que indica que una variable ha sido declarada pero no ha sido inicializada con ningún valor. Es un valor asignado por JavaScript, cuando detecta que una variable no tiene valor.

```js
let indefinida;
console.log(indefinida);
```

**_NaN (Not a Number)_**: Es un valor especial que representa el resultado de una operación matemática la cuál no se da mediante números válidos

```js
let noEsUnNumero = "hola" * 3.7;
console.log(noEsUnNumero);
```

---

### Funciones

Una **_función_** es un bloque de código, autocontenido, que se puede definir una vez y ejecutar en cualquier momento, con el fin de realizar una tarea especifica.

Opcionalmente, una función puede aceptar parámetros y devolver un valor.

Las funciones en JavaScript son objetos, un tipo especial de objeto

Se dice que las funciones son ciudadanos de primera clase porque pueden asignarse a un valor, y pueden pasarse como argumentos y usarse como un valor de retorno.

Ejemplo:

```js
function saludar() {
  console.log("¡Hola, Mundo!");
}

saludar(); // Llama a la función para que se ejecute y muestre "¡Hola, Mundo!" en la consola.
```

En este ejemplo:

**_function saludar()_** define una función llamada saludar.
El código entre las llaves _**{}**_ es lo que hace la función.
_**saludar()**_; es cómo llamas a la función para que haga su trabajo.

Las funciones son muy útiles para organizar y reutilizar código en tus programas.

---

**Nota**:

Información adaptada para fines educativos mediante la creación de un resumen personal, el cual esta basado en las siguientes fuentes:

- https://jonmircha.com/cursos
- https://jonmircha.com/javascript
- https://aprendejavascript.org/
- https://github.com/jonmircha/youtube-js
- https://www.youtube.com/playlist?list=PLvq-jIkSeTUZ6QgYYO3MwG9EMqC-KoLXA
- https://chatgpt.com/
- https://developer.mozilla.org/en-US/
