# String (Cadena de caracteres)

Ejemplo:

```
<?php

echo "esto es una cadena";

?>
```

Lo que se muestra en pantalla:

`esto es una cadena`


## Comillas simples o comillas dobles

### Comillas simples

Las comillas simples se utilizan cuando no se va a utilizar variables dentro de las cadenas de texto (String).

```
<?php

$x = "Firulais"

echo 'Hola $x';

?>

```
Lo que se muestra en pantalla:

`Hola $x`

### Comillas dobles
Las comillas dobles se utilizan cuando se quiere mostrar el contenido de la variable dentro de una cadena de texto.

```
<?php

$x = "Firulais"

echo "Hola $x";

?>

```
Lo que se muestra en pantalla:

`Hola Firulais`

## Longitud de una cadena de texto

Para utilizarlo:

```
<?php

echo strlen("Jose");

?>
```
Lo que se muestra en pantalla
`4`

## Contador de palabras

Para utilizarlo:

```
<?php

echo str_word_count("Jose Roberto");

?>
```
Lo que se muestra en pantalla
`2`

## Buscar un texto

Para utilizarlo:

```
<?php

echo strpos("Jose Roberto", "Roberto");

?>
```
Lo que se muestra en pantalla
`5`

## Modificar cadenas de texto

### Mayusculas
Para utilizarlo:

```
<?php

echo strtoupper("Jose Roberto");

?>
```
Lo que se muestra en pantalla
`JOSE ROBERTO`

### Minusculas
Para utilizarlo:

```
<?php

echo strtolower("Jose Roberto");

?>
```
Lo que se muestra en pantalla
`jose roberto`

### Remplazar una cadena de texto

Para utilizarlo:

```
<?php

echo str_replace("Roberto","Martinez","Jose Roberto");

?>
```
Lo que se muestra en pantalla
`Jose Martinez`

### Cadenas a la inversa

Para utilizarlo:

```
<?php

echo strrev("Jose Roberto");

?>
```
Lo que se muestra en pantalla
`otreboR esoJ`

### Las funciones trim(), rtrim(), ltrim() 

La función trim() sirve para poder eliminar caracteres a los extremos de las cadenas de texto. 

La función rtrim() sirve para poder eliminar caracteres del lado derecho de la cadena de texto.

La función ltrim() sirve para poder eliminar caracteres del lado izquierdo de la cadena de texto.


```
<?php
echo trim("   Jose Roberto    ");
echo trim("Jose Roberto", "Jo ");
echo ltrim("Jose Roberto","Jo" );
echo rtrim("Jose Roberto", "to");

?>
```
Lo que se muestra en pantalla
`Jose Roberto` // No se nota en html plano, pero si dentro de cajas de entradas
`se Robert`
`seRoberto`
`Jose Rober`

### Convertir una cadena de caracteres a arreglos

Para esto se utiliza la función explode()
```
<?php
$str1 = "Hola Mundo";
$str2 = explode(" ",$str1);
?>
```

` entonces ahora $str2[0] = Hola , $str2[1] = mundo `

### Concatenar cadenas de texto

Esto se logra mediante el uso de un punto o tambien se pueden usar camillas dobles 

```
<?php
$x1 = "Hola";
$x2 = "Mundo";

echo $x1." ".$x2;

echo "$x1  $x2"

?>
```
Lo que se muestra en pantalla
`Hola Mundo`
`Hola Mundo`
