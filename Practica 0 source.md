#Practica 0: Modelos de Computación  
---

##El entscheidungsproblem.
___
El entscheidungsproblem es uno de los problemas planteados por **Hilbert**  en 1928. Consiste en encontrar un algoritmo que sea capaz de deducir si una formula de la lógica de primer orden es una tautología o no.  
>Nota: El origen de la pregunta se remonta al siglo XVII cuando Leibniz después de crear su calculadora mecanica se propuso crear una máquina que fuese capaz de decir si un teorema era cierto o no.

En 1936 **Alonso Church** y **Alan Turing** demostraron de forma independiente que es imposible encontrar dicho algoritmo.
___
##Turing, Church y el entscheidungsproblem. 
___  
**Alonzo Church** (14 de junio de 1903 - 11 de agosto de 1995), fue  un matemático y lógico norteamericano conocido por ser el padre de la computación teórica.  

Church desarrolló el cálculo lambda y lo utilizó para demostrar la existencia de problemas indecibles (problemas en los que no hay algoritmo que de una respuesta *si o no* correcta.  
Más adelante su alumno Alan Turing demostó la exisitencia de problemas que no podían ser resueltos mediante una maquina de Turing (problema de la parada).  
Más adelante al revisar la tesis de Turing demostraron que el cálculo lambda y la maquina de Turing eran equivalentes en el sentido de que resolvian los mismos problemas. Lo que dio lugar a la tesis de Church-Turing.
___
##Vida y contribución de Turing a la computabilidad.
___
Alan Mathison Turing, nació en Londres en 1912 y demostró su inteligencia a muy temprana edad.
Se graduó en la licenciatura de matemáticas en 1934 y en 1935 fue nombrado profesor del King's College.
En 1938 obtuvo su doctorado en matemáticas con su tesis sobre la maquina de Turing y el entscheidungsproblem.
Durantela Segunda Guerra Mundial participó activamente descifrando codigos enigma mediante una maquina de Turing llamada Colossus que podemos considerar el primer ordenador digital de la historia, tras la guerra se destruyeron las maquinas Colossus y sus planos por motivos militares ya que eran alto secreto entonces.
___
##La tesis de Church-Turing
___
En teoría de la computabilidad, la tesis de Church-Turing formula hipotéticamente la equivalencia entre los conceptos de función computable y máquina de Turing, que expresado en lenguaje corriente vendría a ser "todo algoritmo es equivalente a una máquina de Turing". No es un teorema matemático, es una afirmación formalmente indemostrable, una hipótesis que, no obstante, tiene una aceptación prácticamente universal.

___
##Variantes de la tesis de Church-Turing
___
Tras un estudio exhaustivo se ha podido comprobar que existen diversas versiones de la tesis de Church-Turing. Esto se debe a que, cuando Turing enunció su tesis no lo hizo de manera formal y concisa, sino que esta tesis es bastante ambigüa. Esto ha provocado que los científicos que la han utilizado o la han leído, la hayan interpretado de manera diferente.

La formulación original de la tesis de Church se muestra a continuación:

        "A function of positive integers is effectively calculable only if recursive."

Es decir, una función de enteros positivos es efectivamente calculable sólo si es recursiva.

####Versiones alternativas:
La version actual mas aceptada es:

        "Todo algoritmo o procedimiento efectivo es Turing-computable."
Hay una gran variedad de definiciones alternativas puesto que la formulación original es un tanto ambigua.

Lo que si es innegable es la gran cantidad de interpretaciones que se han dado a dicha tesis:

* **Principio Church-Turing-Deutsch:** 

    Deutsch afirma que la tesis de Church es demasiado general en comparación con algunos de los principios físicos conocidos.  
    Deutsch propone referirse a las "funciones que de manera natural sean consideradas computables" como "funciones que puedan ser computadas por un sistema físico real", ya que de esta forma lo que se quiere expresar es mucho más concreto.   
    De esta manera, Deutsch convierte la tesis en un principio llamado "Principio de Church-Turing-Deutsch" cuyo enunciado se muestra a continuación:
    
    *"Todos los sistemas físicos finitos comprensibles pueden ser simulados por una máquina de computación universal que opere en pasos finitos".*
    
* **Tesis Física de Church-Turing (PCTT):**  

    *"Cualquier función que pueda ser físicamente computable, puede ser computada por una máquina de Turing."*

    En 2002 este teorema fue refutado por Willem Fouché, puesto que descubrió que las máquinas de Turing no pueden obtener todos los valores posibles, unidimensionales, de los números racionales.
    
* **Strong Church-Turing thesis (SCTT):**

    En 1997, Bernstein y Vazirani expusieron la tesis Strong Church-Turing (SCTT), cuyo enunciado se muestra a continuación:  
    *"Any ‘reasonable’ model of computation can be efficiently simulated on a probabilistic Turing machine".*  
    Es un misterio que la tesis original de Church-Turing sea equivalente a esta interpretación, aunque Turing negó dicha coincidencia.  
    **Los estudios actuales sugieren que este enunciado es falso**, puesto que no es posible capturar todas las formas de computación tanto existentes como posibles mediante un algoritmo.   
    Por ejemplo, los protocolos interactivos no son algoritmos.
    
* **Tesis de Church-Turing Extendida (ECT):**
    
    Esta tesis afirma que *"la máquina de Turing es tan eficiente como un computador"*.   
Es decir, si alguna función es computable por algún dispositivo hardware para una entrada de tamaño n, entonces dicha función es computable por una máquina de Turing en *T(n)k* para algún *k* fijo (dependiente del problema).


####Implicaciones.
Tras estudiar en profundidad la tesis de Church-Turing, nos encontramos con que existen diversas implicaciones filosóficas bastante interesantes e importantes. Además, podemos encontrar cuestiones que nos permiten vincular la tesis de Church con la física y con la construción de hipercomputadoras.

___
##Detractores a la tesis de Church-Turing
___
La tesis de Church-Turing no es un teorema y por tanto no debe ser aceptada como válida, sin embargo no se ha encontrado nada que indique su falsedad ya que la tesis se utiliza como teorema actualmente y todo funciona correctamente.  

Es claro que es más "fácil" probar la falsedad de la tesis que la verdad de la misma. Basta con exponer un método efectivo o algoritmo que no sea computable en el sentido de Turing (es decir Turing-computable).

Aunque exponer un algoritmo que no sea Turing-computable no es tan fácil, pero, es más "fácil" que probar la verdad de la tesis, ya que parece imposible negar que sea verdadera a pesar de que eso es una posibilidad lógica.

Existe una tesis relativizada de Church-Turing que depende de los grados de Turing definidos por máquinas de Turing con *oráculos*. Los oráculos son medios formales que suponen que se le facilita cierta información a la máquina de Turing para resolver algún problema, esto define una jerarquía que se ha estudiado tanto en la teoría de la Computabilidad como en la **Teoría de la Complejidad**.

######Bibliografía:
[Tesis de Church-Turing (Wikibooks)](http://es.wikibooks.org/wiki/La_tesis_de_Church-Turing/TextoCompleto#Enunciado_de_la_tesis_de_Church)