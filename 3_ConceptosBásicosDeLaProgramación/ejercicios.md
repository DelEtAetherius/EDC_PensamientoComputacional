# Ejercicio en JavaScript
Realizar los siguientes algoritmos en javaScript
## Qué necesitas saber de javaScript
### Mostrar mensaje
Para mostrar un mensaje en consola se utiliza; <span style="color:#F92672 ">console.log\(</span>mensaje <span style="color:#F92672 ">\);</span> o un mensaje como alerta; <span style="color:#F92672 ">alert\(</span>mensaje <span style="color:#F92672 ">\);</span>
```javaScript
saludo = "Hola Mundo"
console.log(saludo);
// salida: Hola mundo
console.log("Hola mundo, otra vez");
// salida: Hola mundo, otra vez
console.log(saludo,"otra vez");
// salida: Hola mundo, otra vez

// Con alert()
alert(saludo);
alert("Hola mundo, otra vez");
alert(saludo+" otra vez");// el + no agrega espacios
```
### Leer un dato de entrada
Solicitar al usuario un dato de entrada y guardarla en una variable
```javaScript
// identificador = prompt("mensaje","valorDefault") valorDefault no es obligatorio
// como caracteres, (no son números)
saludo = prompt("Ingresa un saludo","Hola mundo");
// guardar como entero,(son número)
dato = parseInt(prompt("Ingresa un número","0"));
// guardar como real (punto decimal)
dato = parseFloat(prompt("Ingresa un número","0"));
```
### Cómo declarar una variable
Sólo tenemos que utilizar el operador de asignación " = "
```javaScript
a = 5;
b = 7;
// si no existe b o a, marcara un error
c = a + b; 
// todo lo que es cadena de caracteres(texto) se coloca entre comillas
saludo = "Hola Mundo";
```
### Potencias
Una forma de elevar un número al cuadrado en JavaScript es utilizar el método pow() de la biblioteca Math.
```javaScript
a = 5;
a2 = Math.pow(a,2); // 25
```
### Estructura condicional
Una estructura condicional nos ayudará a tomar una desición.
Ejemplo.
<span style="color:#F92672 ">Si</span> a = 20 <span style="color:#F92672 ">Entonces</span> a es mayor a 10, <span style="color:#F92672 ">Sino</span> a es menor o igual a  10  
```javaScript
if (a > 10) {
    console.log("a es mayor a 10");
}else{
    console.log("a es menor o igual a 10");
}
```
## Ejercicios
1. Escribir un programa que muestre por pantalla la cadena <span style="color:#AA115E">¡Hola Mundo!</span>.

    ```javaScript
    console.log("Hola Mundo");
    alert("Hola Mundo");
    ```

1. Escribir un programa que almacene la cadena <span style="color:#AA115E">¡Hola Mundo!</span> en una variable y luego muestre por pantalla el contenido de la variable
    ```javaScript
    saludo = "Hola Mundo"
    console.log(saludo);
    alert(saludo);
    ```
1. Escribir un programa que pregunte el nombre del usuario en la consola y después de que el usuario lo introduzca muestre por pantalla la cadena <span style="color:#AA115E ">¡Hola \<nombre\>!</span>, donde <span style="color:#AA115E">\<nombre\></span> es el nombre que el usuario haya introducido.
    ```javaScript
    nombre = prompt("Ingresa tu nombre:");
    console.log("Hola",nombre);
    alert("Hola "+nombre);
    ```
1. Escribir un programa que muestre por pantalla el resultado de la siguiente operación aritmética: $$\left(\frac{3+2}{2*5}\right)^2$$
    ```javaScript
    operacion = Math.pow(((3+2)/(2*5)),2);
    console.log(operacion);
    alert(operacion)
    ```
1. Escribir un programa que lea un entero positivo, _n_, introducido por el usuario y después muestre en pantalla la suma de todos los enteros desde 1 hasta _n_ . La suma de los *n* primeros enteros positivos puede ser calculada de la siguiente forma:  $$suma = \frac{n(n+1)}{2}$$
    ```javaScript
    n = parseInt(prompt("Ingresa un número:"));
    suma = (n*(n+1))/2;
    console.log(suma);
    alert(suma);
    ```
1. Escribir un programa que pida al usuario dos números enteros y muestre por pantalla la <span style="color:#AA115E ">n</span> entre <span style="color:#AA115E ">m</span> da un cociente <span style="color:#AA115E ">c</span> y un resto <span style="color:#AA115E ">r</span> donde <span style="color:#AA115E ">n y m</span> son los números introducidos por el usuario, y <span style="color:#AA115E ">c y r</span> son el cociente y el resto de la división entera respectivamente.
    ```javaScript
    n = parseInt(prompt("Ingresa el divisor"));
    m = parseInt(prompt("Ingresa el divividendo"));
    if (n != 0){
        c = parseInt(m/n);
        r = m%n
        console.log("n =",n,"\nm =",m,"\nc =",c,"\nr =",r);
        alert("n = "+n+"\nm = "+m+"\nc = "+c+"\nr = "+r);
    }else{
        console.log("Error el divisor es igual a cero");
        alert("Error el divisor es igual a cero");
    }
    ```
1. Calcular los salarios semanales de los empleados de una empresa,sabiendo que éstos se calculan con base en las horas trabajadas y de acuerdo con un precio especificado por horas, si se pasan de cuarenta horas semanales, las horas extraordinarias se pagarán a razón de 1.5 veces la hora ordinaria. [salario](../1_Algoritmos/1_salario.md)
    ```javaScript
    horasTrabajadas = parseInt(prompt("Ingresa horas trabajadas"));
    precioPorHora = parseFloat(prompt("Ingresa precio por hora"));
    horasExtras = horasTrabajadas - 40;
    if (horasExtras > 0){
        salarioTotal = precioPorHora*(horasExtras*1.5+40);
    }else{
        salarioTotal = precioPorHora*horasTrabajadas
    }
    console.log("El salario total = "+salarioTotal);
    alert("El salario total = "+salarioTotal);
    ```
