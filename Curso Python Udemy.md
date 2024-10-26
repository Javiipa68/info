# Sintaxis y Semántica de Python

La descripción de un lenguaje de programación viene determinada por dos componentes principales, la **sintaxis** y la **semántica** del lenguaje.
* **Sintaxis**: La sintaxis de un lenguaje de programación es el conjunto de reglas que define las combinaciones de símbolos que se consideran declaraciones o expresiones válidas en ese lenguaje.
* **Semántica**: La semántica es el campo que se ocupa del estudio matemático riguroso del significado de los lenguajes de programación. Para ello, evalúa el significado de las cadenas sintácticamente válidas definidas por un lenguaje de programación específico.

### 1. Variables en Python

Una variable es un elemento de un lenguaje de programación que tiene asignado un valor determinado. Para crear una variable en Python se le debe proporcionar un nombre y asignarle un valor utilizando el símbolo `=`

El valor asignado a una variable puede cambiar a lo largo del programa escrito en Python

### 2. Asignación múltiple

Otra de las cosas que podemos hacer con las variables en Python es asignar una variable a otra variable diferente.

En el caso que se acaba de mostrar en las celdas anteriores, la variable `var` y `var2` apuntan a la misma cadena de texto `Hola mundo`

### 3. Sintaxis de las variables en Python

Tal y como se ha introducido en la primera sección, para definir variables en Python se debe cumplir con las reglas sintácticas definidas por el leguaje. A continuación se indican las reglas que debemos cumplir cuando definimos el nombre de una variable:

<div style="background-color:#D9EEFF;color:black;padding:2%;">
1. Los nombres de las variables en Python pueden tener cualquier longitud y pueden consistir en letras mayúsculas y minúsculas (A-Z, a-z), dígitos (0-9) y el carácter de subrayado (_)
</div>

Si no se cumple con estas reglas definidas en la sintaxis de Python, el intérprete de Python emitirá un error a la hora de ejecutar la sentencia

<div style="background-color:#D9EEFF;color:black;padding:2%;">
2. Aunque el nombre de una variable puede contener dígitos, el primer carácter de un nombre de variable no puede ser un dígito.
</div>

<div style="background-color:#D9EEFF;color:black;padding:2%;">
3. El nombre de las variables en Python es sensible a mayúsculas y minúsculas
</div>


# Strings

### 1. ¿Qué es un string?

Un **string** se corresponde con un conjunto de caracteres que forman una cadena de texto.

La sintaxis que debemos utilizar para definir strings en Python consiste en situar los caracteres entre `"` o `'`

La flexibilidad de definir string con el caracter `"` y el caracter `'` nos permite definir cadenas de texto que contienen esos mismos caracteres.

### 2. Indexación

En muchos tipos de datos en Python se puede acceder a elementos individuales de un conjunto ordenado de datos directamente mediante un índice numérico o un valor clave. Este proceso se denomina indexación.

En Python, las cadenas son secuencias ordenadas de caracteres, y por lo tanto pueden ser indexadas de esta manera. Se puede acceder a los caracteres individuales de una cadena especificando el nombre de la cadena seguido de un número entre corchetes `[]`.

El primer carácter de la cadena tiene el índice 0, el siguiente tiene el índice 1, y así sucesivamente. El índice del último carácter será la longitud de la cadena menos uno.

Tambien podemos utilizar números negativos para extraer caracteres por el final de la cadena de texto.


### 3. Slicing

Python también permite una sintaxis específica de indexación que extrae subcadenas de una cadena de texto, a esto se denomina **slicing**. 

La sintaxis que se utiliza para extraer una subcadena de una cadena `s` es de la forma `s[m:n]`, esto devuelve la porción de `s` que comienza en la posición `m`, y termina en la posición `n` (sin ser incluido el último caracter)

Si no indicamos uno de los números, lee hasta el final.


### 4. Stride

El stride es otra variante más del slicing. Si se añade un `:` adicional y un tercer índice, se designa una stride, que indica cuantos caracteres saltar hasta obtener el siguiente caracter.

Un string es un tipo de dato que Python considera **inmutable**, esto quiere decir que no podemos modificar una parte de un string asociada a una variable

A pesar de que no pueda modificarse el contenido de un string, si puede asignarse un string diferente a la variable.


### 6. Strings de múltiples líneas

En algunas ocasiones es posible que queramos definir un string que tenga múltiples líneas. Existen varias formas de definir esto en Python.

La forma más sencilla es introducir el caracter `\n` en la posición de la cadena de texto donde queremos que se produzca el salto de línea.

Otra opción interesante es situar nuestra cadena de texto entre los caracteres ```"""```.

### 7. F-Strings

# ¿Qué son f-Strings en Python?
En Python, una cadena de texto normalmente se escribe entre comillas dobles ("") o comillas simples (''). Para crear f-strings, solo tienes que agregar la letra f o F mayúscula antes de las comillas.

Por ejemplo, "esto" es una cadena de texto normal y f"esto" es una f-string.

# Como imprimir variables usando f-strings en Python
Si quieres mostrar variables utilizando f-strings, solo tienes especificar el nombre de las variables entre llaves {}. Y al ejecutar tu código, todos los nombres de las variables serán remplazados con sus respectivos valores.

En caso de tener multiples variables en tu cadena de texto, cada variable necesita llaves propias {}

Aquí puedes ver la sintaxis:

<div style="background-color:#D9EEFF;color:black;padding:2%;">
f"Esta es una f-string {nombre_var} y {nombre_var}."\
</div>


