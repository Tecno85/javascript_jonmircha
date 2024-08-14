# ![logo javascript](./img/logo_javascript.png) _JavaScript_ con Jon Mircha ![logo javascript](./img/learning.png)

![logo javascript](./img/logo_javascript_3.png) es un lenguaje de programación versátil y popular que se utiliza principalmente para el desarrollo web. Permite a los desarrolladores agregar interactividad y funcionalidades dinámicas a las páginas web. Aquí están los puntos clave:

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

**Nota** : En el caso que el identificador sea una sola palabra, esta inicia en minúscula, en el caso que este compuesta por más de dos palabras, estas deben llevar la primera letra en mayúscula.

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

**Nota**:

Información adaptada para fines educativos mediante la creación de un resumen personal, el cual esta basado de las siguientes fuentes:

- https://jonmircha.com/cursos
- https://jonmircha.com/javascript
- https://aprendejavascript.org/
- https://github.com/jonmircha/youtube-js
- https://www.youtube.com/playlist?list=PLvq-jIkSeTUZ6QgYYO3MwG9EMqC-KoLXA
- https://chatgpt.com/

