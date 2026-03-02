---
title: Bucles
description: Scripts en Bash para la administración de linux
---

# 15. Bucles

Hasta ahora, las condiciones que hemos visto nos permiten ejecutar una serie de acciones diferentes según se cumpla una condición determinada, como por ejemplo que el valor de una variable sea 1, 2, 3, o 4, etc...

Lo que no sabemos hacer todavía es volver hacia atrás en un script. Siempre hemos ido hacia delante hasta que llegábamos al final del script, y este finalizaba. Pero podemos encontrarnos con la situación de que si el usuario no introduce una opción válida, podamos seguir preguntándole hasta que introduzca una opción que sí sea correcta, y de esa manera no tener que volver a ejecutar todo
el script otra vez.

Se puede decir que un bucle, es un conjunto de instrucciones que se repiten, es decir, cuando llega al final de esas instrucciones, vuelve a empezar desde el principio del conjunto. Normalmente, no queremos que esas instrucciones se repitan todo el tiempo, y nunca terminen, ya que en ese caso estaríamos hablando de un bucle infinito (siempre se repite y nunca terminará). Por ello, estableceremos una condición o conjunto de condiciones que se deberán cumplir si queremos que las instrucciones dentro del bucle se vuelvan a repetir, o no.

Ejemplo de un bucle infinito. Podemos observar como después de ejecutar todas las instrucciones vuelve a empezar desde el principio:

<div align="center">
    <img src="../img/bash/Bucle_Infinito.png" alt="Bucle infinito" width="30%" />
</div>

## 15.1. Estructura `While` (mientras)

Esta estructura establece un bucle dentro de si misma. Este bucle de instrucciones se repetirá siempre que la condición que pongamos sea cierta. Se puede decir que es como una estructura `if`, con la diferencia de que cuando termina, vuelve al principio a comprobar otra vez la condición una y otra vez hasta que esta no se cumpla.

La estructura while es así:

```bash
while [ condición ]
do
    # Instrucciones dentro del bucle
done
```
<div align="center">
    <img src="../img/bash/Bucle_WHILE.png" alt="Bucle infinito" width="50%" />
</div>

Como podemos observar, siempre que la condición sea cierta, se ejecutarán las instrucciones dentro del bucle una y otra vez, hasta que la condición sea falsa.

Esta condición nos puede servir para cuando detectamos un error, o que el usuario introduce una condición que no es válida y le queremos seguir insistiendo hasta que nos de una opción correcta.

Ejemplo:

```bash
#!/bin/bash
echo -n "¿Desea continuar (s/n)?: "
read resp

# Mientras que la respuesta sea diferente de “s” y de “n”, sigue preguntando
while [ $resp != "s" -a $resp != "n" ]
do
    echo "Respuesta no valida. ¿Desea continuar (s/n)?"
    read resp
done

if [ $resp = “n” ]
then
    exit
fi

# y en caso de pulsar s, seguiría la ejecución por aquí...
```

Otro uso que le podemos dar a esta estructura es el de repetir algo un número determinado de veces:

```bash
#!/bin/bash
repeticiones=3
i=0

# Mientras el contador sea menor que el total, repite
while [ $i -lt $repeticiones ]
do
    # Como la variable va de 0 a 2, le sumamos 1 al mostrarla
    # para que aparezcan números del 1 al 3
    echo "Repetición numero: " `expr $i + 1`
    #incrementamos en una unidad la variable i
    let i++
done
```

otro ejemplo: 

```bash
#!/bin/bash
echo "¿Cuantos directorios deseas crear?"
read total
num=1

# Si el número es mayor que el total, paramos de crear, mientras tanto, sí creamos.
while [ $num -le $total ]
do
    # Por si acaso existe el directorio, quitamos los mensajes de error
    mkdir dir${num} 2> /dev/null
    # incrementamos la variable num una unidad más para el siguiente directorio
    let num++
done

echo "Hemos creado $total directorios."
```