[Freecodecamp](https://www.freecodecamp.org/espanol/news/tutorial-de-f-strings-en-python-formato-de-cadenas-en-python-explicado-con-ejemplos/)


# Números

### 1. ¿Qué es un número en Python?

En Python existen tres tipos de datos numéricos: enteros (`int`), números de punto flotante (`float`) y números complejos.

### 2. Números enteros

De manera básica los números enteros son aquellos que no tienen parte decimal. En Python los números enteros se referencia con la palabra `int`.

Es importante diferencia entre un número entero y una cadena de texto que representa un número entero.

En Pthon puede convertirse una cadena de texto que representa un número entero en un valor numérico utilizando la función `int()`

Cuando escribimos un número grande, solemos utilizar diferentes símbolos para separar algunos dígitos de manera que sea más facil de leer. Por ejemplo el número 1000000 solemos representarlo como 1,000,000 o como 1.000.000.

En Python no puede añadirse el caracter `,` o `.` para separar los dígitos de un número grande, debe utilizarse el caracter `_`.

Una de las cosas sorprendentes sobre los números enteros en Python es que no hay límite en el tamaño de los números que podemos definir. Se pueden definir números enteros tan grandes como la memoria de tu sistema pueda soportar.

### Números de punto flotante

De manera básica, y en contraste con los número enteros, los número de punto flotante son aquellos que tienen una parte decimal. En Python los números de putno flotante se referencian con la palabra `float`.


De igual manera que con los números enteros, en Pthon puede convertirse una cadena de texto que representa un número de punto flotante en un valor numérico utilizando la función `float()`

Respecto a la sintaxis de los números de punto flotante, existen tres formas de representarlos en Python.

Al contrario que los números enteros, los número de punto flotante si tienen un tamaño máximo en Python. Aunque el tamaño máximo depende de tu sistema, cifras cercanas o superiores a `2e400` o lo que es lo mismo 2x10<sup>400</sup> suelen superar el tamaño máximo.

Cuando se alcanza el valor máximo, Python devuelve el valor especial `inf` haciendo referencia a infinito.


### Números complejos

Python es uno de los pocos lenguajes de programación que ofrece soporte integrado para los números complejos. Aunque los números complejos no suelen aparecer fuera de los dominios de la computación científica, pueden ser de mucha utilidad en dominios que utilicen técnicas estadísticas.

Un número complejo esta formado por dos componentes distintos: una parte real y una parte imaginaria. Para definir un número complejo en python, se define la parte real seguida de un símbolo `+` y la parte imaginaria terminando con la letra `j`.


# Comentarios

### 1. ¿Qué son los comentarios en Python?

Los comentarios son una parte fundamental de cualquier lenguaje de programación. Permiten describir partes del código que desarrollamos de manera que sea mucho más facil de comprender. Poner comentarios en nuestro código es una muy buena práctica que debemos seguir.

En Python existen diferentes tipos de comentarios que podemos utilizar para documentar nuestro código.

### 2. Comentarios básicos

La manera más básica de poner comentarios en Python es utilizando el símbolo `#`

También podemos poner comentarios después de alguna sentencia en Python

Los comentarios en Python deben ser cortos y transmitir información relevante para el desarrollador. No debe saturarse el código de un número muy elevado de comentarios que no transmiten información significativa.

### 3. Comentarios de varias líneas

En algunas ocasiones es posible que necesitemos poner comentarios de varias líneas. Python no permite crear un comentario de varias líneas utilizando el símbolo `#`.

La forma más sencilla de poner comentarios de varias líneas en Python, es comenzar cada una de las líneas con el símbolo `#`

Otra forma existente para definir comentarios de múltiples líneas en Python consiste en situar el texto entre `"""`. Como ya hemos comentado en secciones anteriores, esta construcción realmente esta creando un string de varias líneas.

Mientras que esto le da la funcionalidad de multilínea al comentario, debemos tener claro que no es técnicamente un comentario. Es una cadena que no está asignada a ninguna variable, por lo que será ignorada en tiempo de ejecución y no aparecerá en el bytecode de tu programa.

Sin embargo, debemos tener cuidado con el uso de este tipo de comentarios multilínea. Dependiendo de dónde se sitúen en nuestro programa, podrían convertirse en _docstrings_, que es un tipo de documentación que se asocian a una función o método.


# Funciones

### 1. ¿Qué es una función?

En matemáticas, una función es una relación o asignación entre una o más entradas y un conjunto de salidas. Una función se suele representar así:

`y = f(x)`

Todos los lenguajes de programación modernos implementan el concepto de función. Sin embargo, en programación, las funciones son construcciones mucho más genéricas y versátiles que en la definición matemática mostrada anteriormente. Una función va a consistir en un bloque de código que encapsula una tarea específica o un grupo de tareas relacionadas. Las funciones permiten dividir programas complejos en fragmentos más pequeños y modulares.

var = "Hola mundo" 

len(var)

len_var = len(var)

len_var

La función que se muestra anterioremente forma parte de un conjunto de funciones que estan definidas en el interprete de Python y podemos utilizar siempre que lo necesitemos.

Para utilizar estas funciones no necesitamos conocer el detalle del código fuente que la implementa, únicamente necesitamos conocer su interfaz:

* Qué argumentos recibe
* Qué valores devuelve

Cuando invocamos la función a través de su nombre y le proporcionamos los argumentos necesarios, el interprete de Python automáticamente recorre el código fuente que define esta función y ejecuta las tareas pertienentes sobre los argumentos proporcionados. Cuando la función termina, la ejecución vuelve a la línea de código donde se invocó la función. La función puede devolver un valor de retorno que podemos utilizar a lo largo de nuestro código.

len()


### 2. Definiendo funciones personalizadas

La sintaxis utilizada para definir funciones en Python es la siguiente:

```
def <nombre_funcion>([<parámetros>]):
    <sentencia(s)>
```

El último elemento, `<sentencia(s)>`, se denomina cuerpo de la función. El cuerpo es el bloque de sentencias en Python que se ejecutará cuando se llame a la función. El cuerpo de una función de Python se define por la sangría.

def mi_funcion(arg1, arg2):
    print(arg1)
    print(arg2)

La sintaxis utilizada para invocar una función es la siguiente: `<nombre_funcion>([<argumentos>])`

Los `<argumentos>` son los valores que se pasan a la función. Se corresponden con los `<parámetros>` en la definición de la función en Python. 

mi_funcion("Hola mundo", "Adios mundo")

print(1)
mi_funcion(2, 3)
print(4)

Se pueden definir funciones que no reciban ningún argumento, pero los paréntesis siguen siendo necesarios. Tanto una definición de función como una llamada a una función deben incluir siempre paréntesis, incluso si están vacíos.

def mi_funcion2():
    print("Hola mundo")

mi_funcion2()

### 3. Argumentos de las funciones

Los argumentos que le proporcionamos a una función en Python pueden ser de diferentes tipos.

#### 3.1 Argumentos posicionales

La forma más sencilla de pasar argumentos a una función en Python es con argumentos posicionales (también llamados argumentos requeridos). En la definición de la función, debe especificarse una lista de parámetros separada por comas dentro de los paréntesis.

def mi_funcion(arg1, arg2, arg3):
    print(arg1)
    print(arg2)
    print(arg3)

El número de argumentos que le proporcionamos en la invocación de la función debe respetar el orden y el número de parámetros definidos.

mi_funcion("Hola mundo", "Adios mundo", "Hola mundo")

mi_funcion("Hola mundo", "Adios mundo")

**Los parámetros se comportan como variables que estan definidas de manera local a la función (únicamente en el cuerpo de la función)**. Cuando se invoca la función, los argumentos que se le proporcionan se asignan a los parámetros en el orden en el que estuvieran definidos.

def mi_funcion():
    var = "variable 'var' dentro de la funcion"
    print(var)

var = "variable 'var' fuera de la funcion"
mi_funcion()
print(var)

#### 3.2. Argumentos de palabra clave

Otra forma de invocar una función en Python es indicando los argumentos de la forma `<palabra clave>=<valor>`. En ese caso, cada `<palabra clave>` debe coincidir con un parámetro en la definición de la función.

def mi_funcion(arg1, arg2):
    print(arg1)
    print(arg2)

var = "Hola mundo"
var2 = "Adios mundo"

mi_funcion(arg1=var, arg2=var2)

Utilizar argumentos de palabra clave, nos exime de tener que respetar el orden de los parámetros definidos en la función

mi_funcion(arg1=var, arg2=var2)

mi_funcion(arg2=var2, arg1=var)

Por otro lado, el número de argumentos debe seguir respetándose.

mi_funcion(arg1=var)

Una de las cosas interesantes que nos permite hacer Python, es combinar argumentos posicionales y de palabra clave en la misma llamada a una función. En estos casos, los argumentos posicionales deben indicarse primero.

mi_funcion(var, arg2=var2)

#### 3.3 Parámetros con valores por defecto u opcionales

Si especificamos un parámetro en la definición de una función en Python utilizando la forma `<nombre>=<valor>`, entonces `<valor>` se convierte en un valor por defecto para ese parámetro. 

Los parámetros definidos de esta manera se denominan parámetros por defecto u opcionales.

def mi_funcion(arg1, arg2="Valor por defecto"):
    print(arg1)
    print(arg2)

mi_funcion("Hola mundo")

mi_funcion("Hola mundo", "Adios mundo")

### 4. Sentencia Return

Las funciones en Python pueden retornar un valor despues de haber ejecutado las sentencias de código definidas. Para devolver un valor, se debe utilizar la palabra `return` dentro del cuerpo de la función.

Debemos de tener en cuenta varias cosas cuando utilizamos la palabra `return`:

<div style="background-color:#D9EEFF;color:black;padding:2%;">
1. Cuando se ejecuta esta sentencia en Python, el intérprete termina inmediatamente la ejecución de la función y regresa a la línea de código desde dónde la hubiésemos invocado.
</div>

def mi_funcion():
    print("Sentencia 1 en mi_funcion")
    return
    print("Sentencia 2 en mi_funcion")

print("Hola mundo")
mi_funcion()
print("Adios mundo")

<div style="background-color:#D9EEFF;color:black;padding:2%;">
2. Si indicamos definimos la palabra `return` de la siguiente forma `return <valor>` se retornará el `<valor>` especificado en la llamada a dicha función.
</div>

def mi_funcion():
    return "Valor de mi_funcion"

var = mi_funcion()

print(var)

mi_funcion()

mi_funcion()[0:5]

<div style="background-color:#D9EEFF;color:black;padding:2%;">
3. Si no indicamos el término `<valor>` en la sentencia `return` se devuelve un tipo de datos conocido como `None`
</div>

def mi_funcion():
    return

var = mi_funcion()

print(var)

<div style="background-color:#D9EEFF;color:black;padding:2%;">
4. Puede utilizarse la sentencia `return` para devolver varios valores utilizando la sintaxis `return <valor1>,<valor2>,...,<valorn>`
</div>

def mi_funcion():
    return "texto1","texto2","texto3"

var1,var2,var3 = mi_funcion()

print(var1)
print(var2)
print(var3)

### 5. Docstrings

Cuando la primera declaración en el cuerpo de una función en Python es un string de la forma `"""texto"""`, se conoce como docstring de la función. 

Los docstring se utilizan para proporcionar la documentación de una función. Puede contener el propósito de la función, los argumentos que toma, información sobre los valores de retorno, o cualquier otra información que se considere útil.

Existe un PEP (Python Enhancement Proporsal) que establece el estilo con el que deben definirse los docstrings: https://www.python.org/dev/peps/pep-0257/

`def mi_funcion():
    """Esto es un docstring de la función."""
    print("Hola mundo")


mi_funcion()

def mi_funcion2(arg1=0.0, arg2=0.0):
    """Esto es un docstring de varias líneas.

    Keyword arguments:
    arg1 -- primer argumento de la funcion (default 0.0)
    arg2 -- segundo argumento de la funcion (default 0.0)
    """
    return

mi_funcion2()`

<div style="background-color:#D9EEFF;color:black;padding:2%;">
5. Ejercicio

def generar_mensaje(nombre, mensaje="Bienvenido al curso de Python"):
    """Esta función genera un mensaje de 
    bienvenida al curso de Python
    """
    return f'¡Hola, {nombre}! {mensaje}'
    
var = generar_mensaje("Javier")

print (var)
</div>



# Funciones propias de Python

El intérprete de Python tiene una serie de funciones que están siempre disponibles. A continuación se enumeran en orden alfabético.

<table>
<colgroup>
<col style="width: 21%">
<col style="width: 18%">
<col style="width: 20%">
<col style="width: 20%">
<col style="width: 22%">
</colgroup>
<thead>
<tr><th></th>
<th></th>
<th><p>Built-in Functions</p></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr><td><p><code><span>abs()</span></code></p></td>
<td><p><code><span>delattr()</span></code></p></td>
<td><p><code><span>hash()</span></code></p></td>
<td><p><code><span>memoryview()</span></code></p></td>
<td><p><code><span>set()</span></code></p></td>
</tr>
<tr><td><p><code><span>all()</span></code></p></td>
<td><p><code><span>dict()</span></code></p></td>
<td><p><code><span>help()</span></code></p></td>
<td><p><code><span>min()</span></code></p></td>
<td><p><code><span>setattr()</span></code></p></td>
</tr>
<tr><td><p><code><span>any()</span></code></p></td>
<td><p><code><span>dir()</span></code></p></td>
<td><p><code><span>hex()</span></code></p></td>
<td><p><code><span>next()</span></code></p></td>
<td><p><code><span>slice()</span></code></p></td>
</tr>
<tr><td><p><code><span>ascii()</span></code></p></td>
<td><p><code><span>divmod()</span></code></p></td>
<td><p><code><span>id()</span></code></p></td>
<td><p><code><span>object()</span></code></p></td>
<td><p><code><span>sorted()</span></code></p></td>
</tr>
<tr><td><p><code><span>bin()</span></code></p></td>
<td><p><code><span>enumerate()</span></code></p></td>
<td><p><code><span>input()</span></code></p></td>
<td><p><code><span>oct()</span></code></p></td>
<td><p><code><span>staticmethod()</span></code></p></td>
</tr>
<tr><td><p><code><span>bool()</span></code></p></td>
<td><p><code><span>eval()</span></code></p></td>
<td><p><code><span>int()</span></code></p></td>
<td><p><code><span>open()</span></code></p></td>
<td><p><code><span>str()</span></code></p></td>
</tr>
<tr><td><p><code><span>breakpoint()</span></code></p></td>
<td><p><code><span>exec()</span></code></p></td>
<td><p><code><span>isinstance()</span></code></p></td>
<td><p><code><span>ord()</span></code></p></td>
<td><p><code><span>sum()</span></code></p></td>
</tr>
<tr><td><p><code><span>bytearray()</span></code></p></td>
<td><p><code><span>filter()</span></code></p></td>
<td><p><code><span>issubclass()</span></code></p></td>
<td><p><code><span>pow()</span></code></p></td>
<td><p><code><span>super()</span></code></p></td>
</tr>
<tr><td><p><code><span>bytes()</span></code></p></td>
<td><p><code><span>float()</span></code></p></td>
<td><p><code><span>iter()</span></code></p></td>
<td><p><code><span>print()</span></code></p></td>
<td><p><code><span>tuple()</span></code></p></td>
</tr>
<tr><td><p><code><span>callable()</span></code></p></td>
<td><p><code><span>format()</span></code></p></td>
<td><p><code><span>len()</span></code></p></td>
<td><p><code><span>property()</span></code></p></td>
<td><p><code><span>type()</span></code></p></td>
</tr>
<tr><td><p><code><span>chr()</span></code></p></td>
<td><p><code><span>frozenset()</span></code></p></td>
<td><p><code><span>list()</span></code></p></td>
<td><p><code><span>range()</span></code></p></td>
<td><p><code><span>vars()</span></code></p></td>
</tr>
<tr><td><p><code><span>classmethod()</span></code></p></td>
<td><p><code><span>getattr()</span></code></p></td>
<td><p><code><span>locals()</span></code></p></td>
<td><p><code><span>repr()</span></code></p></td>
<td><p><code><span>zip()</span></code></p></td>
</tr>
<tr><td><p><code><span>compile()</span></code></p></td>
<td><p><code><span>globals()</span></code></p></td>
<td><p><code><span>map()</span></code></p></td>
<td><p><code><span>reversed()</span></code></p></td>
<td><p><code><span>__import__()</span></code></p></td>
</tr>
<tr><td><p><code><span>complex()</span></code></p></td>
<td><p><code><span>hasattr()</span></code></p></td>
<td><p><code><span>max()</span></code></p></td>
<td><p><code><span>round()</span></code></p></td>
<td></td>
</tr>
</tbody>
</table>
<br>
<center>https://docs.python.org/3/library/functions.html</center>

### help()

Esta función se utiliza para mostrar la documentación de un objeto en Python.

help()

### print()

help(print)

print("Hola mundo")

print("Este es el número", 3)

print("Este es el número", 3, sep=":")

### str(), int(), float()

texto = "10" # string
num_int = 10 # int 
num_float = 10.6 # float

int(num_float)

int(texto)

str(num_int)

str(num_float)

### type()

Retorna el tipo del objeto que le proporcionamos como argumento.

type(10)

type("10")

type(10.5)

### id()

help(id)

var = "Hola mundo"

id(var)

Debemos tener en cuenta que el identificador hace referencia al objeto, en este caso al string, y no a la variable a la que esta asignado.

var2 = var

id(var2)

### exec()

help(exec)

var = "print('Hola mundo')"

exec(var)

# Zen of Python

- Lo disperso es mejor que lo denso.
- La legibilidad cuenta.
- Los casos especiales no son tan especiales como para romper las reglas.
- Aunque la practicidad gana a la pureza.
- Los errores nunca deben pasar en silencio.
- A menos que se silencien explícitamente.
- Ante la ambigüedad, rechaza la tentación de adivinar.
- Debe haber una -y preferiblemente sólo una- forma obvia de hacerlo.
- Aunque esa manera puede no ser obvia al principio, a menos que seas holandés.
- Ahora es mejor que nunca.
- Aunque a menudo "nunca" es mejor que "ahora mismo".
- Si la implementación es difícil de explicar, es una mala idea.
- Si la implementación es fácil de explicar, puede ser una buena idea.
- Los espacios de nombres son una gran idea: ¡hagamos más!



# Operadores Aritméticos

### 1. ¿Cuáles son los operadores aritméticos?

A continuación se presentan los operadores aritméticos soportados por Python 3

<table>
<thead>
<tr>
<th>Operator</th>
<th>Example</th>
<th>Meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>+</code>&nbsp;(unario)</td>
<td><code>+a</code></td>
<td><strong>Unario Positivo</strong></td>
</tr>
<tr>
<td><code>+</code>&nbsp;(binario)</td>
<td><code>a + b</code></td>
<td><strong>Suma</strong></td>
</tr>
<tr>
<td><code>-</code>&nbsp;(unario)</td>
<td><code>-a</code></td>
<td><strong>Unario Negativo</strong></td>
</tr>
<tr>
<td><code>-</code>&nbsp;(binario)</td>
<td><code>a - b</code></td>
<td><strong>Resta</strong></td>
</tr>
<tr>
<td><code>*</code></td>
<td><code>a * b</code></td>
<td><strong>Multiplicación</strong></td>
</tr>
<tr>
<td><code>/</code></td>
<td><code>a / b</code></td>
<td><strong>División</strong></td>
</tr>
<tr>
<td><code>%</code></td>
<td><code>a % b</code></td>
<td><strong>Módulo</strong></td>
</tr>
<tr>
<td><code>//</code></td>
<td><code>a // b</code></td>
<td><strong>División de enteros</strong> (también denominado <strong>Floor Division</strong>)</td>
</tr>
<tr>
<td><code>**</code></td>
<td><code>a ** b</code></td>
<td><strong>Exponencial</strong></td>
</tr>
</tbody>
</table>

### 2. Operadores Unarios

Los operadores unarios se caracterizan porque se aplican sobre un único operando. En Python se soportan el operador **Unario Positivo** y **Unario Negativo**. Este tipo de operadores se aplican sobre tipos numéricos en Python.

num = 10

# Operador Unario Positivo
+num

# Operador Unario Negativo
-num

texto = "Hola mundo"

-texto

### 3. Suma y Resta

Los operadores **Suma** y **Resta** son operadores binarios que pueden aplicarse sobre distintos tipos de datos.

#### 3.1. Tipos de datos Numéricos

num1 = 10
num2 = 5

num1 + num2

num1 - num2

num2 - num1

num3 = 1.5
num4 = 0.5

num3 + num4

num3 - num4

#### 3.2. Strings

text1 = "Hola"
text2 = "mundo"

text1 + text2

text1 + " " + text2

text1 - text2

### 4. Multiplicación y División

Los operadores **Multiplicación** y **División** son operadores binarios que pueden aplicarse sobre distintos tipos de datos.

#### 4.1. Tipos de datos numéricos

num1 = 10
num2 = 5

num1 * num2

## IMPORTANTE: El resultado siempre es un float
num1 / num2

#### 4.2. Strings

text1 = "Hola"
text2 = "mundo"

text1 * text2

text1 / text2

text1 * 2

### 5. Módulo (Muestra el resto de una división).

El operador **Módulo** es un operador binario que devuelve el resto de una división entre tipos de datos numéricos.

num1 = 10
num2 = 7

num1 % num2

num2 % num1

num1 = 10.5
num2 = 7.2

num1 % num2

### 6. Exponencial

El operador **Exponencial** es un operador binario que se aplica sobre tipos de datos numéricos.

num1 = 10

num1 ** 2

num1 ** 3

text1 = "Hola mundo"

text1 ** 2

### 7. Floor Division

El operador **Floor Division** es un operador binario que se aplica sobre tipos de datos numéricos y devuelve la parte entera del resultado.

num1 = 10
num2 = 7

num1 / num2

num1 // num2

num1 = 13
num2 = 7

num1 / num2

num1 // num2


# Operadores de asignación

### ¿Cuáles son los operadores de asignación?

En secciones anteriores ya hemos presentado el operador de asignación que utilizabamos para asignar un valor a una variable, concretamente se corresponde con `=`.

Sin embargo, una de las cosas interesantes que nos proporciona Python es un mecanismo para combinar operadores aritméticos y operadores de asignación simplificando el código que escribimos. A la combinación de ambos operadores se les denomina **_Augmented Assignment_**.

<table>
<thead>
<tr>
<th>Augmented<br>Assignment</th>
<th></th>
<th>Standard<br>Assignment</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>a += 5</code></td>
<td>es equivalente a</td>
<td><code>a = a + 5</code></td>
</tr>
<tr>
<td><code>a /= 10</code></td>
<td>es equivalente a</td>
<td><code>a = a / 10</code></td>
</tr>
<tr>
<td><code>a *= b</code></td>
<td>es equivalente a</td>
<td><code>a = a * b</code></td>
</tr>
</tbody>
</table>

# Booleanos

### 1. ¿Qué son los Booleanos?

Los booleanos se corresponden con uno de los tipos de datos más importantes de cualquier lenguaje de programación. Este tipo de dato se utiliza para representar la certeza de una expresión en Python.

Los tipos de datos Boolenos en Python se representan con el tipo `bool` y reciben únicamente dos posibles valores:
1. True
2. False

Una de las cosas interesantes a tener en cuenta es que las palabras `True` y `False` son palabras clave dentro de Python. Esto quiere decir que son palabras reservadas dentro del lenguaje de programación y no se les puede asignar ningún valor.

De manera intuitiva, este tipo de palabras se comportan como si fuesen un tipo de datos numérico o texto.


# Operadores de comparación

### ¿Cuáles son los operadores de comparación?

Los operadores de comparación evalúan la relación que existe entre dos valores en Python. Existen diferentes tipos de operadores de comparación.

<table>
<thead>
<tr>
<th>Operador</th>
<th>Ejemplo</th>
<th>Significado</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>==</code></td>
<td><code>a == b</code></td>
<td><strong>Igual a</strong></td>
</tr>
<tr>
<td><code>!=</code></td>
<td><code>a != b</code></td>
<td><strong>No igual a</strong></td>
</tr>
<tr>
<td><code>&lt;</code></td>
<td><code>a &lt; b</code></td>
<td><strong>Menor que</strong></td>
</tr>
<tr>
<td><code>&lt;=</code></td>
<td><code>a &lt;= b</code></td>
<td><strong>Menor que o igual a</strong></td>
</tr>
<tr>
<td><code>&gt;</code></td>
<td><code>a &gt; b</code></td>
<td><strong>Mayor que</strong></td>
</tr>
<tr>
<td><code>&gt;=</code></td>
<td><code>a &gt;= b</code></td>
<td><strong>Mayor que o igual a</strong></td>
</tr>
</tbody>
</table>

### 1. Igualdad y desigualdad

Los operadores de comparación más utilizados son el de igualdad `==` y el de desigualdad `!=`. Estos operadores pueden aplicarse a varios tipos de datos en Python.

#### 1.1. Tipos de datos numéricos

num1 = 2
num2 = 5

num1 == 2

num1 == num2

num1 == 2.0

num1 != 2

num1 != num2

#### 1.2. Strings

text1 = "cadena de texto"
text2 = "cadena de texto 2"

text1 == "cadena de texto"

text1 == text2

text1 != text2

### 2. Otros operadores de comparación

#### 2.1. Tipos de datos numéricos

num1 = 2
num2 = 5

num1 < num2

num2 < num1

num1 <= 2.0

#### 2.2. Strings

text1 = "Cadena de texto"

text1 < "texto"

**La comparación utiliza un orden lexicográfico: primero se comparan los dos primeros elementos, y si son diferentes, esto determina el resultado de la comparación; si son iguales, se comparan los dos siguientes elementos, y así sucesivamente, hasta que se agote cualquiera de las dos secuencias.**

Esto quiere decir que la comparación se realiza utilizando los equivalentes numéricos (el resultado de la función por defecto `ord()`) de sus caracteres.

help(ord)

ord('a')

"Cadena" < "Texto"

ord('C')

ord('T')

help(chr)

chr(67)

chr(84)


# Operadores de identidad

### ¿Cuáles son los operadores de identidad?

Los operadores de identidad se utilizan para comparar objetos. Sin embargo, no comparan si los objetos son iguales, en su lugar, comparan si son el mismo objeto:

<table>
<thead>
<tr>
<th>Operador</th>
<th>Ejemplo</th>
<th>Significado</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>is</code></td>
<td><code>x is y</code></td>
<td><code>True</code> si las dos variables <br>son el mismo objeto</td>
</tr>
<tr>
<td><code>is not</code></td>
<td><code>x is not y</code></td>
<td><code>True</code> si las dos variables <br>no son el mismo objeto</td>
</tr>
</tbody>
</table>

text1 = "Hola mundo"
text2 = "Hola mundo"

help(id)

id(text1)

id(text2)

text1 is text2	False

text1 == text2	True

text1 is not text2	True

text3 = text1

text3 is text1	True

# Operadores lógicos

### 1. ¿Cuáles son los operadores lógicos?

Los operadores lógicos modifican y unen expresiones evaluadas en contexto booleano para crear condiciones más complejas.

<table>
<thead>
<tr>
<th>Operador</th>
<th>Ejemplo</th>
<th>Significado</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>not</code></td>
<td><code>not x</code></td>
<td><code>True</code> if <code>x</code> is <code>False</code><br><code>False</code> if <code>x</code> is <code>True</code></td>
</tr>
<tr>
<td><code>or</code></td>
<td><code>x or y</code></td>
<td><code>True</code> if either <code>x</code> or <code>y</code> is <code>True</code><br><code>False</code> otherwise</td>
</tr>
<tr>
<td><code>and</code></td>
<td><code>x and y</code></td>
<td><code>True</code> if both <code>x</code> and <code>y</code> are <code>True</code><br><code>False</code> otherwise</td>
</tr>
</tbody>
</table>

### 2. Operador `not`

num = 5

num < 10	True

not num < 10	False

### 3. Operador `or`

num1 = 5
num2 = 10

num1 < 4	False

num1 < 4 or num2 > 5	True

### 4. Operador `and`

num1 = 5
num2 = 10

num1 < 4 and num2 > 5	False

num1 < 10 and num2 > 3	True



# Listas

### 1. ¿Qué son las listas en Python?

Las listas son un tipo de dato complejo y particular del lenguaje de programación Python. Una lista se corresponde con una colección arbitraria de objetos. Las listas son similares a estructuras como los arrays en otros lenguajes de programación con la diferencia de que aportan una mayor flexibilidad.

Las listas en Python se representan con el tipo `list` y la sintaxis que se utiliza para definirlas consiste en indicar una lista de objetos separados entre comas y encerrados entre corchetes: `[obj1, obj2, ..., objn]`

lista = [1, 2, 3, 4, 5]

type(lista)

print(lista)

lista2 = ["texto1", "texto2", "texto3"]

type(lista2)

print(lista2)

### 2. Las listas respetan el orden

Una de las características importantes de las listas es que se corresponden con una colección ordenada de objetos. El orden en el que se especifican los elementos cuando se define una lista es relevante y se mantiene durante toda su vida.

lista1 = ['t1', 't2', 't3']

print(lista1)

print(lista1)

**Podemos utilizar los operadores vistos en el tema anterior para comparar listas**

lista2 = ['t2', 't1', 't3']

lista1 == lista2

lista1 in lista2

lista1 == ['t1', 't2', 't3']

lista1 is ['t1', 't2', 't3']

### 3. Las listas pueden contener objetos de diferentes tipos

Las listas puden contener una colección de objetos de diferentes tipos.

lista = [1, 2, "uno", "dos"]

print(lista)

Una cosa interesante es que una lista puede llegar a contener una función.

def func():
    print("Hola mundo")

func

lista = ["texto1", "texto2", func]

print(lista)

Los elementos de una lista no tienen que ser únicos. Puede repetirse el mismo elemento varias veces en la misma lista

lista = ["texto", "texto", "texto"]

print(lista)

### 3. Acceso a los elementos de una lista

Los elementos de una lista pueden ser accedidos utilizando el concepto y la sintaxis de la indexación que se presentó cuando hablamos de strings.

Todas las variaciones vistas en la sección de strings (indexing, slicing, stride) aplican a las listas.

#### Indexing

lista = ["text1", "text2", "text3", "text4", "text5"]

lista[0]

lista[-1]

#### Slicing

lista[2:4]

lista[:3]

lista[2:]

#### Stride

lista[0:4:2]

Una cosa interesante es que podemos utilizar el concepto de stride para darle la vuelta a una lista

lista

lista[::-1]

Una de las pocas construcciones sintácticas en cuanto a indexación que cambia entre los strings y las listas es `[:]`.

* Cuando utilizamos esta construcción sintáctica con un string, nos devuelve una referencia a ese mismo objeto:

texto = "Hola mundo"

texto[:]

texto[:] is texto	True

* Sin embargo, cuando lo utilizamos con una lista, nos devuelve una copia del objeto:

lista = [1, 2, 3, 4]

lista[:]

lista[:] is lista	

### 4. Operaciones con listas

Como comentaba anteriormente, las listas soportan muchos de los operadores y funciones de Python por defecto presentados en los temas anteriores.

lista1 = [1, 2, 3]
lista2 = [4, 5, 6]

lista1 + lista2

lista1 * 2

len(lista1)

min(lista1)

max(lista2)

[1, 2, 3] + 4

[1, 2, 3] + [4]

### 5. Las listas se pueden anidar

Tal y como se ha presentado anteriormente, una lista puede contener cualquier tipo de objeto. Esto incluye otra lista. Una lista puede contener sublistas, que a su vez pueden contener sublistas, y así hasta una profundidad arbitraria.

lista = [1, [2, [3, 4], 5], 6]

lista[0]

lista[1]

Para aceder a los elementos de una sublista utilizamos la sintaxis `[][]`

lista[1][0]

lista[1][1]

lista[1][1][0]

No hay límite en la cantidad de listas que podemos anidar, pueden ser tantas como soporte la memoria de nuestro sistema.

Es importante entender que los operadores aplicarán sobre la primera lista y no aplicarán de manera recursiva.

lista

[3, 4] in lista		False

lista[1]

[3, 4] in lista[1]

### 6. Las listas son mutables

Al contrario que lo que veíamos cuando hablabamos de strings, las listas son estructuras mutables. Esto quiere decir que podemos modificar los elementos que forman parate de ellas.

lista = ["texto1", "texto2", "texto3"]

lista[0]

lista[0] = "texto4"

lista

También podemos eliminar elementos de una lista

del lista[0]

lista

Podemos utilizar otros conceptos de indexación, como el slicing o el stride para modificar varios elementos de una lista

lista

lista += ["texto4", "texto5", "texto6"]

lista

lista[0:3]

lista[0:3] = [1, 2, 3]

lista

El número de elementos seleccionados no tiene que ser igual a los asignados

lista[0:3]

lista[0:3] = [1, 2]

lista

lista[2:2] = [3, 4, 5]

lista

lista[0:6] = []

lista


# Tuplas

### 1. ¿Qué son las tuplas en Python?

Las tupas son un tipo de dato complejo y particular del lenguaje de programación Python. Una tupla es un objeto idéntico a una lista excepto por las siguientes propiedades:

* 1. Al igual que las listas, definen una colección ordenada de objetos, sin embargo utilizan la sintaxis `(obj1, obj2, ..., objn)` en lugar de `[obj1, obj2, ..., objn]`

* 2. Las tuplas son inmutables
#%% md
Las tuplas se representan dentro de python con el tipo de dato `tuple`.

tupla = (1, 2, 3, 4, 5)

type(tupla)

print(tupla)

### 2. Funcionamiento de las tuplas

tupla = (1, 2, 3, "text1", "text2", "text3")

tupla

tupla[0:3]

tupla[2] = "text0"

### 3. ¿Cuándo utilizar una tupla en lugar de una lista?

Hay determinados casos de uso en los que puede ser recomendable utilizar una tupla en lugar de una lista:

* 1. La ejecución del programa es más rápida cuando se manipula una tupla que cuando se trata de una lista equivalente. (Esto probablemente no se note cuando la lista o tupla es pequeña).

* 2. Si los valores de la colección van a permanecer constantes durante la vida del programa, el uso de una tupla en lugar de una lista protege contra la modificación accidental.

* 3. Hay otro tipo de datos de Python que presentaremos próximamente llamado diccionario, que requiere como uno de sus componentes un valor inmutable. Una tupla puede ser utilizada para este propósito, mientras que una lista no puede serlo.

### 4. Tuplas y tipos de datos numéricos

Hay que tener cuidado si definimos una tupla con un único elemento de tipo numérico. Python puede llegar a interpretar los paréntesis como parte de la expresión matemática y definir un tipo numérico en lugar de una tupla.

tupla = (2)

tupla

type(tupla)

Para solucionar este problema se utiliza la sintaxis `(num,)`

tupla = (2,)

tupla

type(tupla)

### 5. Packing y Unpacking

En las secciones anteriores, hemos visto como una tupla con varios elementos puede asignarse a una única variable:

tupla = (1, 2, 3, 4)

Sin embargo, una tupla permite utilizar esta estructura "empaquetada" y "desempaquetarla" en varias variables de manera simultánea

num1, num2, num3, num4 = tupla

num1

num2

num3

num4

# El número de variables debe coincidir con el número de elementos de la tupla
num1, num2, num3 = tupla

Este mecanismo de "unpacking" es lo que utilizabamos en secciones anteriores para devolver varios elementos en una función

def func():
    return 5,6

func()

num1, num2 = func()

num1

num2

¿Por qué no se indican los paréntesis después de la sentencia `return`? Una curiosidad relativa a la sintaxis de las tuplas, es que no es necesario poner los paréntesis para definirlas.

tupla = 1, 3, 5

tupla

(1, 3, 5)



# Diccionarios

### 1. ¿Qué son los diccionarios en Python?

Los diccionarios son un tipo de dato complejo y particular del lenguaje de programación Python que se corresponden con una colección de elementos clave-valor. Cada elemento clave-valor asocia la clave con un valor determinado.

Los diccionarios se representan dentro de python con el tipo de dato `dict`. La sintaxis utilizada para definir diccionarios es la siguiente: `{key:value, key2:value2, ..., keyn:valuen}`

dic = {
    "Nombre":"Santiago",
    "Apellido":"Hernandez",
    "Pais":"España",
    "Ciudad":"Madrid"
}

type(dic)

print(dic)

# Otra forma de definir diccionarios con la funcion dict()
dic2 = dict(
    Nombre="Santiago",
    Apellido="Hernandez",
    Pais="España",
    Ciudad="Madrid"
)

print(dic2)

### 2. Acceso a los elementos de un diccionario

Al contrario que las listas o las tuplas, los diccionarios no se acceden utilizando un índice. Los valores se acceden utilizando el nombre de la clave entre corchetes `[]`.

dic = {
    "Nombre":"Santiago",
    "Apellido":"Hernandez",
    "Pais":"España",
    "Ciudad":"Madrid"
}

dic['Nombre']

dic['Pais']

dic['Edad']

dic[0]

Una de las cosas importantes que debemos tener en cuenta es que podemos utilizar cualquier objeto inmutable como clave de un diccionario, esto incluye números, strings, tuplas...

dic2 = {
    0: "cero",
    1: "uno",
    2: "dos",
    3: "tres"
}

dic2[0]

dic2[3]

dic3 = {
    ("uno", 1): "one",
    ("dos", 2): "two",
    ("tres", 3): "three"
}

dic3[("uno", 1)]

dic3["dos", 2]

### 3. Elementos de un diccionario

Los diccionarios son estructuras que **pueden ser modificadas** y que **no respetan el orden** de los elementos, esto es como consecuencia de que sus elementos no se acceden a través de un índice númerico que determina su posición sino a través de una clave.

dic = {
    "Nombre":"Santiago",
    "Apellido":"Hernandez",
    "Pais":"España",
    "Ciudad":"Madrid"
}

dic["Nombre"] = "Pedro"

dic["Apellido"] = "Ramos"

print(dic)

Una cosa interesante sobre los diccionarios es que podemos añadir nuevos elementos en la estructura cuando lo necesitemos.

print(dic)

dic["Edad"] = 30

print(dic)

Como podéis observar en el ejemplo anterior, los diccionarios permiten asignar diferentes tipos de datos a los valores que referencian las claves. Podemos asignar datos de cualquier tipo: números, strings, listas, tuplas... o incluso diccionarios.

dic2 = {
    "num":10,
    "str":"Hola mundo",
    "lista":[1, 2, 3, 4],
    "tupla":(1, 2, 3, 4),
    "dic":{"k1":"clave1", "k2":"clave2"}
}

dic2["str"]

dic2["lista"]

dic2["lista"][2]

dic2["dic"]

dic2["dic"]["k1"]

Las claves del diccionario tampoco tienen que se del mismo tipo de dato.

dic3 = {
    1:"primer valor",
    "dos":"segundo valor",
    ("tres",):"tercer valor"
}

dic3[1]

dic3["dos"]

dic3[("tres",)]

**La restricción más importante que debemos de tener en cuenta cuando utilizamos diccionarios, es que no puede haber dos claves con el mismo nombre**

dic4 = {
    "key":"value1",
    "key":"value2"
}

dic4

### 4. Operaciones con diccionarios

Al igual que con las listas y el resto de tipos de datos complejos, podemos utilizar algunos de los operadores presentados en el tema anterior con los diccionarios.

dic1 = {
    "key1": "value1",
    "key2": "value2"
}

dic2 = {
    "key3": "value3",
    "key4": "value4"
}

dic1 is dic2

dic1 == dic2

dic1 == dic1

dic1 is dic1

dic1 + dic2



# Bytes y Bytearray

### 1. ¿Qué son los bytes en Python?

Un byte es una ubicación de memoria con un tamaño de 8 bits. Un objeto bytes es una secuencia inmutable de bytes, conceptualmente similar a un string.

El objeto bytes es importante porque cualquier tipo de dato que se escribe en disco se escribe como una secuencia de bytes, los enteros o las cadenas de texto son secuencias de bytes. Lo que convierte la cadena de bytes en una cadena de texto o un número entero, es la forma en la que se interpreta.

Los bytes se representan dentro de python con el tipo de dato `bytes`. La sintaxis utilizada para definir bytes es la siguiente: `b'<cadena de bytes>'`

cadena_bytes = b'\x02\x1f'

type(cadena_bytes)

print(cadena_bytes)

bin(543)

type(bin(543))

# Hay que añadir el padding de ceros a la izquierda
# 00000010 | 00011111

hex(543)

num_bytes = b'\x02\x1f'

int.from_bytes(num_bytes, "big")

# Otra forma de definir cadenas de bytes con la funcion bytes()
cadena_bytes2 = bytes(3)

cadena_bytes2

### 2. Transformando tipos de datos en bytes

Una de las cosas que podemos hacer con el tipo de datos bytes es transformar otros tipos de datos, como cadenas de texto o número, a esta representación.

texto = "Hola mundo"

texto_bytes = b'Hola mundo'

texto_bytes

type(texto)

type(texto_bytes)

Como podemos observar en el caso anterior, aparentemente ambos tipos tienen la misma representación, esto es debido a que si la cadena de bytes puede interpretarse como caracteres ASCII imprimibles, lo saca por pantalla de esta forma. Tabla ASCII: https://ascii.cl/es/

# Estos bytes se interpretan como A, B y C en ASCII
b'\x41\x42\x43'

int("41", base=16)

b'\x20\x19\x61\x62\x39\x40'

bytes(1)

### 3. Acceso a los elementos de una cadena de bytes

El acceso a los elementos de una cadena de bytes es muy similar al acceso a los elementos de un string y respeta los conceptos de indexing, slicing y stride. Sin embargo, tiene algunas pecualiaridades a la hora de devolver los valores.

cadena_bytes = b'\x20\x19\x61\x62\x39\x40'

cadena_bytes[-1]

Como podemos observar, cuando indexamos un elemento de una cadena de bytes, se retorna este elemento interpretado como un `int`. Puedes comprobar la equivalencia en la tabla que se mostraba anteriormente: https://ascii.cl/es/

Por otro lado, podemos interpretar el entero como un valor hexadecimal utilizando la función pode defecto de Python `hex()`

hex(cadena_bytes[-1])

Utilizando slicing y stride, nos devuelve un tipo de dato `bytes`

cadena_bytes[-1:]

cadena_bytes[0::2]

Como veíamos en la introducción, los tipos de datos `bytes` son inmutables y por lo tanto no permiten la modificación de sus elementos.

cadena_bytes[0] = b'4'

### 4. Operaciones con bytes

Al igual que con otros tipos de datos, los bytes van a permitir el uso de varios de los operadores presentados en la sección anterior.

cad1 = b'\x20\x19\x61'
cad2 = b'\x62\x39\x40'

# Suma
cad1 + cad2

# Multiplicación
cad1 * 2

cad1 == cad2

cad1 != cad2

cad1 is cad2

cad1 is cad1

### 5. Bytearray

Este tipo de dato se correponde con una cadena de bytes, similar al tipo `bytes` con la diferencia fundamental de que es un tipo de dato mutable

La creación de este tipo de dato debe hacerse siempre a través de la función por defecto de Python `bytearray()`

cadena_bytes = bytearray(b'\x20\x19\x61\x62\x39\x40')

cadena_bytes

type(cadena_bytes)

#### 5.1. Acceso a los elementos de un bytearray

El acceso a los elementos de un objeto bytearray es igual que a un objeto bytes.

cadena_bytes[0]

cadena_bytes[0:4]

#### 5.2. Modificación de los elementos de un bytearray

La diferencia fundamental entre un objeto bytearray y bytes es que el primero permite modificar sus elementos

cadena_bytes

cadena_bytes[0:1] = b'8'

cadena_bytes

Si realizamos la asignación indexando un único elemento del bytearray, debemos proporcionar un valor de tipo `int`.

Podemos transformar un único carácter a su representación en ASCII como número entero utilizando la función por defecto de Python `ord()`

help(ord)

cadena_bytes

cadena_bytes[0]

ord('8')

cadena_bytes

cadena_bytes[2]

ord('a')

help(chr)

chr(97)

cadena_bytes[2] = ord('c')

cadena_bytes

#### 5.3. Operaciones con bytearray

Las operaciones que podemos realizar con bytearray son muy similares a las que se realizan con objetos bytes

cad1 = bytearray(b'\x20\x19\x61')
cad2 = bytearray(b'\x62\x39\x40')

cad1 + cad2		

cad1*2


# Sets

### 1. ¿Qué son los sets en Python?

Los sets son un tipo de datos en Python que permite almacenar múltiples elementos en una misma variable. A diferencia de las listas, la colección de elementos que forman un set: 
* 1. No se puede indexar
* 2. No respeta un orden
* 3. No puede contener valores duplicados

Los set se representan dentro de python con el tipo de dato `set`. La sintaxis que se utiliza para definir un set en Python es la siguiente: `{val1, val2, ..., valn}`

miset = {"rojo", "azul", "verde"}

print(miset)

type(miset)

### 2. Funcionamiento de un set

Debido a las características que presentea este tipo de dato, suele utilizarse para casos de uso muy específicos, como eliminar elementos duplicados de una lista o implementar algunas operaciones matemáticas como la intersección de dos conjuntos. Se utiliza para eliminar duplicados de una Lista o de una Tupla.

miset = {"rojo", "azul", "verde"}

# Los elementos de un set no se pueden indexar
miset[0]

lista = ["rojo", "rojo", "amarillo", "azul", "azul"]

set(lista)

lista_unicos = list(set(lista))

lista_unicos

### 3. Frozenset

Es un tipo de dato exactamente igual que un set, con la diferencia de que es inmutable.

fset = frozenset({"azul, amarillo, verde"})

fset

type(fset)



# NoneType

### 1. ¿Qué es el tipo de dato NoneType?

La palabra clave `None` se utiliza para definir una variable nula o un objeto vacío. En Python, la palabra clave `None` es un objeto de la clase `NoneType`.

Podemos asignar `None` a cualquier variable, pero no se pueden crear otros objetos `NoneType`.

var = None

var

print(var)

type(None)

### 2. Funcionamiento de None

Algunos aspectos importantes sobre `None` son:
* `None` no es lo mismo que `False`
* `None` no es 0
* `None` no es un string vacío
* Comparar `None` con cualquier cosa devuelve `False` excepto con `None`

var = None

var is None

var == None

var is False

var is True

var == False

var == 0

var == ""


# Sentencia `if/elif/else`

### 1. ¿Qué son las estructuras de control de flujo?

Todo lo que hemos visto hasta ahora han sido elementos de Python que se ejecutan de manera secuencial y exactamente en el orden especificado.

Sin embargo, con frecuencia un programa necesita cambiar el control del flujo de ejecución de las sentencias y realizar cosas como: saltarse algunas sentencias, ejecutar una serie de sentencias de forma repetitiva, o elegir entre conjuntos alternativos de sentencias a ejecutar.

Aquí es donde entran en juego las estructuras de control. Una estructura de control nos permite modificar el flujo de ejecución de un programa.

### 2. ¿Qué es la sentencia `if`?

La sentencia de control de flujo `if` es probablemente una de las estructuras más importantes de cualquier lenguaje de programación, incluido Python. 

**Esta estructura nos permite implementar sentencias condicionales dentro de nuestro programa.**

La sintaxis utilizada para definir la sentencia `if` es la siguiente:
```
if <expresión>:
    <sentencia(s)>
```
  
`<expresión>` es una expresión evaluada en un contexto booleano. El resultado de evaluar esta expresión debe ser `True` o `False`

`<sentencia(s)>` es el bloque de sentencias en Python que se ejecutará cuando el resultado de evaluar la expresión sea `True`, en caso contrario se omitirá.

num1 = 5
num2 = 10

# Esto sería una expresión
num1 < num2

if num1 < num2:
    print("Sentencia 1")
    print("Sentencia 2")
    print("Sentencia 3")

num1 = 15

if num1 < num2:
    print("Sentencia 1")
    print("Sentencia 2")
    print("Sentencia 3")

num1 < num2

<div style="background-color:#D9EEFF;color:black;padding:2%;">
IMPORTANTE: Recuerda que en Python todo el codigo que sea local a una estructura, por ejemplo una función o una estructura de control como `if`, debe esta "identado", es decir, respetar la sangría.
</div>

if num1 < num2:
    print("Sentencia 1")
    print("Sentencia 2")
    print("Sentencia 3")
print("Sentencia fuera del if")

### 3. ¿Qué expresiones y operadores podemos utilizar con la sentencia `if`?

Una de las cosas interesantes de esta sentencia de control de flujo es que podemos utilizar casi cualquier tipo de operador, tipo de dato y expresión siempre que el resultado sea un valor booleano (`True` o `False`)

lista = ["azul", "amarillo", "verde"]

if "azul" in lista:
    print("Sentencia 1 en if")
    print("Sentencia 2 en if")

tupla = (1, 2, 3, 4)

if 6 in tupla:
    print("Sentencia 1 en if")
    print("Sentencia 2 en if")

### 4. La cláusula `else`

En agunas ocasiones nos encontraremos con casos de uso en los que querremos una estructura condicional que ejecute unas sentencias en Python si la expresión es `True` pero además, que ejecute otras sentencias diferentes si la expresión es `False`. Para este tipo de casos se utiliza la cláusula `else`.

La sintaxis que debemos utilizar en Python 3 para definir la cláusula `else` dentro de una estructura `if` es la siguiente:

```
if <expresión>:
    <sentencia(s)>
else:
    <sentencia(s)>
```


num1 = 5
num2 = 10

if num1 < num2:
    print("Sentencias si True")
else:
    print("Sentencias si False")

if num1 > num2:
    print("Sentencias si True")
else:
    print("Sentencias si False")

### 5. La cláusula `elif`

Otros de los casos de uso que nos encontraremos con frecuencia es la implementación de una estructura condicional que requiera múltiples evaluaciones de varias expresiones para tomar la decisión de qué código ejecutar. Para estos casos específicos podemos utilizar la cláusula `elif`.

La sintaxis que debemos utilizar en Python 3 para definir la cláusula `elif` dentro de una estructura `if` es la siguiente:

```
if <expresión>:
    <sentencia(s)>
elif <expresión>:
    <sentencia(s)>
elif <expresión>:
    <sentencia(s)
...
else:
    <sentencia(s)>

```

Una cosa importante que debemos tener en cuenta es que podemos utilizar tantas cláusulas `elif` como consideremos oportunas.

nombres = ["Santiago", "Laura", "Julia"]

if "Pedro" in nombres:
    print("Hola Pedro")
elif "Juan" in nombres:
    print("Hola Juan")
elif "Marta" in nombres:
    print("Hola Marta")
elif "Santiago" in nombres:
    print("Hola Santiago")
else:
    print("El nombre no esta en la lista")

nombres = ["Laura", "Julia"]

if "Pedro" in nombres:
    print("Hola Pedro")
elif "Juan" in nombres:
    print("Hola Juan")
elif "Marta" in nombres:
    print("Hola Marta")
elif "Santiago" in nombres:
    print("Hola Santiago")
else:
    print("El nombre no esta en la lista")

### 6. Sentencia `if` en una sola línea

Como curiosidad interesante, Python 3 nos permite utilizar una sintaxis específica para implementar sentencias `if` en una sola línea de código. Sin embargo, en general esta opción no es muy recomendable debido a que puede aumentar la complejidad en la lectura del código fuente.

if 4 > 2: print("Sentencia 1");print("Sentencia 2");print("Sentencia 3")

if 4 < 2: print("Sentencia 1")
else: print("Sentencia 2")

### 7. Operador condicional

Por último, Python soporta una construcción más relacionada con la sentencia `if` que puede resultarnos muy interesante para determinados casos de uso. A esta construcción se le denomina operador condicional.

La sintaxis que se utiliza para implementar el operador condicional en Python3 es la siguiente:
```
<expresión1> if <expresión_condicional> else <expresión2>
```
Este operador nos permite simplificar el código que utilizamos para determinadas tareas como, por ejemplo, asignarle un valor a una variable en función de una condición.

nombre = "Pedro"

edad = 30 if nombre == "Pedro" else 15

edad

tiempo="lluvia"

print("Vamos", "a la piscina" if tiempo=="sol" else "al cine")

"al cine"

# Sentencias `break`, `continue` y `pass`

### 1. ¿Qué es la sentencia `break`?

La sentencia `break` es una palabra reservada del lenguaje Python que podemos utilizar para terminar de manera inmediata la ejecución de una estructura de control de flujo `for` o `while`. El flujo de ejecución del programa pasará a la siguiente línea de código que se encuentre fuera de la estructura de control flujo.

colores = ["rojo", "verde", "azul"]

for color in colores:
    print(color)

for color in colores:
    print(color)
    break

num = 5

while num > 0:
    print(num)
    num -= 1

num = 5

while num > 0:
    print(num)
    num -= 1
    break

Una de las cosas importantes que debemos tener en cuenta cuando estamos utilizando la sentencia `break` es que no se ejecutarán las líneas de código que pongamos en la claúsula `else`.

for color in colores:
    print(color)
    break
else:
    print("Ejecución en la claúsula else")

### 2. ¿Qué es la sentencia `continue`?

La sentencia `continue` es otra palabra reservada de Python sin embargo, a diferencia de la sentencia `break`, no termina la ejecución completa de los bucles `for` y `while` sino que termina únicamente la ejecución de la iteración actual.

colores = ["azul", "verde", "rojo"]

for color in colores:
    print(color)

for color in colores:
    if color == "verde":
        continue
    print(color)

num = 5

while num > 0:
    num -= 1
    if num == 2:
        continue    
    print(num)

### 3. ¿Qué es la sentencia `pass`?

La sentencia `pass` es una palabra reservada de Python que nos permite definir el esqueleto de diferentes estructuras de diferentes tipos (funciones, if, while, for...) sin indicarle ninguna línea de código en el cuerpo de la estructura.

def funcion():

def funcion():
    pass

colores = ["azul", "verde", "rojo"]

for color in colores:

    # Aqui voy a hacer algo que todavia no se

for color in colores:

    # Aqui voy a hacer algo que todavia no se

    pass

# Scope y Namespace

### 1. ¿Qué es el `Scope` y los `Namespaces` en Python 3?

Antes de hablar sobre clases, es importante que comprendamos los conceptos de `Scope` y `Namespace` en Python.

Un **`Namespace`** es un mapeo de nombres a objetos. Los `Namespaces` se crean en diferentes momentos y tienen diferentes tiempos de vida.

Durante la ejecución de un programa en Python 3 se crean diferentes `Namespaces` que pueden ser accesibles desde diferentes `scopes`:

* El **`Namespace` por defecto** que se crea cuando el intérprete de Python se inicia es el que contiene los nombres por defecto de Python. Este `Namespace` nunca se borra.

dir(__builtins__)

* El **`Namespace` global** para un módulo se crea cuando se lee la definición del módulo y, normalmente, dura hasta que el intérprete se cierra. 

var_modulo = 10
globals()

* El **`Namespace` local** para una función o cualquier otra estructura de Python se crea cuando se llama a la función, y se borra cuando la función termina. Las invocaciones recursivas tienen cada una su propio `Namespace`.

def func():
    var_local_func = 5
    var_local_func = 10
    print(locals())
func()

### 2. ¿Qué es el `scope` en Python 3?

El `scope` es una región de un programa en Python donde un `Namespace` es directamente accesible.

En Python existen diferentes `scopes` desde los que se puede acceder a los `Namespaces` con algunas particularidades que debemos tener en cuenta:

* **El `scope` local (o de función)** es el bloque de código o cuerpo de cualquier función o expresión en Python. Contiene los nombres que se definen dentro de la función. Estos nombres sólo serán visibles desde el código de la función. Se crea en la llamada a la función, no en la definición de la misma, por lo que habrá tantos `scopes` locales diferentes como llamadas a la función.

def func():
    var_local_func = 10
    print(var_local_func)
func()
La variable `var_local_func` definida en el Namespace local de la funcion no es accedida desde un scope global.

var_local_func

* **El `scope` no local** es un ámbito especial que sólo existe para las funciones anidadas. En estos casos el `scope` local es el cuerpo de la función anidada y el `scope` no local es el ámbito de la función externa. Los nombres del `scope` no local son visibles desde el código de las funciones internas y externas.

def func():
    var_no_local_func = 10
    def func2():
        var_local_func2 = 5
def func():
    var_no_local_func = 10
    print("Namespace func", locals())
    def func2():
        var_local_func2 = 5
        print("Namespace func2", locals())
    func2()
func()
La variable `var_no_local_func` es visible desde el código de `func2` pero la variable `var_local_func2` no es visible desde el código de `func`
def func():
    var_no_local_func = 10
    def func2():
        var_local_func2 = 5
        print(var_no_local_func)
    func2()
func()
def func():
    var_no_local_func = 10
    print(var_local_func2)
    def func2():
        var_local_func2 = 5
    func2()
func()

* **El `scope` global (o de módulo)** es el ámbito superior de un programa, script o módulo de Python. Este ámbito de Python contiene todos los nombres que se definen en el nivel superior de un programa o módulo. Los nombres en este ámbito de Python son visibles desde cualquier parte de tu código.

var_global = 15
print(var_global)
def func3():
    def func4():
        print(var_global)
    func4()
func3()
La variable `var_global` es accesible desde el código de `func` y cualquier otra función interna. Las variables definidas en `func` no son accesibles desde este scope.
def func():
    var_local_func = 10
var_local_func


* **El `scope` por defecto** es un ámbito especial de Python que se crea o carga cada vez que ejecutas un script o abres una sesión interactiva. Este ámbito contiene nombres como palabras clave, funciones, excepciones y otros atributos que están incorporados en Python. Los nombres en este ámbito de Python también están disponibles desde cualquier parte de tu código. Es cargado automáticamente por Python cuando ejecutas un programa o script.

# Scope global

True

# Scope no local

def func():
    True

# Scope local

def func():
    def func2():
        True
    func2()
func()

**Una de las cosas importantes es que los nombres que se encuentran en un scope determinado puede ser accedidos desde un scope externo pero no pueden ser actualizados o modificados**
contador = 0
def actualizar_contador():
    contador += 1
actualizar_contador()

### 3. Sentencias `global` y `nonlocal`

Teniendo en cuenta el comportamiento por defecto que hemos visto en los apartados anteriores, Python nos proporciona las dos sentencias `global` y `nonlocal` para modificarlo si lo necesitásemos.
contador = 0
def actualizar_contador():
    global contador
    contador += 1
actualizar_contador()
contador
def funcion():
    contador = 0
    def actualizar_contador():
        nonlocal contador
        contador += 1
    actualizar_contador()
    print(contador)
funcion()


# Clases en Python 3

### 1. ¿Qué es la Orientación a Objetos en Python 3?

La orientación a objetos es un paradigma de programación que proporciona unas estructuras denominadas objetos con el objetivo de estructurar los programas para que propiedades y comporatamientos similares se agrupen.

**Python es un lenguaje orientado a objetos y todas las estructuras que hemos visto en secciones previas son objetos.**

La programación orientada a objetos nos permite crear estruturas que representan cosas de la vida real a través de una construcción de que se donomina `clase` y después crear objetos basándonos en estas clases.

### 2. ¿Qué son las clases?

Las clases son la estructura principal de la programación orientada a objetos y nos proporcionan un medio para agrupar datos y funcionalidad. **Al crear una nueva clase se crea un nuevo tipo de dato, lo que permite crear nuevas instancias de ese tipo que se denominan objetos**. Cada instancia de clase puede tener atributos adjuntos para mantener su estado. Las instancias de clase también pueden tener métodos (definidos por su clase) para modificar su estado.

La sintaxis que se utiliza para definir clases en Python 3 es la siguiente:
```
class <nombre_clase>:
    <sentencia(s)>
```
class Coche:
    pass
Los nombres de las clases en Python siempre deben comenzar con una letra mayúscula. Aunque Python no fuerza que esto sea así a nivel sintáctico, es una convención muy importante.
class coche:
    pass

### 3. ¿Qué son los objetos?

Una vez que hemos definido una clase, podemos utilizarla para crear varios objetos pertenecientes a esa clase. La creación de un nuevo objeto a partir de una clase se denomina **instanciar**.

La sintaxis que utilizamos en Python 3 para instanciar un objeto es: 
```
<nombre_clase>([<argumentos>])
```
class Coche:
    pass
coche1 = Coche()
coche1
type(coche1)
id(coche1)
coche2 = Coche()
coche1 is coche2
id(coche2)
cadena1 = "Hola mundo"
cadena2 = "Adios mundo"
cadena1 is cadena2


# Métodos y Atributos

### 1. ¿Qué son los métodos?

La primera construcción que vamos a presentar que puede definirse dentro del cuerpo de la clase son las funciones. **Cuando una función forma parte de una clase se le denomina método**. 

Todo lo que hemos visto sobre las funciones se aplica también a los métodos, la única diferencia práctica por ahora es la forma en que se invocan los métodos. 
class Coche:
    def velocidad_maxima():
        """Este método devuelve la velocidad máxima del coche."""
        print("Velocidad máxima: ???")
coche1 = Coche()

### 2. Parámetro `self`

Cuando definimos métodos en una clase es necesario proporcionarles el parámetro `self`, que debe situarse en primer lugar antes de los otros parámetros. El parámetro `self` es una referencia a la propia clase, y se utiliza para poder acceder a diferentes componentes de la misma.
class Coche:
    def velocidad_maxima(self):
        """Este método devuelve la velocidad máxima del coche."""
        print("Velocidad máxima: ???")

### 3. Acceso a los métodos de una clase

Cuando instanciamos un objeto a partir de la clase, podemos acceder a los métodos con la siguiente sintáxis: 
```
<nombre_objeto>.<nombre_metodo>([<argumentos>])
```
class Coche:
    def velocidad_maxima(self):
        """Este método devuelve la velocidad máxima del coche."""
        print("Velocidad máxima: ??")
coche1 = Coche()
coche1.velocidad_maxima()

### 4. Atributos

Otra de las cosas que podemos definir en una clase son variables. **Cuando se define una variable dentro de una clase se denomina atributo**.

A la hora de definir atributos en una clase, podemos definirlos de dos tipos: **Atributos de clase** y **Atributos de instancia**.

* Un **atributo de clase** es una variable que pertenece a la clase y va a estar compartida entre todos los objetos que se instancien a partir de esa clase. Podemos acceder al valor de estos atributos con la sintaxis:
```
<nombre_objeto>.<nombre_atributo_clase>
```
class Coche:
    atributo_clase = 150
    
    def velocidad_maxima(self):
        """Este método devuelve la velocidad máxima del coche."""
        print("Velocidad máxima:", self.atributo_clase)
renault = Coche()
renault.velocidad_maxima()
renault.atributo_clase
bmw = Coche()
bmw.velocidad_maxima()
bmw.atributo_clase

* Un **atributo de instancia** es una variable que pertenece a un objeto en particular y que solo puede ser accedida en el contexto de ese objeto. Estas variables deben definirse en un método especial denominado constructor y representado por la sintaxis `__init__()`. Podemos acceder al valor de estos atributos con la sintaxis:
```
<nombre_objeto>.<nombre_atributo_instancia>
```
### 4. Método `__init__()`

El método `__init__()` es un método especial que Python ejecuta automáticamente cada vez que creamos una nueva instancia basada en esa clase. Este método tiene dos guiones bajos iniciales y dos guiones bajos finales, una convención que ayuda a evitar que los nombres de métodos por defecto de Python entren en conflicto con los definidos por el usuario.

El método `__init__()` se denomina constructor de la clase debido a que asigna valores específicos del objeto que se esta instanciando.
class Coche:
    
    def __init__(self, vel_max, consumo_medio):
        self.vel_max = vel_max
        self.con_medio = consumo_medio
    
    def velocidad_maxima(self):
        """Este método devuelve la velocidad máxima del coche."""
        print("Velocidad máxima:", self.vel_max)
        
    def consumo_medio(self):
        print("El consumo medio es:", self.con_medio)
renault = Coche(200, 7)
renault.velocidad_maxima()
renault.consumo_medio()
bmw = Coche(250, 10)
bmw.velocidad_maxima()
bmw.consumo_medio()
renault.velocidad_maxima()
bmw


# Trabajando con Clases y Objetos

### 1. Definiendo una clase

class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self.modelo = modelo
        self.potencia = potencia
        self.consumo = consumo
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self.modelo,
             "\nPotencia: {} cv".format(self.potencia),
             "\nConsumo: {} l/100km".format(self.consumo))
