# Function scope js

## Objetivos

 Identificar las funciones globales, locales, funciones de callback, expresions, statement, clousure, scope, contextos de ejecucion, que funciones forman parte de la pila de ejecucion (stack execution) y que funciones forman parte de la cola de eventos (event queue).

## Funciones Globales

La siguiente es una función global:

~~~
$(document).ready(function() { ... })
~~~

## Funciones Locales

Las siguientes son funciones locales:

~~~
function activeButton() 
function desactiveButton()
function longitud(input)
function soloNumeros(input)
function isValidCreditCard(numberCard) 
~~~

## Funciones de callback

Dentro del manejador de evento input, se invoca a la función ` isValidCreditCard `, en este contexto, la función es una función de callback. 

## Funciones Statement

Las siguientes son funciones statement:

~~~
function activeButton() 
function desactiveButton()
function longitud(input)
function soloNumeros(input)
function isValidCreditCard(numberCard) 
~~~

## Funciones Expression

Las funciones expression son declaradas de la siguiente forma:

~~~
var hello = function() {
    console.log ('hola mundo');
}
~~~

No existe ninguna función expression.

## Scope

El scope es el alcance de una variable. Existen dos tipos, global y local.

Las siguientes son variables globales, ya que se puede acceder desde cualquier parte del código debido a que han sido definidas fuera de cualquier función.

~~~
var $inputCard 
var $inputMonth 
var $inputYear 
var $buttonNext 
var regexOnlyNumbers
var labelErrorOrSuccessMessages
~~~

Las siguientes son variables locales ya que se definieron dentro de alguna función y sólo podemos acceder a ellas dentro de dichas funciones.

~~~
var regex
var creditCardNumber
var arr
var sumaTotal
var index
~~~

## Closure

Un closure es una función libre de variables, un closure no tiene variables propias, pero las variables de una función padre pueden funcionar. Las siguientes son closures:

~~~
function activeButton() 
function desactiveButton()
function longitud(input)
~~~

## Funciones que forman parte de la pila de ejecución

~~~
$(document).ready(function() { ... }
console.log('Probar con el numero valido 4544164785372342');
~~~

## Funciones que forman parte de la cola de eventos

~~~
function activeButton() 
function desactiveButton()
function longitud(input)
function soloNumeros(input)
~~~
