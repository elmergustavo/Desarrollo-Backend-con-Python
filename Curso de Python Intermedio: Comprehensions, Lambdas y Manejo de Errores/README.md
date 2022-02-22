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



