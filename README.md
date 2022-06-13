# EXPRESIONES REGULARES

Son patrones de cadena de caracteres que pueden representar una forma de filtrar datos iterables y pueden ser tan sencillas o complejas como podamos implementarlas. 

# Usos
Filtrar archivos csv para buscar telefono por indicativo, filtrar cadenas de numeros para  tarjetas bancarias etc.

## El caracter (.)
Las Cadenas de caracteres son conjuntos o filas de caracteres que pueden o no ser visibles.
* El caracter punto es un caracter universal que hace refencia a todos los caracteres en general sean letras, numeros, simbolos o espacios. Al usarlo en una expresion regular este seleccionara cada uno de los caracteres.

Ejemplos:

* Si pongo un . y despues un espacio me seleccionara todos los caracteres que preceden un espacio mas el espacio.
* Si pongo el espacio antes buscara los espacios y tambien seleccionara el caracter que le sigue.
* podemos ademas de usar el espacio otros caracteres
* Si repetimos el punto le estaremos indicando la cantidad de caracteres juntos que queremos que encuentre en una sola linea.
En este caso se argupara la seleccion de caracteres por las unidades de puntos que halla.

## Las Clases predefinidas construidas

* \d ---> Solo selecciona digitos numericos. Al igual que con (.) si lo repetimos le estaremos diciendo la cantidad de digitos que debe encontrar juntos por linea.
* \w ---> Selecciona elementos de una palabra podrian ser digitos numericos y letras del alfabeto mayusculas y minusculas.
* \s busca solo espacios en blanco
* Las clases equivalentes las podemos usar con corchetes.
* [0-9]     indica el rango de digitos numericos del 0 al nueve equivalente a \d con la diferencia que podemos modificar el rango.
*[a-z] caracteres de la (a) a la (z) minuscula
*[A-Z] caracteres de la A a la Z mayuscula_
*[] dentro de los corchetes podemos agregar tantos simbolos como queramos seleccionar si queremos usar un caracter especial para poder escaparlo usamos el simbolo diagonal invertida ( \ ) de esta forma podemos usar el punto como caracter de busqueda y no de clase.

* IMPORTANTE: la clase \d debe ser obligatoriamente mayuscula.

    