help(Coche)
mercedes = Coche("mercedes c200", 180, 7)
mercedes.especificaciones()

### 2. Atributos con valores por defecto

class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self.modelo = modelo
        self.potencia = potencia
        self.consumo = consumo
        self.km_actuales = 0
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self.modelo,
             "\nPotencia: {} cv".format(self.potencia),
             "\nConsumo: {} l/100km".format(self.consumo),
             "\nKilometros actuales:", self.km_actuales)
mercedes = Coche("mercedes c200", 180, 7)
mercedes.especificaciones()

### 3. Modificando los valores de los atributos de un objeto

La manera más sencilla de modificar el valor de un atributo de un objeto es utilizando la sintaxis: 
```
<objeto>.<atributo> = <nuevo_valor>
```
mercedes.km_actuales = -200
mercedes.especificaciones()
Por otro lado, existe una práctica mejor a la hora de modificar los atributos de la clase que consiste en hacerlo a través de un método especialmente creado para ello.

Esto nos permite realizar operaciones adicionales dentro de nuestro objeto siempre que se recibe un nuevo valor de un atributo.
class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self._modelo = modelo
        self._potencia = potencia
        self._consumo = consumo
        self._km_actuales = 0
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self._modelo,
             "\nPotencia: {} cv".format(self._potencia),
             "\nConsumo: {} l/100km".format(self._consumo),
             "\nKilometros actuales:", self._km_actuales)
        
    def actualizar_kilometros(self, kilometros):
        """Actualiza los kilometros del coche."""
        if kilometros > self._km_actuales:
            self._km_actuales = kilometros
        else:
            print("ERROR: No se puede establecer un numero de kilometros inferior al actual")