## 15.2. Estructura `for`

La estructura `for` funciona de manera similar a la estructura `while`, aunque está pensada para ser usada en casos más concretos (algo similar a lo que pasa con la estructura case con respecto a `if`). La estructura `if` se puede usar de dos maneras. La primera es la siguiente:

```bash
for variable in lista
do
    # Instrucciones dentro del bucle
done
```

Este bucle se repetirá siempre tantas veces como elementos haya en la lista. En cada repetición la variable utiliza para iniciar el bucle tomará como valor el siguiente elemento de la lista, así en la primera repetición tomará el valor del primer elemento de la lista y así sucesivamente.

Esta lista puede ser una lista de palabras o números. Si queremos agrupar texto para que por ejemplo, si ponemos un nombre y apellido vayan juntos y no sean elementos diferentes debemos agruparlos entre comillas:

```bash
for nombre in Francisco Martínez Juan López     # Se repetirá 4 veces (4 elementos)
for nombre in “Francisco Martínez” “Juan López” # Así es correcto, se repetirá 2 veces.
```

Podemos ver su uso en el siguiente ejemplo
```bash
#!/bin/bash

# Este bucle se repetirá 9 veces
for num in 1 2 3 4 5 6 7 8 9
do
    echo "Repetición número $num"
done

# Creamos los siguientes directorios
for dir in dir1 dir2 dir3 dir4 dir5
do
    if [ ! -e $dir ]
    then
        mkdir $dir
    fi
done

# Mostramos los parámetros recibidos
echo "Número de parámetros $#"
num=1
for param in $*
do
    echo "Parámetro $num: $param"
    let num++
done
```

También podemos añadir grupos de valores o **rangos**, si vamos a iterar por valores enteros:

Ejemplo: 

```bash
#!/bin/bash
for NUM in {1..10}
# Equivalente for NUM in `seq 1 10`
do
    echo Linea $NUM
done
```

--- 

Un **rango** se puede expresar con un número de inicio y un número de fin. Sin embargo, `Bash`, es lo suficientemente inteligente, como para interpretar que si el número de inicio, es mayor que el número de fin, lo que tiene que hacer es una cuenta regresiva. Así,

- `{1..1000}` contará de 1 a 1000 
- `{1000..1}` contará de 1000 a 1

Pero, no solo puedes decir que cuente de uno en uno, también le puedes definir paso. Así

- `{1..1000..2}` contará de 1 a 1000, pero, de dos en dos.
- `{1000..1..-2}`, lo mismo que en el caso anterior, pero de forma regresiva.

Por supuesto que además de ponerlo en un bucle `for`, también lo puedes utilizar directamente en un echo, por ejemplo,

```bash
echo {1..100..5}
```

---

Existe, sin embargo, otra forma de utilizar el bucle `for`. Esta otra forma es muy útil sobretodo cuando queremos hacer un contador, y queda más limpio que utilizando la estructura `while`:

```bash
for (( instr1; condición; instr2 ))
do
    # Instrucciones que se repiten hasta que condición sea falsa
done
```

<div align="center">
    <img src="../img/bash/Bucle_FOR.png" alt="Bucle infinito" width="50%" />
</div>

En esta estructura tenemos un bucle `for`, y encerrados entre un doble paréntesis una instrucción que se ejecutará justo antes de comenzar el bucle por primera vez (instr1), una condición que indicará si se ejecutan las instrucciones dentro del bucle o se terminará y una instrucción final que se ejecutará como última instrucción dentro del bucle (instr2). Se podría expresar así en *pseudocódigo*:

```
instr1
mientras condición=verdadera
    instrucciones dentro del bucle
    instr2
fmientras
```

> ***Importante***: las instrucciones y condiciones dentro del doble paréntesis se escriben de forma casi idéntica a las instrucciones cuando se utiliza el comando `let`. De esta manera, una condición de si un número es mayor que otro se escribirá `n1 > n2`, si se quiere comparar si dos números son iguales se escribirá `n1 == n2`, etc... (de forma idéntica a cuando se utiliza `let`)

