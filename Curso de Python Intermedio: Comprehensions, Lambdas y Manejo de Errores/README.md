# El Zen de Python

El Zen de Python se compone por los principios para escribir tu código de manera clara, sencilla y precisa. Estos son:

    Bello es mejor que feo:
    Pyhton es estéticamente superior a cualquier otro lenguaje de programación. Al momento de escribir código, es mejor que sea de manera limpia y estética.
    Explícito es mejor que implícito:
    Hacer más fácil que las otras personas entiendan el código.
    Simple es mejor que complejo:
    Es mejor tener una implementación simple, que ocupe pocas lineas de código y sea entendible, a que sea una larga y complicada.
    Complejo es mejor que complicado:
    Si tenemos que extendernos en la implementación y hacerla más compleja para que el código si se entienda, esto es mejor que hacerlo simple y mal.
    Plano es mejor que anidado:
    El anidamiento es cuando tenemos un bloque de código dentro de otro bloque de código (dependiendo de este). Esto se nota en Python por la identación, nos quedarían estos bloques muy corridos a la derecha.
    Es mejor evitar el anidamiento, y hacer las cosas de manera plana.
    Espaciado es mejor que denso:
    Por la identación de Python (sus sangrías), este principio se nos hace imposible de esquivar. El código inevitablemente es espaciado.
    La legibilidad es importante:
    Es importante que otros programadores puedan entender lo que estamos escribiendo. Esto hace más fáciles las cosas cuando trabajemos con otros en los proyectos.
    Los casos especiales no son lo suficientemente especiales cpmo para romper las reglas (sin embargo, la practicidad le gana a la pureza):
    Siempre que podamos respetar estas reglas que nos plantea Python, es mejor así. Sin embargo, si por el hecho de hacer un código muy puro o muy ‘Pythonista’, este pierde legibilidad, es mejor ser más prácticos y romper o saltearnos algunas de estas reglas para que el código sea más eficiente. Por lo tanto, llegado el momento debermos decidir si es mejor hacer las cosas de manera pura o práctica.
    Los errores nunca deberían pasar silenciosamente (a menos que se silencien explícitamente):
    Manejar los erroes es fundamental. Cada error nos dice algo y hay que prestarle atención. A menos que seas capaz de silenciar un error explícitamente, aunque para esto hay que tener criterio.
    Frente a la ambiguedad, evitar la tentación de adivinar:
    Nuestro código debería solamente tener una interpretación. Si en un contexto significa algo, y en otro otra cosa, es mejor que lo revisemos y busquemos una solución.
    Debería haber una, y preferiblemente sola, una manera obvia de hacerlo. (A pesar de que esa manera no sea obvia a menos que seas holandés):
    Esto hace referencia al creador de Python ''Guido van Rossum", que de manera muy inteligente encontrar las soluciones precisas a los problemas, y deberíamos imitarlo.
    Ahora es mejor que nunca:
    Es mejor desarrollar nuestra solución cuánto antes, no dejarlo para mañana o para mas adelante.
    A pesar de que nunca es muchas veces mejor que ahora mismo:
    Si por hacer las cosas ya y tenemos poco tiempo, si es mejor dejarlo para después y no hacerlo apurado y mal.
    Si la implementación es díficil de explicar, es una mala idea, y si es fácil de explicar, es una buena idea:
    Si somos capaces de explicar nuestra implementación a otros desarrolladores paso a paso, es una buena idea. En cambio si no podemos hacerlo, significa que ni nosotros entendemos la implementación y deberíamos repensar nuestra forma de encarar la solución.
    **Los espacios de nombres son una gran idea, ¡Tengamos más de esos! (namespaces):
    Es el nombre que se ha indicado luego de la palabra import, es decir la ruta (namespace) del módulo. (Lo veremos a profundidad más adelante).

## ¿Qué es un entorno virtual?
* https://docs.python.org/es/3/tutorial/venv.html

Resumiendo lo que dice la documentación de Python sobre Entornos Virtuales
.
Un entorno virtual es un directorio que contiene una instalación de Python de una versión en particular, además de unos cuantos paquetes adicionales.
.
Ejemplo:
La aplicación A puede tener su propio entorno virtual con la versión 1.0 instalada mientras que la aplicación B tiene otro entorno virtual con la versión 2.0. Si la aplicación B requiere que actualizar la librería a la versión 3.0, ésto no afectará el entorno virtual de la aplicación A.

Los entornos virtuales son de mucha utilidad ya que nos ayudan a tener versiones especificas de librerías o módulos a un proyecto sin afectar a otros. De esta forma en el mismo equipo pueden coexistir distintos proyectos con distintas versiones de la misma librería o modulo.