mercedes = Coche("mercedes c200", 180, 7)
mercedes.especificaciones()
mercedes.actualizar_kilometros(1000)
mercedes.especificaciones()
mercedes.actualizar_kilometros(10)

### 4. Extendiendo la funcionalidad de nuestra clase

class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self._modelo = modelo
        self._potencia = potencia
        self._consumo = consumo
        self._km_actuales = 0
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self._modelo,
             "\nPotencia: {} cv".format(self._potencia),
             "\nConsumo: {} l/100km".format(self._consumo),
             "\nKilometros actuales:", self._km_actuales)
        
    def actualizar_kilometros(self, kilometros):
        """Actualiza los kilometros del coche."""
        if kilometros > self._km_actuales:
            self._km_actuales = kilometros
        else:
            print("ERROR: No se puede establecer un numero de kilometros inferior al actual")
            
    def consumo_total(self):
        """Muestra el consumo total del coche desde el kilometro 0."""
        consumo_total = (self._km_actuales / 100) * self._consumo
        print("El consumo total es de {} litros".format(consumo_total))
mercedes = Coche("mercedes c200", 180, 7)
mercedes.consumo_total()
mercedes.especificaciones()
mercedes.actualizar_kilometros(100)
mercedes.consumo_total()
mercedes.actualizar_kilometros(153_000)
mercedes.consumo_total()


