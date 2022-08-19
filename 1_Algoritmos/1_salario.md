# Salario
Calcular los salarios mensuales de los empleados de una empresa,
sabiendo que éstos se calculan con base en las horas semanales
trabajadas y de acuerdo con un precio especificado por horas, si
se pasan de cuarenta horas semanales, las horas extraordinarias
se pagarán a razón de 1.5 veces la hora ordinaria.
## Entrada: 
    horasTrabajadas y precioPorHora
## Salida: 
    saliroSemanal
## Restricciones: 
    Las horasTrabajadas tienen que ser enteros positivos y precioPorHora tiene no puede ser negativo.
    si se pasan de cuarenta horas semanales, las horas extraordinarias se pagarán a razón de 1.5 veces la hora ordinaria.
## Proceso : Algoritm
***
1. Leer _horasTrabajadas_
2. __Si__ _horasTrabajadas_ > 0 __entonces__ paso 3 __SiNo__ Paso 1
3. Leer _precioPorHora_
4. __Si__ precioPorHora > 0 __entonces__ paso 5 __SiNo__ Paso 3
5. Calcular _horasExtras_, donde _horasExtras_ = horasTrabajadas - 40
6. __Si__ horasExtras > 0 __entonces__ Paso 7, __SiNo__ Paso 8
7. _salarioTotal_ = precioPorHora\*(40 + horasExtras*1.5)
8. _salarioTotal_ = precioPorHora*horasTrabajadas  
***
