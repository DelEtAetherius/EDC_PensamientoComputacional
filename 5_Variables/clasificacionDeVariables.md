# Clasificación de variables
## Constantes
Una constante es un dato númerico o alfanumérico que no cambia durante la ejecución del programa.  

Ejemplo:
```Java
// LAS CONSTANTES SE COLOCAN EN MAYÚSCULAS
double PI = 3.1416;
int PORT = 3306;
String CONECT_DB = "jdbc:mysql://localhost:"+PORT+"/miBaseDeDatos";
```

## Variables
Es un espacio en la memoria de la computadora que permite almacenar temporalmente un dato y su contenido puede cambiar durante la ejecución.  

Ejemplo:
```Java
// radio y area son variables, PI constante
double area = PI*radio^2;
// h, c1 y c2 son variables
int h = sqrt(c1^2+c2^2);

```

# Clasificación de las variables
* Variables
    * Por su contenido
        * Númericas
        * Lógicas
        * Alfanuméricas (String)
    * Por su Uso
        * De trabajo
        * Contadores
        * Acumuladores

## Por su contenido
### Variables Numéricas
Son aquellas en las cuales se almacenan valores numéricos (Reales o Enteros), positivos o negativos.  

Ejemplo:  
```Java
double g = 9.8; 
double pi = 3.1416; 
float costo = 2500.00;
int edad = 25;
```

### Variables Lógicas
Son aquellas que solo pueden tener dos valores (cierto o falso) estos representan el resultado de una comparación entre otros datos.

Ejemplos:
```Java
boolean comp = 3>5;
boolean acceso = (pass == passDB) && (user == userDB);
```

### Variables Alfanuméricas
Esta formada por caracteres alfanuméricos (letras, números y caracteres especiales).

Ejemplo:
```Java
String camelCase = "SoyUnaVariable"
String l3e7 = "$0yUn4V4r146l3 #014MUD0"

```

## Por uso
### Variable de trabajo
Variables que reciben el resultado de una operación matemática completa y que se usan normalmente dentro de un programa.
```Java
 double suma = a +b/c;
 double perimetro = l*4;
```
### Contadores
Se utilizan para llevar el control del numero de ocasiones en que se realiza una operación o se cumple una condición. Con los incrementos generalmente de uno en uno( aun que los incrementos pueden ser mayores o menores a cero pero siempre Enteros).

Ejemplo:
```Java
 int cont = 0
 cont = cont + 1;
 int cont2 = 0
 cont2 = cont2 + 2;
 cont++;
 cont2+=2;
 // negativos
 int cont3 = 0;
 cont3 = cont3 - 1;
 int cont4 = 0;
 cont4 = cont4 - 2;
 cont3--;
 cont4-=2;
``` 
### Acumuladores
Forma que toma una variable y que sirve para llevar la suma acumulativa de una serie de valores que se van leyendo o calculando progresivamente.

Ejemplo:
```Java
 int acum = 0;
 int n = 5;
 acum = acum + n;
 n = 48;
 acum = acum + n;
 n = 78;
 acum+=n;
```