# Decorators

### 1. Conceptos avanzados sobre funciones

En Python las funciones también se consideran objetos y como consecuencia de esto se pueden asignar a una variable, almacenarlas en estructuras de datos (listas, tuplas, diccionarios...) o incluso pasarlas como argumento de otras funciones.
def func():
    print("Hola mundo")
var = func
var()
def func2(funcion):
    funcion()
func2(func)

### 2. ¿Qué es un _decorator_?

Los _decorator_ envuelven una función, modificando su comportamiento realizando una combinación de todas las propiedades que hemos visto anteriormente.
def mi_funcion():
    print("Hola mundo!!")
def mi_decorator(func):
    def wrapper():
        print("Ejecucion antes de la llamada a la funcion")
        func()
        print("Ejecucion despues de la llamada a la funcion")
    return wrapper
mi_funcion_mod = mi_decorator(mi_funcion)
mi_funcion_mod()
Podemos utilizar _decorators_ para modificar el comportamiento de una función que programemos, por ejemplo, añadiendo condiciones que se evalúen antes de ejecutar la función ya existente que no queremos modificar.
def funcion():
    print("Hola mundo!!")
def mi_decorator(func):
    def wrapper():
        if var < 5:
            func()
        else:
            print("No se puede ejecutar la funcion")
    return wrapper
