https://www.cpcjudge.com/problem/quatroq

# D31O25. ¿Cuatro qué? 😡
#### Autores: Tourist, Ignacio_benq

## Descripción
Ese Maullin, como ya está conociendo el mundo después de su fuga, acaba de ver la película de *Los 4 Impresionantes*. Ahora, cualquier número que ve quiere saber si es múltiplo de 4.

## Entrada
En la primera línea, un número $N$ $(1 \leq N \leq 1000)$.

## Salida
Imprimir **"CUATRO"** si el número es divisible entre 4, de otro modo, imprimir **"NO"**

## Ejemplo

### Entrada
```
10
```
### Salida
```
NO
```
### Entrada
```
16
```
### Salida
```
CUATRO
```


## Temas identificados
### Matemáticas
- Divisibilidad.
- Múltiplos de 4.
- Operación módulo.

### Programación
- Operador módulo %.
- Estructuras condicionales.
- Entrada y salida.

## Propuesta de solución
#### Autor: mae
Se debe verificar si el número recibido es divisible entre 4. Para ello, se puede obtener el residuo de dividir $N$ entre 4. Si el residuo es 0, el número es múltiplo de 4 y se imprime `CUATRO` de lo contrario, se imprime `NO`.

## Implementación
Se lee el número $N$ y se utiliza el operador % para obtener el residuo de su división entre 4. Con un if se verifica si el resultado es 0 y se imprime la respuesta correspondiente.


### C++

#### Autor: mae
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    int n;
    cin >> n;

    if ( n % 4 == 0 ){
    cout << "CUATRO";
    }
    else
        cout << "NO";

    return 0;
}
```
