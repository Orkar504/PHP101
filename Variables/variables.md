# Las variables

Las variables en PHP no son necesarias, ya que es un Lenguaje no tipado

```
<?php
$nVar = 65
$_Var = "variable"
?>
```

Pero los nombres de las variables dependen del Tamaño de la letra

```
# '!=' significa no es igual
# $nVar != $NVar no son lo mismo
```
## Alcance de las variables
En PHP tenenmos tres tipos de alcance:

- local     (local)
- global    (global)
- static    (estática)
### global
Son las variables declaradas afuera de toda función

#### El arreglo de variables globales
Las variables globales son almacenadas en un arreglo 
`$GLOBALS[]`
### local
Las variables locales son aquellas que estan dentro de las funciones, por ende no pueden ser referenciadas fuera de estas.
### estática
En las funciones de PHP cuando terminan su procesamiento las variables son eliminadas de memoria, debido se requiere una solución para guardar las variables, es ahí donde esntran las variables estáticas y se declaran así:

`static $var = 1`


## Tipos de datos
En PHP tenemos los siguientes tipos de datos:

- String    (cadena de caracteres)
- Integer   (un entero)
- Float     (entero con decimal)
- Boolean   (booleanos)
- Array     (arreglos)
- Object    (objetos)
- NULL      (nula)
- Resource

Para saber que tipo de datos es una variables se utiliza lo siguiente:

`var_dump($var)`