funcion = mi_decorator(funcion)
var = 2
funcion()
var = 10
funcion()

### 3. _Syntactic Sugar_

La sintaxis que hemos utilizado en el apartado anterior para definir el _decorator_ es bastante compleja, por ello, Python nos proporciona una alternativa mucho más sencilla.
def mi_decorator(func):
    def wrapper():
        print("Ejecucion antes de la llamada a la funcion")
        func()
        print("Ejecucion despues de la llamada a la funcion")
    return wrapper
@mi_decorator
def mi_function():
    print("Hola mundo!!")
mi_function()

### 4. _Decorators_ en las Clases

Una de las cosas interesantes sobre los _decorators_ es que Python nos proporciona varios definidos por defecto que podemos utilizar dentro de una clase.

Uno de los _decorators_ más interesantes que podemos utilizar es `@property`, que nos permite definir métodos en una clase para consultar y modificar un atributo interno.
class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self._modelo = modelo
        self._potencia = potencia
        self._consumo = consumo
        self._km_actuales = 0
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self._modelo,
             "\nPotencia: {} cv".format(self._potencia),
             "\nConsumo: {} l/100km".format(self._consumo),
             "\nKilometros actuales:", self._km_actuales)
        
    def actualizar_kilometros(self, kilometros):
        """Actualiza los kilometros del coche."""
        if kilometros > self._km_actuales:
            self._km_actuales = kilometros
        else:
            print("ERROR: No se puede establecer un numero de kilometros inferior al actual")
            
    def consumo_total(self):
        """Muestra el consumo total del coche desde el kilometro 0."""
        consumo_total = (self._km_actuales / 100) * self._consumo
        print("El consumo total es de {} litros".format(consumo_total))
class Coche():
    """Esta clase representa un coche."""
    
    def __init__(self, modelo, potencia, consumo):
        """Inicializa los atributos de instancia.
        
        Argumentos posicionales:
        modelo -- string que representa el modelo del coche
        potencia -- int que representa la potencia en cv
        conumo -- int que representa el consumo en l/100km
        """
        self._modelo = modelo
        self._potencia = potencia
        self._consumo = consumo
        self._km_actuales = 0
        
    def especificaciones(self):
        """Muestra las especicificaciones del coche."""
        print("Modelo:", self._modelo,
             "\nPotencia: {} cv".format(self._potencia),
             "\nConsumo: {} l/100km".format(self._consumo),
             "\nKilometros actuales:", self._km_actuales)
        
    @property
    def kilometros(self):
        return self._km_actuales
        
    @kilometros.setter
    def kilometros(self, kilometros):
        """Actualiza los kilometros del coche."""
        if kilometros > self._km_actuales:
            self._km_actuales = kilometros
        else:
            print("ERROR: No se puede establecer un numero de kilometros inferior al actual")
            
    def consumo_total(self):
        """Muestra el consumo total del coche desde el kilometro 0."""
        consumo_total = (self._km_actuales / 100) * self._consumo
        print("El consumo total es de {} litros".format(consumo_total))
bmw = Coche("bmw i3", 150, 6)
bmw.kilometros
bmw.kilometros = 500
bmw.especificaciones()
bmw.kilometros
bmw.kilometros = 200

# Trabajando con Strings

Como hemos visto en el tema anterior, todos los tipos de datos que definimos en Python son objetos, y como consecuencia de esto, tienen varios métodos y atributos interesantes que debemos conocer.
help(dir)
texto = "cadena de texto"
dir(texto)

### 1. Transformaciones entre letras mayúsculas y minúsculas

texto = "hOlA MuNdO"
texto.capitalize()
texto.lower()
texto.swapcase()
texto.title()
texto.upper()

### 2. Buscar y reemplazar 

texto = "aoo boo coo"

# Cuenta las veces que se repite una subcadena
texto.count('oo')

# Devuelve el índice donde se encuentra la subcadena
texto.find('boo')

# Busca la subcadena empezando por el final
texto.rfind('oo')

### 3. Clasificaciones de caracteres

texto1 = '123abc'
texto2 = '123$abc'

# Determina si todos son caracteres alfanumericos
texto1.isalnum()
texto2.isalnum()

# Determina si todos los caracteres son numeros
texto1.isdigit()
texto1[:3]
texto1[:3].isdigit()

### 4. String Formatting

texto = 'Hola mundo'
texto.center(20)
texto.ljust(20)
texto = "       hola       que        tal     "
print(texto)
texto.lstrip()
texto.rstrip()
texto.strip()
texto.replace(" ", "")
texto = "Hola"
texto.zfill(8)

# Concatena un string con un objeto iterable
",".join(["azul", "verde", "azul"])
"{}-{}-{}".format(3, "hola", [1, 2])

# Trabajando con Listas
Como hemos visto en el tema anterior, todos los tipos de datos que definimos en Python son objetos, y como consecuencia de esto, tienen varios métodos y atributos interesantes que debemos conocer.
lista = ['azul', 'rojo', 'verde']
dir(lista)

### 1. Modificando una lista
lista = ['rojo', 'azul', 'verde']
lista.append('amarillo')
lista
lista.extend(['morado', 'rojo', 'azul'])
lista
lista.remove('azul')
lista
lista.reverse()
lista
lista.pop()
lista
lista2 = lista.copy()
lista2
lista.clear()
lista

### 2. Accediendo a elementos de la lista
lista = ['azul', 'verde', 'rojo']
lista.index('azul')
lista.index('verde')
lista.extend(['azul', 'azul'])
lista
lista.count('azul')

# Módulos

### 1.  ¿Qué es la programación modular?
La programación modular se refiere al proceso de dividir una tarea de programación grande y difícil de manejar en subtareas o módulos separados, más pequeños y manejables. Los módulos individuales se irán uniendo posteriormente para crear un programa más grande.

La modularización del código en una aplicación grande tiene varias ventajas:

* **Simplicidad**: En lugar de centrarse en todo el problema, un módulo suele centrarse en una parte relativamente pequeña del problema. Si trabajas en un solo módulo, tendrás un dominio del problema más pequeño en el que centrarte. Esto hace que el desarrollo sea más fácil y menos propenso a errores.

* **Mantenimiento**: Los módulos se diseñan normalmente de manera que imponen límites lógicos entre los diferentes dominios del problema. Si los módulos se escriben de forma que se minimice la interdependencia, se reduce la probabilidad de que las modificaciones en un solo módulo tengan un impacto en otras partes del programa.

* **Reutilización**: La funcionalidad definida en un solo módulo puede ser fácilmente reutilizada (a través de una interfaz bien definida) por otras partes de la aplicación. Esto elimina la necesidad de duplicar el código.

* **Alcance**: Los módulos suelen definen un namespace (namespace global) separado, lo que ayuda a evitar colisiones entre nombres en diferentes áreas de un programa.

**Las funciones, las clases, los módulos y los paquetes son construcciones de Python que promueven la modularización del código.**

### 2. ¿Qué es un módulo?

Hay tres formas diferentes de definir un módulo en Python:

* Un módulo puede estar escrito en Python.
* Un módulo puede estar escrito en C y cargado dinámicamente en tiempo de ejecución.
* Un módulo puede estar incorporado por defecto en el intérprete.

En los tres casos se accede al contenido de un módulo de la misma manera: con la sentencia `import`.

El tipo de módulo más importante y utilizado un 99% de las veces es el escrito en Python, que será en el que nos centraremos en este tema.

Un módulo escrito en Python no es más que un archivo que contiene código en Python y una extensión `.py`. Esto es todo. No se requiere ningún tipo de sintaxis especial para definirlos.

# Este código vamos a ejecutarlo en PyCharm

cadena_texto = "Hola mundo"
lista = ["azul", "verde", "rojo"]

def funcion(arg):
    print(arg)
    
class Coche:
    pass

>>> import modulo
>>> print(modulo.cadena_texto)
>>> print(modulo.lista)
>>> modulo.funcion("Hola mundo")
>>> bmw = modulo.Coche()
Cuando el intérprete ejecuta la sentencia `import`, busca el `mimodulo.py` en una lista de directorios que obtiene a partir de las siguientes fuentes:

* El directorio desde el que se ejecutó el script o el directorio actual si el intérprete se está ejecutando de forma interactiva
* La lista de directorios contenida en la variable de entorno `PYTHONPATH`, si está configurada.
* Una lista de directorios dependiente de la instalación configurada en el momento de instalar Python

La ruta de búsqueda resultante es accesible en la variable de Python `sys.path`, que se obtiene de un módulo llamado sys:
import sys
sys.path
Por lo tanto, para asegurarnos de que el módulo es encontrado, se requiere que hagamos alguna de las siguientes acciones:

* **Guardar el `módulo.py` en el directorio donde se encuentra el script o en el directorio actual si estamos utilizando el interprete interactivo**
* Modificar la variable de entorno `PYTHONPATH` para que contenga el directorio donde se encuentra el módulo, o bien, guardar el módulo en uno de los directorios ya contenidos en esta variable
* Guardar el módulo en uno de los directorios dependientes de la instalación, a los que puede o no tener acceso de escritura, dependiendo del sistema operativo

### 3. Sentencia `import`

La sentencia `import` nos permite incluir un módulo dentro de nuestro programa actual y utilizar las estructuras que esten definidas en él.

La manera más sencilla de utilizar la sentencia `import` es la que se mostraba en el apartado anterior:
```
import <nombre_modulo>
```
Debemos tener en cuenta que utilizando esta sintaxis el contenido del módulo no es directamente accesible por nuestro programa. Esta sentencia incorpora el nombre del módulo en el namespace global del programa que lo esta importando, pero no incorpora el namespace del módulo dentro del actual.

Por esta razón, los objetos del módulo sólo son accesibles cuando se les antepone `<nombre_módulo>` al nombre del objeto.

>>> import modulo
>>> print(modulo.cadena_texto)

Para evitar tener que invocar todos los objetos definidos en el módulo utilizando el nombre del módulo, Python nos proporciona una sintaxis alternativa:
```
from <nombre_modulo> import <nombre(s)>
```
Esto nos permite importar cualquier objeto del módulo en el namespace del programa actual.

>>> from modulo import funcion
>>> funcion()

Podemos importar varios objetos separándolos entre `,`

>>> from modulo import funcion, Coche
>>> funcion()
>>> mercedes = Coche()

Incluso podemos llegar a importar todos los objetos que se encuentre en el módulo utilizando el carácter `*`
>>> from modulo.py import *

### 4. Alias

Una de las cosas interesantes que nos proporciona Python a nivel sintáctico cuando importamos elementos de un módulo es asignarles un alias. De esta manera, los objetos se almacenan en el namespace del programa con otro diferente al original. Para ello podemos utilizar la siguiente sintaxis:
```
import <nombre_modulo> as <nombre_alias>

from <nombre_modulo> import <nombre_objeto> as <nombre_alias>
```

>>> import modulo as mimodulo
>>> mimodulo.function()
>>> from modulo import function as func
>>> func()

# Paquetes

### 1. ¿Qué son los paquetes en Python?

Los paquetes permiten estructurar jerárquicamente los módulos que hemos definido(Agrupación de Módulos).

Para inicializar un directorio dentro de nuestro sistema operativo y que Python lo reconozca como un paquete que contiene módulos que pueden importarse, debe crearse un fichero dentro del directorio con el nombre `__init__.py`.

El código de `__init__.py` se invocará cuando el paquete o un módulo del paquete sea imortando en el programa. Esto puede utilizarse para establecer código de inicialización de los paquetes o de los módulos.

Para importar un módulo que se encuentra en un paquete debe utilizarse la sintaxis:

```
import <nombre_paquete>.<nombre_modulo>

from <nombre_paquete>.<nombre_modulo> import <nombre(s)>
```

### 2. Importando todos los módulos de un paquete

Podríamos pensar que para importar todos los módulos de un paquete podríamos utilizar la sintaxis:

```
from <nombre_paquete> import *
```

Sin embargo, ¿qué es lo que sucede?

