https://www.cpcjudge.com/problem/lametamorfosisgmail

# D14O25. La metamorfosis de Gmail (el perrito)
#### Autor: Crocubot

## Descripción
Una mañana, tras un sueño intranquilo, Gmail (el perrito) se despertó convertido en un programador...

Gmail (el perrito) tenía pensado practicar antes de ir a la clase del campamento de otoño de programación, pero como se le hizo tarde, pensó en un número $X$ y un número $Y$ y te pidió determinar lo siguiente.

- Si $X$ es divisible por $Y$ o no.
- Si $X$ es mayor, menor o igual que $Y$.
- Y si el residuo de $X$ entre $Y$ es par o impar.

## Entrada
Dos enteros $X$ y $Y$ $(1 \leq X, Y \leq 100)$.

## Salida
- En la primera línea imprime "X es divisible por Y" o "X no es divisible por Y" según sea el caso.
- En la segunda línea imprime "X es mayor que Y", "X es menor que Y" o "X es igual que Y" según sea el caso.
- En la tercera línea imprime "El residuo es par" o "El residuo es impar" según sea el caso.


## Ejemplo

### Entrada
```
10 5
```
### Salida
```
X es divisible por Y
X es mayor que Y
El residuo es par
```
### Entrada
```
8 3
```
### Salida
```
X no es divisible por Y
X es mayor que Y
El residuo es par
```
### Entrada
```
1 100
```
### Salida
```
X no es divisible por Y
X es menor que Y
El residuo es impar
```
### Entrada
```
21 21
```
### Salida
```
X es divisible por Y
X es igual que Y
El residuo es par
```

## Temas identificados
### Matemáticas
- Divisibilidad.
- Comparación de números.
- Residuo de una división.
- Números pares e impares. 

### Programación
- Operador módulo %.
- Estructuras condicionales.
- Comparación de valores.
- Entrada y salida de datos.

## Propuesta de solución
#### Autor: mae
Se deben realizar tres comprobaciones independientes: determinar si $X$ es divisible entre $Y$, comparar ambos números para saber si $X$ es mayor, menor o igual que $Y$ y verificar si el residuo de la división es par o impar.

## Implementación
Se leen $X$ y $Y$. Se calcula el residuo con % y se utilizan estructuras if para determinar la divisibilidad, para comparar si es mayor, menor o igual y saber si el residuo es par o impar.

### C++

#### Autor: mae
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int x, y;
    cin >> x >> y;

    if (x % y == 0){
        cout << "X es divisible por Y" << '\n';
    } else {
        cout << "X no es divisible por Y" << '\n';
    }

    if (x > y){
        cout << "X es mayor que Y" << '\n';
    } else if (x < y) {
        cout << "X es menor que Y" << '\n';
    } else {
        cout << "X es igual que Y" << '\n';
    }

    if ((x % y) % 2 == 0){
        cout << "El residuo es par" << '\n';
    } else {
        cout << "El residuo es impar" << '\n';
    }


return 0;
}
```
