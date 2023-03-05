# Reto #4
Algoritmos

## Números primos hasta n

A continuación se presentará el pseudocódigo propuesto por mi persona para obtener números primos.
```sh
[variables]
n : entero
i : entero
x: entero
inicio
  i: = 2
  mientras (i < n)
    If (i < n**0.5) hacer
      (residuo de n/i)
         If hay residuo de n/i
           (n no es un número primo)
         else hacer
           (i = i + 1)
         Fin mientras  
    else
      (n es un número primo)
fin      
```

Ahora el algoritmo presentado anteriormente para hallar números primos se mostrará en forma de diagrama de flujo
```mermaid
flowchart TD
    A(Hallar número primo) --> B[n = 2]
    B --> C[i < n]
    C --> D{i < n**0.5}
    D --> |no| P(fin)
    D --> |si| E[i = 2]
    E --> H{residuo de n/i = 0}
    H --> |no| L[n es un número primo]
    H --> |si| K[n no es un número primo]
    C --> M[n = n + 1]
    L --> M
    K --> M
```

## Hallar raíz cuadrada

Para hallar la raíz cuadrada de un número se debe realizar el siguiente proceso, expresado a continuación mediante un pseudocódigo de Markdown.

```sh
[variables]
x : entero 
i : entero
z : float
inicio
 print x ("Ingrese un número positivo")
 hacer if len(lista_cifras) % 2!= 0 #agrupamos de a dos las cifras del número x
 hacer i (número que el cuadrado se aproxime al primer par sin pasarse)
 escribir (2 * i) #en nuevo renglón
 par_actual = concatenar(num1, num2)  // formar el siguiente par de dígitos
 resultado = x * (x + 1)
   Si (no hay residuo) entonces
     (z) encontrado #hallamos la raíz
   else
   mientras (condición no se cumpla) hacer
     instrucciones a repetir
```