Python sigue la siguiente convención: si el archivo `__init__.py` en el directorio del paquete contiene una lista llamada `__all__`, se toma como una lista de módulos que deben ser importados cuando se encuentra la sentencia: 

```
from <nombre_paquete> import *.
```

# Dentro del fichero __init__.py del modulo

__all__ = [
    'mimodulo'
]

### 3. Subpaquetes

Los paquetes pueden contener un número arbitrario de paquetes anidados. La sintaxis que se utiliza para acceder a los modulos que se encuentran en los paquetes anidados es similar a la anterior pero añadiendo algunos `.` adicionales:

```
from <nombre_paquete>.<nombre_subpaquete>.<nombre_modulo> import <nombre(s)>
```


# Paquetes

### 1. ¿Qué son los paquetes en Python?

Los paquetes permiten estructurar jerárquicamente los módulos que hemos definido.

Para inicializar un directorio dentro de nuestro sistema operativo y que Python lo reconozca como un paquete que contiene módulos que pueden importarse, debe crearse un fichero dentro del directorio con el nombre `__init__.py`.

El código de `__init__.py` se invocará cuando el paquete o un módulo del paquete sea imortando en el programa. Esto puede utilizarse para establecer código de inicialización de los paquetes o de los módulos.

Para importar un módulo que se encuentra en un paquete debe utilizarse la sintaxis:

```
import <nombre_paquete>.<nombre_modulo>

from <nombre_paquete>.<nombre_modulo> import <nombre(s)>
```

### 2. Importando todos los módulos de un paquete

Podríamos pensar que para importar todos los módulos de un paquete podríamos utilizar la sintaxis:

```
from <nombre_paquete> import *
```
Sin embargo, ¿qué es lo que sucede?

Python sigue la siguiente convención: si el archivo `__init__.py` en el directorio del paquete contiene una lista llamada `__all__`, se toma como una lista de módulos que deben ser importados cuando se encuentra la sentencia: 

```
from <nombre_paquete> import *.
```

# Dentro del fichero __init__.py del modulo

__all__ = [
    'mimodulo'
]

### 3. Subpaquetes

Los paquetes pueden contener un número arbitrario de paquetes anidados. La sintaxis que se utiliza para acceder a los modulos que se encuentran en los paquetes anidados es similar a la anterior pero añadiendo algunos `.` adicionales:
```
from <nombre_paquete>.<nombre_subpaquete>.<nombre_modulo> import <nombre(s)>
```

# PIP - Gestor de paquetes

A continuación se muestra un listado de los comandos principales que podemos utilizar con pip. Ten en cuenta que en los ejemplos se esta utilizando el paquete externo `pandas`.

#### 1. Actualizando pip

>>> python3 -m pip install --upgrade pip

#### 2. Instalando paquetes con pip
>>> pip install pandas

#### 3. Listar los paquetes instalados en el entorno
>>> pip list

#### 4. Mostrar los detalles de un paquete instalado
>>> pip show pandas

#### 5. Exportando los paquetes instalados en el entorno
>>> pip freeze > requirements.txt

#### 6. Instalando `requirements.txt`
>>> pip install -r requirements.txt

#### 7. Desinstalando paquetes
>>> pip uninstall pandas
>>> pip uninstall -r requirements.txt


# Introducción a NumPy

[Numpy](https://numpy.org) es una librería fundamental para la computación científica con Python.

* Proporciona arrays N-dimensionales
* Implementa funciones matemáticas sofisticadas
* Proporciona herramientas para integrar C/C++ y Fortran
* Proporciona mecanismos para facilitar la realización de tareas relacionadas con álgebra lineal o números aleatorios

## Imports
import numpy as np

## Arrays
Un **array** es una estructura de datos que consiste en una colección de elementos (valores o variables), cada uno identificado por al menos un índice o clave. Un array se almacena de modo que la posición de cada elemento se pueda calcular a partir de su tupla de índice mediante una fórmula matemática. El tipo más simple de array es un array lineal, también llamado array unidimensional.

En numpy:

* Cada dimensión se denomina **axis**
* El número de dimensiones se denomina **rank**
* La lista de dimensiones con su correspondiente longitud se denomina **shape**
* El número total de elementos (multiplicación de la longitud de las dimensiones) se denomina **size**

# Array cuyos valores son todos 0

a = np.zeros((2, 4))
a
_**a**_ es un array:

* Con dos **axis**, el primero de longitud 2 y el segundo de longitud 4
* Con un **rank** igual a 2
* Con un **shape** igual (2, 4)
* Con un **size** igual a 8

a.shape
a.ndim
a.size

## Creación de Arrays

# Array cuyos valores son todos 0
np.zeros((2, 3, 4))

# Array cuyos valores son todos 1
np.ones((2, 3, 4))

# Array cuyos valores son todos el valor indicado como segundo parámetro de la función
np.full((2, 3, 4), 8)

# El resultado de np.empty no es predecible 

# Inicializa los valores del array con lo que haya en memoria en ese momento
np.empty((2, 3, 9))

# Inicializacion del array utilizando un array de Python
b = np.array([[1, 2, 3], [4, 5, 6]])
b
b.shape

# Creación del array utilizando una función basada en rangos

# (minimo, maximo, número elementos del array)
print(np.linspace(0, 6, 10))

# Inicialización del array con valores aleatorios
np.random.rand(2, 3, 4)

# Inicialización del array con valores aleatorios conforme a una distribución normal
np.random.randn(2, 4)
%matplotlib inline
import matplotlib.pyplot as plt

c = np.random.randn(1000000)

plt.hist(c, bins=200)
plt.show()

# Inicialización del Array utilizando una función personalizada

def func(x, y):
    return x + 2 * y

np.fromfunction(func, (3, 5))

## Acceso a los elementos de un array

### Array unidimensional

# Creación de un Array unidimensional
array_uni = np.array([1, 3, 5, 7, 9, 11])
print("Shape:", array_uni.shape)
print("Array_uni:", array_uni)

# Accediendo al quinto elemento del Array al igual que con las Listas
array_uni[4]

# Accediendo al tercer y cuarto elemento del Array
array_uni[2:4]

# Accediendo a los elementos 0, 3 y 5 del Array
array_uni[0::3]

### Array multidimensional

# Creación de un Array multidimensional
array_multi = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])
print("Shape:", array_multi.shape)
print("Array_multi:\n", array_multi)

# Accediendo al cuarto elemento del Array
array_multi[0, 3]

# Accediendo a la segunda fila del Array
array_multi[1, :]

# Accediendo al tercer elemento de las dos primeras filas del Array
array_multi[0:2, 2]

## Modificación de un Array

# Creación de un Array unidimensional inicializado con el rango de elementos 0-27
array1 = np.arange(28)
print("Shape:", array1.shape)
print("Array 1:", array1)

# Cambiar las dimensiones del Array y sus longitudes
array1.shape = (7, 4)
print("Shape:", array1.shape)
print("Array 1:\n", array1)

# El ejemplo anterior devuelve un nuevo Array que apunta a los mismos datos. 
# Importante: Modificaciones en un Array, modificaran el otro Array
array2 = array1.reshape(4, 7)
print("Shape:", array2.shape)
print("Array 2:\n", array2)

# Modificación del nuevo Array devuelto
array2[0, 3] = 20
print("Array 2:\n", array2)
print("Array 1:\n", array1)

# Desenvuelve el Array, devolviendo un nuevo Array de una sola dimension
# Importante: El nuevo array apunta a los mismos datos
print("Array 1:", array1.ravel())

## Operaciones aritméticas con Arrays

# Creación de dos Arrays unidimensionales
array1 = np.arange(2, 18, 2)
array2 = np.arange(8)
print("Array 1:", array1)
print("Array 2:", array2)

# Suma
print(array1 + array2)

# Resta
print(array1 - array2)

# Multiplicacion
# Importante: No es una multiplicación de matrices
print(array1 * array2)

## Broadcasting
Si se aplican operaciones aritméticas sobre Arrays que no tienen la misma forma (shape) Numpy aplica un propiedad que se denomina Broadcasting.

# Creación de dos Arrays unidimensionales
array1 = np.arange(5)
array2 = np.array([3])
print("Shape Array 1:", array1.shape)
print("Array 1:", array1)
print()
print("Shape Array 2:", array2.shape)
print("Array 2:", array2)

# Suma de ambos Arrays
array1 + array2

# Creación de dos Arrays multidimensional y unidimensional
array1 = np.arange(6)
array1.shape = (2, 3)
array2 = np.arange(6, 18, 4)
print("Shape Array 1:", array1.shape)
print("Array 1:\n", array1)
print()
print("Shape Array 2:", array2.shape)
print("Array 2:", array2)

# Suma de ambos Arrays
array1 + array2

## Funciones estadísticas sobre Arrays

# Creación de un Array unidimensional
array1 = np.arange(1, 20, 2)
print("Array 1:", array1)

# Media de los elementos del Array
array1.mean()

# Suma de los elementos del Array
array1.sum()

Funciones universales eficientes proporcionadas por numpy: **ufunc**

# Cuadrado de los elementos del Array
np.square(array1)

# Raiz cuadrada de los elementos del Array
np.sqrt(array1)

# Exponencial de los elementos del Array
np.exp(array1)

# log de los elementos del Array
np.log(array1)


# Introducción a Pandas