![](https://static.platzi.com/media/user_upload/Screenshot%20from%202021-04-06%2015-17-31-98f9a6fa-3e6c-4353-9644-31a4e7208737.jpg)
![](https://static.platzi.com/media/user_upload/Screenshot%20from%202021-04-06%2015-10-22-1804c0b6-79d2-40bd-aced-f859f86c5309.jpg)

## El primer paso profesional: creación de un entorno virtual
* https://docs.python.org/es/3/tutorial/venv.html

Creando un ambiente virtual con VENV
Creación de ambiente Virtual:

python3 -m venv nombre_venv

Usualmente el nombre del ambiente virtual es venv.
Activación del ambiente virtual:

Windows:
.\venv\Scripts\activate

Unix o MacOS:
source venv/bin/activate

Desactivar el ambiente virtual:

deactivate

Crear un alias en linux/mac:

alias nombre-alias="comando"

``alias avenv=“source venv/bin/activate”``

Clase del curso de Git y Github 👩🏽‍💻

Aquí les dejo los pasos para crear un alias en Linux Ubuntu:
Para hacerlo en este sistema operativo, necesitamos que cada que la terminal cargue, el alias sea leído, para ello, la terminal tiene un archivo llamado .bashrc que contiene la configuración inicial, y usualmente se encuentra en nuestro home, por lo que hacemos lo siguiente:

Ejecutar sudo nano ~/.bashrc
Ir al final del archivo
Agregar el comando: alias avenv='source venv/bin/activate'
Guardar presionando ctrl + o y luego salir con ctrl + x
Reejecutar la configuración de la terminal: source ~/.bashrc
Activar el entorno vitual avenv
`
## para linux

sudo apt-get install python3-venv

## sudo apt-get install python3-venv

## Instalación de dependencias con pip

* https://pypi.org/project/pipenv/
* https://github.com/pyenv/pyenv
* https://platzi.com/cursos/web-scraping/
* https://platzi.com/cursos/pandas/

```

Básicamente, pip es como el npm de JavaScript, y el archivo requeriments.txt es como el package.json de JavaScript.
Es importante recordar que esto se debe correr con el entorno virtual activado (avenv), de esta manera todas las dependencias que instalemos se guardaran para este entorno virtual (de lo contrario se guardarían de manera global, que es justo lo que no queremos).
Algo importante, si estás manejando git, es bueno siempre ignorar la carpeta venv, esto porque realmente no nos importa subir todo eso al repositorio, puedes mirarlo como que venv es el node_modules de JavaScript, a fin de cuentas, cualquier otro programador que trabaje con nuestro código creará su propio entorno virtual e instalará las dependencias que dejamos en nuestro requeriments.txt.
Y un dato curioso es que, el operador > en la terminal es algo especial de UNIX, ya que este operador lo que hace es redirigir la salida de cualquier comando hacia donde lo mandes, por defecto la salida es en la terminal, pero al usar > le dijimos a la terminal que, en lugar de que la salida sea en la terminal, que se redirija al archivo requeriments.txt 👀. Si quieren jugar con ello, pueden hacerlo con este ejemplo: ls -al > test.txt, eso creará un archivo llamado test.txt, y si lo abren verán cómo es que ese comando funciona 😄
Resumen
Pip (package installer for python) Nos permite descargar paquetes de terceros para utilizarlos en nuestro enviroment, ademas se puede definir una versión especifica del paquete.


pip install <paquete> instala el paquete(pandas , matplotlib, bokeh, etc) que se especifique

pip freeze muestra todos los paquetes instalados en tu ambiente virtual


Si quisiéramos que alguien mas pueda ejecutar nuestro proyecto es importante compartir que librería y versión hemos empleado; eso se realiza con el comando:
    
pip freeze > requirements.txt
El resultado de pip freeze se escribe en requirements.txt (puedes usar otro nombre pero el mostrado es una buena practica)

```
para instalar paquetes desde un archivo como requirements.txt ejecutamos:

```pip install -r requirements.txt```
    
## Listas y diccionarios anidados
![](https://static.platzi.com/media/user_upload/code-a45e30d1-b20b-47cd-b3ab-d6a8efabeffb.jpg)
![](https://static.platzi.com/media/user_upload/carbon-a5a5b903-f318-45c6-926d-7d08ab4f481f.jpg)
![](https://static.platzi.com/media/user_upload/Curso%20de%20Python%20Intermedio-3-2a7a270f-1b99-46c9-9123-b876f6c580c2.jpg)

## Dictionary comprehensions
```py
    def run():

    my_dict = {i : round(i**0.5,2) for i in  range(1,1001)}

    print(my_dict)

if __name__=='__main__':
    run()
```

* https://docs.python.org/3/tutorial/controlflow.html?highlight=lambda#lambda-expressions
![](https://static.platzi.com/media/user_upload/lambda.png-c06b5ab0-03d2-42c2-a442-19559fee74d6.jpg)

## High order functions: filter, map y reduce
La diferencia entre filter y map:

filter devuelve True or False según el valor esté dentro de los criterios buscados o no. En caso de que no cumpla con la condición, no será devuelto y la lista se verá reducida por este filtro.
Map funciona muy parecido, pero su diferencia radica en que no puede eliminar valores de la lista del array entregado. Es decir, el output tiene la misma cantidad de valores que el input.
Cómo funciona reduce:

Reduce toma 2 valores entregados como parámetros y el iterador como otro parámetro. Realiza la función con estos 2 valores, y luego con el resultado de esto y el valor que le sigue en el array. Y así hasta pasar por todos los valores de la lista.

```py
from functools import reduce
def main():

    #Filter
    myList = [1,4,5,7,9,13,19,21]

    odd = list(filter(lambda x: x % 2 != 0, myList))
    print(odd)

    #Map
    myList2 = [1, 2, 3, 4, 5]

    squares = list(map(lambda x: x**2, myList2))
    print(squares)

    myList3 = [2, 2, 2, 2, 2]
    
    allMultiplied = reduce(lambda a, b: a * b, myList3)
    print(allMultiplied)

if __name__ == '__main__':
    main()
```
 * https://www.youtube.com/watch?v=hUes6y2b--0


```py
"""
Dada una lista de numeros filtra para quedarte solo con 
los números impares
"""

my_list = [i for i in range(10)]

# Usando def
def get_odds(arr):
    odds = []
    for n in arr:
        if n % 2 == 1:
            odds.append(n)
    return odds

# Usando List Comprehension
odds = [n for n in my_list if n % 2 == 1]

# Usando Filter
odds_filter = list(filter(lambda n: n % 2 == 1, my_list))
print(odds_filter)
```
Map
Funciona muy parecido, pero su diferencia radica en que no puede eliminar valores de la lista del array entregado. Es decir, el output tiene la misma cantidad de valores que el input.
```py
"""
Obtener todos los numeros de una lista multiplicados al cuadrado
"""

# Usando Def
def get_squares(arr):
    squares = []
    for n in arr:
        squares.append(n * n)
    return squares

# Usando List Comprehension
squares = [n * n for n in my_list]

# Usando Map
squares_map = list(map(lambda x: x*x, my_list))
print(squares_map)
```
Reduce
Toma 2 valores entregados como parámetros y el iterador como otro parámetro. Realiza la función con estos 2 valores, y luego con el resultado de esto y el valor que le sigue en el array. Y así hasta pasar por todos los valores de la lista.
```py
"""
Suma todos los valores de una lista
"""
from functools import reduce

# Usando def
def get_sum(arr):
    result = 0
    for n inarr:
        result += n
    return result

# Usando Reduce
sum = reduce(lambda a, b: a + b, my_list)
print(sum)
```

* https://taverasmisael.com/blog/usar-map-filter-y-reduce-para-olvidarnos-de-los-bucles-for#:~:text=A%20diferencia%20de%20filter%2C%20map,de%20la%20transformaci%C3%B3n%20que%20apliquemos.&text=A%20map%20le%20pasamos%20una,sin%20afectar%20el%20array%20original

## Los errores en el código

* https://realpython.com/python-exceptions/
* https://docs.python.org/3/tutorial/errors.html

Errores en el código
Cuando python nos avisa que tenemos un error en el código nos avienta un mensaje que conocemos como traceback, puesde ser debido a:

Errores de Sintaxis (SyntaxError) → escribimos mal alguna palabra clave (typo), el programa no se ejecuta.
Excepciones (Exeption) → Producen un colapso o interrupción de la lógica del programa en alguna línea en específico por ejemplo (todas las líneas anteriores se ejecutan), pueden ser de varios tipos, generalmente aparecen cuando no existe un componente clave en la ejecución o hay alguna imposibilidad lógica (matemática) para efectuar la instrucción, tambipen pueden generarse dentro del código o fuera de el (elevar una excepción)
Lectura de un traceback

La manera correcta de leer un traceback es iniciar por el final, en el caso de un error de sintaxis nos indicará en qué línea se encuentra dicho error.
En el caso de excepciones la última línea nos indicará el tipo de exepcion que se generó (generalmente son autoexplicativas pero si no entienedes que paso puedes buscar este error)
La penúltima línea nos indicará dende se encuentra el error (archivo y línea)
La antepenúltima línea nos muestra “most recent call last” lo que significa que la llamada más reciente es la última (el programa se cerró después de esa llamada, se genero un error)
Elevar una excepción

Cuando tenemos una excepción en python lo que sucede es que se crea un objeto de tipo exception que se va moviendo a través de los bloques de código hasta llegar al bloque principal si es que no se maneja dicha excepción en algún bloque intermedio el programa se interrumpe y genera el traceback

Los errores son parte de nuestra vida como programadores y hay que saber lidiar con ellos.

Errores:

Syntax Error -> Errores de escritura, Python no ejecuta el programa.
Exception -> Python se detiene en una línea en específica
KeyboardInterrupt -> Ctrl + C
KeyError -> Cuando tratamos de acceder a una llave que no existe
IndexError -> Cuando tratamos de acceder a un índice que no existe
FileNotFoundError -> Archivo que no existe
ZeroDivisionError -> Dividir entre 0
ImportError -> Intentamos importar un módulo que tiene un error
Estos son solo algunos ejemplos, hay más de 50 excepciones.

“Elevar”, quiere decir que Python crea un objeto de tipo excepción.

Traceback son los errores que muestran en las consolas. Lo correcto es leer desde el final hasta el principio. En el final nos dirá cuál es la excepción que ocurrió.

## Debugging
Debugging:

O depuración es una herramienta que traen varios editores de código con el objetivo de solucionar nuestros errores de lógica. Revisemos la herramienta debugging de VSCode
En este entorno podemos acceder a funcionalidades como:
pause → permite pausar la ejecución del programa
step over → permite avanazr un solo paso en el programa
step in → igresamos a un bloque secundario del programa (funciones)
step out → salimos del bloque secundario
restart → reinicia el programa
stop → detiene el programa
Además podemos generar breakpoints, que son puntos en los que el programa se detendrá para ayudarnos a depurar el código
Nota:

Existen herramientas de debugging propias de python como el módulo pdb o los breakpoints (a partir de python 3.7)

## Manejo de excepciones

* https://docs.python.org/3/tutorial/errors.html#exceptions

Algo que aparece casi al final de la lectura recomendada en el documentación de Python es que se puede agregar un “else” al try-except.

TRY: En el try se coloca código que esperamos que pueda lanzar algún error.
EXCEPT: En el except se maneja el error, es decir, si ocurre un error dentro del bloque de código del try, se deja de ejecutar el código del try y se ejecuta lo que se haya definido en el Except.
ELSE: El else se ejecuta sólo si no hubo ninguna excepción lanzada desde el try
FINALLY: Se ejecuta SIEMPRE, haya sido lanzada la excepción o no haya sido lanzada.

## Poniendo a prueba el manejo de excepciones

* https://docs.python.org/3/tutorial/errors.html#exceptions

```py
def divisors(num):
    divisors = []
    for i in range(1, num + 1):
        if num % i == 0:
            divisors.append(i)
    return divisors


def run():
    while True:
        try:
            num = int(input('Ingresa un número: '))
            if num < 0:
                raise ValueError
            print(divisors(num))
            print("Terminó mi programa")
            break
        except ValueError:
            print("Debes ingresar un entero positivo")


if __name__ == '__main__':
    run()
```

```py
<def divisor(num):
    try:
        if num < 0:
            raise ValueError("ingresa un número positvo")
        divisors =[i for i in range(1, num + 1) if num % i == 0]
        return divisors
    except ValueError as ve:
        print(ve)
        return False


def run():
    try: 
        num = int(input(f'Ingresa un número: '))      
        print(divisor(num))
        print("termino mi programa")
    except ValueError:
        print("ingresa un número")
    
if __name__ =='__main__':
    run()> 
```

```py
def divisors(num):
    try:
        if num < 0:
            raise ValueError('Ingresa solo números positivos')
        else:
            divisors = [i for i in range(1, num + 1) if num % i == 0]
            return divisors
    except ValueError as value_error:
        print(value_error)
        return str(num) + " No es nu numero positivo"


def run():
    try:
        num = int(input("Ingresa un número: "))
        print(divisors(num))
        print("Terminó mi programa")
    except ValueError:
        print("Debes ingresar un número")


if __name__ == "__main__":
    run()
```
## Assert statements

```py
def divisor(num):
    divisors = [i for i in range(1,num+1) if num%i == 0]
    return divisors

def run():
    num = input('Enter a number: ')
    assert num.isnumeric() and int(num)>0, 'Ingresa solo numeros positivos'
    print(divisor(int(num)))
    print('Finish')


if __name__ == '__main__':
    run()
```

Assert statements

Es una manera poco usual de manejar los errores en python
Evalúa una condicional, si esta se cumple continuamos con el flujo normal del python, si no se cumple eleva un error del tipo AssertionError y nos muestra un mensaje.
Su sintaxis es:

```py
assert <condicion>, <"mensaje">
<código>
```
## Trabajando con archivos de texto en Python

```py
def read():
    numbers = []
    with open("./archivos/numbers.txt", "r") as f: 
        for line in f:
            numbers.append(int(line))
    print(numbers)


def write():
    names = ["Facundo", "Gregorio", "Marta", "Susana", "Jose"]
    with open("./archivos/names.txt", "w") as f:
        for name in names: 
            f.write(name)
            f.write("\n")


def run():
    write()


if __name__ == '__main__':
    run()
```
![](https://static.platzi.com/media/user_upload/1-5b2d21b0-06da-4635-8b05-65c54354e1b0.jpg)

```py
def read():
    names = []
    with open("./archivos/name.txt", "r", encoding="utf-8") as f:
        for line in f: 
            if len(line.strip()) > 0:
                names.append(line.strip())
    if len(names)> 0:
        print(names)
    else:
        print("Archivo vacio")

def write():
    names = []
    with open("./archivos/name.txt", "w" , encoding="utf-8") as f:
        for name in names:
            f.write(name)
            f.write('\n')

def agregar_nombre(nombre):
    with open("./archivos/name.txt", "a" , encoding="utf-8") as f:
        f.write(nombre)
        f.write("\n")

def borrar_nombre(nombre):
    names = []
    with open("./archivos/name.txt", "r", encoding="utf-8") as f:
        for line in f: 
            if len(line.strip()) > 0 and line.strip()!= nombre:
                names.append(line.strip())
    with open("./archivos/name.txt", "w" , encoding="utf-8") as f:
        for name in names:
            f.write(name)
            f.write('\n')

    
def run():
    sw = True
    while sw:
        try:
            print("""  
----------------------------------------------------------------------
            Seleccione un numero:
            1. Crear un nuevo archivo 
            2. Agregar nombre
            3. Listar nombre
            4. Borrar nombre
            5. Salir del programa
----------------------------------------------------------------------
            """)
            n = int(input("Ingrese una opcion :   "))
            if n == 1:
                write()
            elif n == 2:
                nombre = input("Ingrese el nombre a agregar: ")
                agregar_nombre(nombre)
            elif n == 3:
                read()
            elif n == 4:
                nombre = input("Ingrese el nombre a borrar : ")
                borrar_nombre(nombre)
            elif n ==5:
                sw = False
                print("Programa Terminado!")
        except ValueError :
                print("Error seleccione una opcion correcta")
    # write()

if __name__ == '__main__':
    run()
```

## Reto final: Juego del Ahorcado o Hangman Game

```py
import random
import os


def read_data(filepath="./archivos/data.txt"):
    words = []
    with open(filepath, "r", encoding="utf-8") as f:
        for line in f:
            words.append(line.strip().upper())
    return words


def run():
    data = read_data(filepath="./archivos/data.txt")
    chosen_word = random.choice(data)
    chosen_word_list = [letter for letter in chosen_word]
    chosen_word_list_underscores = ["_"] * len(chosen_word_list)
    letter_index_dict = {}
    for idx, letter in enumerate(chosen_word):
        if not letter_index_dict.get(letter): 
            letter_index_dict[letter] = []
        letter_index_dict[letter].append(idx)
    
    while True:
        os.system("cls") # Si estás en Unix (Mac o Linux) cambia cls por clear
        print("¡Adivina la palabra!")
        for element in chosen_word_list_underscores:
            print(element + " ", end="")
        print("\n")

        letter = input("Ingresa una letra: ").strip().upper()
        assert letter.isalpha(), "Solo puedes ingresar letras"

        if letter in chosen_word_list:
            for idx in letter_index_dict[letter]:
                chosen_word_list_underscores[idx] = letter
        
        if "_" not in chosen_word_list_underscores:
            os.system("cls") # Si estás en Unix (Mac o Linux) cambia cls por clear
            print("¡Ganaste! La palabra era", chosen_word)
            break


if __name__ == '__main__':
    run()

# ¿Viendo la solución? No hay drama crack
# Python es mejor que JavaScript
```