**Comparativa contador con `for` y `while`**

Veamos un mismo ejemplo resulto con `for` y con `while`:

Versión `for`
```bash
#!/bin/bash
# Este bucle se repetirá 9 veces
for (( i = 1; i <= 9; i++ ))
do
    echo "Repetición número $i"
done
```

Version `ẁhile``
```bash
#!/bin/bash
# Este bucle se repetirá 9 veces
let "i = 1"
while [ $i -le 9 ]
do
    echo "Repetición número $i"
    let i++
done
```

En el ejemplo con `for`, realiza los pasos de forma idéntica a como los realiza en el ejemplo con `while`, pero sin embargo nos estamos ahorrando 2 líneas en el código del programa.

## 15.3. Ruptura de bucles: `break` y `continue`

Hasta ahora hemos visto que para salir de un bucle la condición de entrada en dicho bucle debe ser falsa, y además, sabemos que la instrucciones dentro del bucle se ejecutarán hasta el final antes de volver a repetirse.

Sin embargo, hay algunas ocasiones en las que podría interesarnos salir del bucle debido por ejemplo a un error o a una situación especial, sin esperar a que la condición de dicho bucle se evalúe a falso. En otras ocasiones podría interesarnos saltarnos alguna de las *iteraciones* (vueltas) del bucle y pasar a la siguiente. Para ello tenemos 2 instrucciones útiles:

- `break`: Esta instrucción al ejecutarse, nos hace salir del bucle donde nos encontramos. El resto de instrucciones dentro del bucle no se llegan a ejecutar y además ya no se comprueba la condición de continuidad de bucle, simplemente salimos de él.

    Aunque puede resultar bastante útil en ciertas ocasiones, siempre que se pueda es mejor utilizar la condición del bucle para salir de él. 

La instrucción `break` puede servirnos sobretodo para salir de un bucle al encontrar un error o algo inesperado y no pudiésemos seguir ejecutando el bucle con normalidad.

```bash
#!/bin/bash
encontrado=0

# Vamos a buscar el archivo 'arch' en una lista de directorios
for dir in dir1 dir2 dir3 dir4 dir5
do
    if [ -e ${dir}/arch ]
    then
        encontrado=1
        # Ya no tiene sentido seguir buscando
        break
    fi
done

if [ $encontrado -eq 0 ]
then
    echo "Archivo no encontrado"
else
    echo "Archivo encontrado en $dir"
fi
```

- `continue`: Esta instrucción, a diferencia de `break`, no termina el bucle, sino que se salta las instrucciones que haya desde la palabra continue hasta el final del bucle y pasa a la siguiente *iteración* (vuelta) del bucle. Esto nos puede resultar muy útil cuando queremos hacer algo con una lista de cosas pero tenemos algún tipo de excepción.

```bash
#!/bin/bash
echo -n "Introduce número máximo al que llegaremos: "
read nummax

echo -n "Introduce un número para que los números divisibles entre él no aparezcan: "
read divisor

for (( i = 1; i <= $nummax; i++ ))
do
    let "resto = $i % $divisor"
    if [ $resto -eq 0 ]
    then
        # Si es divisible nos saltamos el resto y pasamos al siguiente
        continue
    fi
    echo "$i "
done
```

Como se ha podido observar, la instrucción continue, en el caso de un bucle del tipo `for (( instr1; condición; instr2 ))`, no afecta a `instr2`, que se sigue ejecutando siempre al final del bucle.

> ***Importante***: aunque estas dos instrucciones nos pueden resultar muy útiles en varias ocasiones, no conviene abusar de ellas (sólo utilizarlas cuando de verdad se necesite), ya que podrían hacer el código del programa más difícil de entender al alterar el comportamiento normal de un bucle e introducir comportamientos no esperados.