[Pandas](https://pandas.pydata.org/about/index.html) es una librería que proporciona estructuras de datos y herramientas de análisis de datos de alto rendimiento y fáciles de usar. 

* La estructura de datos principal es el DataFrame, que puede considerarse como una tabla 2D en memoria (como una hoja de cálculo, con nombres de columna y etiquetas de fila). 
* Muchas funciones disponibles en Excel están disponibles mediante programación, como crear tablas dinámicas, calcular columnas basadas en otras columnas, trazar gráficos, etc.
* Proporciona un alto rendimiento para manipular (unir, dividir, modificar…) grandes conjuntos de datos

## Import

import pandas as pd

## Estructuras de datos en Pandas

La librería Pandas, de manera genérica, contiene las siguientes estructuras de datos:

* **Series**: Array de una dimensión
* **DataFrame**: Se corresponde con una tabla de 2 dimensiones
* **Panel**: Similar a un diccionario de DataFrames

## Creación del objeto Series

# Creacion de un objeto Series

s = pd.Series([2, 4, 6, 8, 10])
print(s)

# Creación de un objeto Series inicializándolo con un diccionario de Python

altura = {"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}
s = pd.Series(altura)
print(s)

# Creación de un objeto Series inicializándolo con algunos 
# de los elementos de un diccionario de Python

altura = {"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}
s = pd.Series(altura, index = ["Pedro", "Julia"])
print(s)

# Creación de un objeto Series inicializandolo con un escalar

s = pd.Series(34, ["test1", "test2", "test3"])
print(s)

## Acceso a los elementos de un objeto Series

Cada elemento en un objeto Series tiene un identificador único que se denomina **_index label_**.

# Creación de un objeto Series

s = pd.Series([2, 4, 6, 8], index=["num1", "num2", "num3", "num4"])
print(s)

# Accediendo al tercer elemento del objeto

s["num3"]

# Tambien se puede acceder al elemento por posición

s[2]

# loc es la forma estándar de acceder a un elemento de un objeto Series por atributo

s.loc["num3"]

# iloc es la forma estándar de acceder a un elemento de un objeto Series por posición

s.iloc[2]

# Accediendo al segundo y tercer elemento por posición

s.iloc[2:4]

## Operaciones aritméticas con Series

# Creacion de un objeto Series

s = pd.Series([2, 4, 6, 8, 10])
print(s)

# Los objeto Series son similares y compatibles con los Arrays de Numpy

import numpy as np


# Ufunc de Numpy para sumar los elementos de un Array

np.sum(s)

# El resto de operaciones aritméticas de Numpy sobre Arrays también son posibles
# Más información al respecto en la Introducción a Numpy

s * 2

## Representación gráfica de un objeto Series

# Creación de un objeto Series denominado Temperaturas

temperaturas = [4.4, 5.1, 6.1, 6.2, 6.1, 6.1, 5.7, 5.2, 4.7, 4.1, 3.9]
s = pd.Series(temperaturas, name="Temperaturas")
s

# Representación gráfica del objeto Series

%matplotlib inline
import matplotlib.pyplot as plt

s.plot()
plt.show()

## Creación de un objeto DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

Puede forzarse al DataFrame a que presente unas columnas determinadas y en un orden determinado

# Creación de un DataFrame inicializándolo con algunos elementos de un diccionario
# de objetos Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(
        personas,
        columns = ["altura", "peso"],
        index = ["Ana", "Julia", "Santiago"])
df

# Creación de un DataFrame inicializándolo con una lista de listas de Python
# Importante: Deben especificarse las columnas e indices por separado

valores = [
    [185, 4, 76],
    [170, 0, 65],
    [190, 1, 89]
]

df = pd.DataFrame(
        valores,
        columns = ["altura", "hijos", "peso"],
        index = ["Pedro", "Ana", "Juan"])
df

# Creación de un DataFrame inicializándolo con un diccionario de Python

personas = {
    "altura": {"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}, 
    "peso": {"Santiago": 87, "Pedro": 78, "Julia": 70, "Ana": 65}}

df = pd.DataFrame(personas)
df

## Acceso a los elementos de un DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

### Acceso a los elementos de las columnas del DataFrame

df["peso"]
df[["peso", "altura"]]

# Pueden combinarse los metodos anteriores con expresiones booleanas

df[df["peso"] > 80]

# Pueden combinarse los metodos anteriores con expresiones booleanas

df[(df["peso"] > 80) & (df["altura"] > 180)]

### Acceso a los elementos de las filas del DataFrame

# Mostrar el DataFrame

df
df.loc["Pedro"]
df.iloc[2]
df.iloc[1:3]

### Consulta avanzada de los elementos de un DataFrame

# Mostrar el DataFrame

df
df.query("altura >= 170 and peso > 60")

## Copiar un DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

# Copia del DataFrame df en df_copy
# Importante: Al modificar un elemento de df_copy no se modifica df

df_copy = df.copy()

## Modificación de un DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

# Añadir una nueva columna al DataFrame

df["cumpleaños"] = [1990, 1987, 1980, 1994]
df

# Añadir una nueva columna calculada al DataFrame

df["años"] = 2020 - df["cumpleaños"]
df

# Añadir una nueva columna creando un DataFrame nuevo

df_mod = df.assign(mascotas = [1, 3, 0, 0])
df_mod
df

# Eliminar una columna existente del DataFrame

del df["peso"]
df

# Eliminar una columna existente devolviendo una copia del DataFrame resultante

df_mod = df.drop(["hijos"], axis=1)
df_mod
df

## Evaluación de expresiones sobre un DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series

personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

# Evaluar una función sobre una columna del DataFrame

df.eval("altura / 2")

# Asignar el valor resultante como una nueva columna

df.eval("media_altura = altura / 2", inplace=True)
df

# Evaluar una función utilizando una variable local

max_altura = 180

df.eval("altura > @max_altura")

# Aplicar una función externa a una columna del DataFrame

def func(x):
    return x + 2

df["peso"].apply(func)
df

## Guardar y Cargar el DataFrame

# Creación de un DataFrame inicializándolo con un diccionario de objetios Series
personas = {
    "peso": pd.Series([84, 90, 56, 64], ["Santiago","Pedro", "Ana", "Julia"]),
    "altura": pd.Series({"Santiago": 187, "Pedro": 178, "Julia": 170, "Ana": 165}),
    "hijos": pd.Series([2, 3], ["Pedro", "Julia"])
}

df = pd.DataFrame(personas)
df

# Guardar el DataFrame como CSV, HTML y JSON

df.to_csv("df_personas.csv")
df.to_html("df_personas.html")
df.to_json("df_personas.json")

# Cargar el DataFrame en Jupyter

df2 = pd.read_csv("df_personas.csv")
df2

# Cargar el DataFrame con la primera columna correctamente asignada

df2 = pd.read_csv("df_personas.csv", index_col=0)
df2


# Introducción a Matplotlib

[Matplotlib](https://matplotlib.org) es una librería que permite la creación de figuras y gráficos de calidad mediante el uso de Python.

* Permite la creación de gráficos de manera sencilla y eficiente
* Permite la integración de gráficos y figuras en un Jupyter Notebook

## Import

import matplotlib
import matplotlib.pyplot as plt

# Muestrar los gráficos integrados dentro de jupyter notebook

%matplotlib inline

## Representación gráfica de datos

Si a la función de trazado se le da una matriz de datos, la usará como coordenadas en el eje vertical, y utilizará el índice de cada punto de datos en el array como la coordenada horizontal.

plt.plot([1, 2, 5, 7, 8, 3, 1])
plt.show()

También se puede proporcionar dos matrices: una para el eje horizontal, y otra para el eje vertical.

plt.plot([-3, -1, 0, 4, 7], [1, 4, 6, 7, 8])
plt.show()

Pueden modificarse las logitudes de los ejes para que la figura no se vea tan ajustada

plt.plot([-3, -1, 0, 4, 7], [1, 4, 6, 7, 8])
plt.axis([-4, 8, 0, 10]) # [xmin, xmax, ymin, ymax]
plt.show()

Se sigue el mismo procedimiento para pintar una función matemática

import numpy as np
x = np.linspace(-2, 2, 500)
y = x**2

plt.plot(x, y)
plt.show()

También pude modificarse el estilo de la gráfica para que contenga más información.

plt.plot(x, y)
plt.title("Square function")
plt.xlabel("x")
plt.ylabel("y = x**2")
plt.grid(True)
plt.show()

Pueden superponerse gráficas y cambiar el estilo de las líneas
import numpy as np

x = np.linspace(-2, 2, 500)
y = x**2
y2 = x + 1

plt.plot(x, y, 'b--', x, y2, 'g')
plt.show()

# Separando en diferentes lineas las funciones

import numpy as np
x = np.linspace(-2, 2, 500)
y = x**2
y2 = x + 1

plt.plot(x, y, 'b--')
plt.plot(x, y2, 'g')
plt.show()

Para poder diferenciar entre ambas funciones siempre es recomendable añadir una leyenda

import numpy as np
x = np.linspace(-2, 2, 500)
y = x**2
y2 = x + 1

plt.plot(x, y, 'b--', label="x**2")
plt.plot(x, y2, 'g', label="x+1")
plt.legend(loc="best") # La situa en la mejor localización
plt.show()
Tambien puede crearse dos graficas que no se superpongan. Estas graficas se organizan en un grid y se denominan subplots.
import numpy as np
x = np.linspace(-2, 2, 500)
y = x**2
y2 = x + 1

plt.subplot(1, 2, 1) # 1 rows, 1 columns, 1st subplot
plt.plot(x, y, 'b--')

plt.subplot(1, 2, 2) # 1 rows, 2 columns, 2nd subplot
plt.plot(x, y2, 'g')

plt.show()
Para que las gráficas no queden tan ajustadas, podemos hacer la figura más grande.
plt.figure(figsize=(14,6))

plt.subplot(1, 2, 1) # 1 rows, 1 columns, 1st subplot
plt.plot(x, y, 'b--')
plt.xlabel("x1", fontsize=14)
plt.ylabel("y1", fontsize=14)

plt.subplot(1, 2, 2) # 1 rows, 2 columns, 2nd subplot
plt.plot(x, y2, 'g')
plt.xlabel("x2", fontsize=14)
plt.ylabel("y2", fontsize=14)

plt.show()

## Scatter plots

from numpy.random import rand

x, y = rand(2, 100)
plt.scatter(x, y)
plt.show()
from numpy.random import rand

x, y = rand(2, 100)
x2, y2 = rand(2, 100)

plt.scatter(x, y, c='red')

plt.scatter(x2, y2, c='blue')

plt.show()

## Histogramas

data = [1, 1.1, 1.8, 2, 2.1, 3.2, 3, 3, 3, 3]

plt.subplot(211) # 2 rows, 1 columns, 1st subplot
plt.hist(data, bins = 10, rwidth=0.8)
plt.xlabel("Value")
plt.ylabel("Frequency")

plt.subplot(212) # 2 rows, 1 columns, 2nd subplot
plt.hist(data, bins = [1, 1.5, 2, 2.5, 3], rwidth=0.95)
plt.xlabel("Value")
plt.ylabel("Frequency")

plt.show()

## Guardar las figuras

import numpy as np

x = np.linspace(-2, 2, 500)
y = x**2
y2 = x + 1

plt.plot(x, y, 'b--', label="x**2")
plt.plot(x, y2, 'g', label="x+1")
plt.legend(loc="best")

plt.savefig("mi_grafica.png", transparent=True)


# Excepciones en Python 3

### 1. ¿Qué son las excepciones?

Python utiliza un tipo de objeto especial denominado excepción para gestionar los errores que surgen durante la ejecución de un programa. 

Cada vez que ocurre un error que hace que Python no sepa qué hacer a continuación, crea un objeto de excepción. Si se escribe código que maneja la excepción, el programa continuará ejecutándose. Por el contrario, si no se maneja la excepción, el programa se detendrá y mostrará un pequeño resumen de la excepción que se ha producido.

Las excepciones se pueden manejan a través de las sentencias `try` y `except`.
print(var)

### 2. Errores de sintaxis vs Excepciones

A pesar de que en muchas ocasiones estos dos términos se utilizan de manera indistinta cuando 
hablamos de Python, debemos tener cuidado porque son cosas diferentes.

Los **errores de sintaxis** se producen cuando escribimos una sentencia de código en Python que no es sintácticamente válida. El intérprete de Python indica estos error con el término `SyntaxError` y nos señala con el carácter `^` donde se encuentra el error.
print("Hola mundo)

**Este tipo de errores no se pueden controlar y no se corresponden con excepciones dentro del lenguaje**

Por otro lado, las **excepciones** se corresponden con errores que se producen en sentencias de código en Python que son sintácticamente correctas. Esto tipo de errores no son fatales para el programa y pueden ser gestionados o ignorados.
print(var)
50/0
'2' + 2

### 3. Gestión de excepciones: Sentencias `try` y `except`

Las sentencias `try` y `except` en Python pueden utilizarse para capturar y manejar excepciones. Python ejecuta el código que sigue a la sentencia `try` como una parte "normal" del programa. El código que sigue a la sentencia `except` se ejecutará si se produce cualquier excepción en la cláusula `try` precedente.

La sintaxis que se utiliza para definir este tipo de comportamiento es la siguiente:

```
try:
    <sentencia(s)>
except <excepción>:
    <sentencias(s) si excepción>
```

print(var)
try:
    print(var)
except NameError:
    var = "Hola mundo"
print(var)

Debemos tener en cuenta que el las sentencias de código que se encuentren en el cuerpo de la sentencia `try` y a continuación de la sentencia que emite la excepción, no se ejecutarán
print("Sentencias de codigo antes del try")

try:
    print("Codigo antes de la excepcion")
    10 + "3"
    print("Codigo despues de la excepcion")
except TypeError:
    print("No se puede sumar un numero entero y un string")
    
print("Sentencias de codigo despues del except")

También podemos utilizar la sentencia `except` sin indicarle el nombre de ninguna excepción, en estos casos capturará todas las excepciones que se produzcan en el código que se encuentra en el cuerpo de la sentencia `try`

try:
    10 + "3"
except:
    print("No se puede sumar un entero y un string")

Adicionalmente a la sintaxis anterior, podemos capturar varias excepciones de manera simultánea utilizando varias cláusulas `except`

try:
    50/0
except NameError:
    print("Gestionando excepcion NameError")
except TypeError:
    print("Gestionando execpcion Type Error")
except ZeroDivisionError:
    print("No puedes dividir un numero por 0")

Por último, podemos asignar el objeto excepción capturado a una variable y utilizarlos para mostrar más información al respecto.
try:
    print(variable)
except NameError as error:
    print("Objeto de tipo:", type(error))
    print("La excepcion consiste en:", error)

### 4. Lanzando excepciones personalizadas

Además de las sentencias anteriores que podemos utilizar para controlar excepciones, Python nos proporciona la sentencia `raise` con la que podemos emitir nuestras propias excepciones. Para ello, debemos utilizar la clase por defecto de Python `Exception`

help(Exception)
colores_permitidos = ("azul", "verde", "rojo")

color = "amarillo"

if color not in colores_permitidos:
    raise Exception("El color {} no se encuentra en la lista de colores permitidos".format(color))
colores_permitidos = ("azul", "verde", "rojo")

color = "verde"

if color not in colores_permitidos:
    raise Exception("El color {} no se encuentra en la lista de colores permitidos".format(color))

### 5. Excepción `AssertionError`

Como complemento a todas las sentencias anteriores, Python nos proporciona una sentencia adicional que nos permite verificar en un punto determinado de nuestro programa que todo esta funcionando adecuadamente, esta sentencia es `assert`.
passwd = input("Introduce una contrasena de mas de 8 digitos:")

assert len(passwd) > 8, "La contrasena es menor a 8 digitos"

### 6. Cláusula `else` en excepciones

Curiosamente, Python nos proporciona un mecanismo por el cual utilizando la sentencia `else`, se puede indicar a un programa que ejecute un determinado bloque de código sólo en ausencia de excepciones.

try:
    print(variable2)
except NameError:
    print("variable2 no estaba definida, se define con la cadena 'Hola mundo'")
    variable2 = 'Hola mundo'
else:
    print("variable2 ya estaba definida con el valor:", variable2)

### 7. Sentencia `finally`

Python nos proporciona una última sentencia que podemos utilizar para realizar una "limpieza" después de la ejecución de nuestro código al gestionar una excepción. Esta sentencia se denomina `finally` y el código que se localice en su cuerpo, se ejcutará siempre, independientemente de si se produce o no la expcepción.

try:
    print(variable3)
except NameError:
    print("variable3 no estaba definida, se define con la cadena 'Hola mundo'")
    variable3 = 'Hola mundo'
else:
    print("variable3 ya estaba definida con el valor:", variable2)
try:
    print(variable3)
except NameError:
    print("variable3 no estaba definida, se define con la cadena 'Hola mundo'")
    variable3 = 'Hola mundo'
else:
    print("variable3 ya estaba definida con el valor:", variable2)
finally:
    del variable3

# Listado de excepciones en Python

A continuación se muestra una lista de las excepciones más relevantes en Python 3 y una breve descripción en inglés:

## Exception

Clase base para todas las excepciones

## StopIteration

Aparece cuando el método next() de un iterador no apunta a ningún objeto.

## SystemExit

Activado por la función sys.exit().

## StandardError

Clase base para todas las excepciones incorporadas excepto StopIteration y SystemExit.

## ArithmeticError

Clase base para todos los errores que se producen en el cálculo numérico.

## OverflowError

Aparece cuando un cálculo supera el límite máximo para un tipo numérico.

## FloatingPointError

Aparece cuando falla un cálculo en coma flotante.

## ZeroDivisonError

Aparece cuando se produce una división o un módulo por cero para todos los tipos numéricos.

## AssertionError

Aparece en caso de fallo de la sentencia Assert.

## AttributeError

Aparece en caso de fallo en la referencia o asignación de atributos.

## EOFError

Se activa cuando no hay entrada desde la función raw_input() o input() y se alcanza el final del fichero.

## ImportError

Aparece cuando falla una sentencia import.

## KeyboardInterrupt

Se activa cuando el usuario interrumpe la ejecución del programa, normalmente pulsando Ctrl+c.

## LookupError

Clase base para todos los errores de búsqueda.

## IndexError

Aparece cuando no se encuentra un índice en una secuencia.

## KeyError

Aparece cuando la clave especificada no se encuentra en el diccionario.

## NameError

Aparece cuando no se encuentra un identificador en el archivolocal o global namespace.

## UnboundLocalError

Aparece cuando se intenta acceder a una variable local en una función o método pero no se le ha asignado ningún valor.

## EnvironmentError

Clase base para todas las excepciones que ocurren fuera del entorno Python.

## IOError

Aparece cuando falla una operación de entrada/salida, como la sentencia print o la función open() al intentar abrir un archivo que no existe.

## OSError

Aparece cuando se producen errores relacionados con el sistema operativo.

## IndentationError

Aparece cuando la sangría no se especifica correctamente.

## SystemError

Aparece cuando el intérprete encuentra un problema interno, pero cuando se encuentra este error el intérprete de Python no sale.

## SystemExit

Aparece cuando se sale del intérprete de Python usando la función sys.exit(). Si no se maneja en el código, provoca la salida del intérprete.

## TypeError

Aparece cuando se intenta realizar una operación o función que no es válida para el tipo de datos especificado.

## ValueError

Aparece cuando la función incorporada para un tipo de datos tiene el tipo válido de argumentos, pero los argumentos tienen valores no válidos especificados.

## RuntimeError

Aparece cuando un error generado no entra en ninguna categoría.

## NotImplementedError

Aparece cuando un método abstracto que debe implementarse en una clase heredada no está implementado.






