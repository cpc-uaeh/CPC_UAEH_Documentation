https://www.cpcjudge.com/problem/queremoscalavera

# D13O25. ¡Queremos calavera!
#### Autor: ash_c4t

## Descripción
Los papás de Fido y Bartolomeo los llevaron a pedir calaverita por todo el vecindario. Al regresar a casa, los dos niños vaciaron sus bolsas para ver qué dulces habían recibido.
Sin embargo, sus papás solo les permitieron comer un dulce esa noche, con una condición: que ambos coman exactamente el mismo dulce.
Ayuda a Fido y a Bartolomeo a determinar si pueden comer su dulce.

## Entrada
En la primera línea una cadena $F$ $(1 \leq |F| \leq 20)$, el dulce que eligió Fido.

En la segunda línea una cadena $B$ $(1 \leq |B| \leq 20)$, el dulce que eligió Bartolomeo.

Cada cadena contiene únicamente letras minúsculas del alfabeto inglés $(a-z)$.

## Salida
Imprime $SI$ si ambos dulces son exactamente iguales, o $NO$ en caso contrario.

## Ejemplo

### Entrada
```
chocolate
chocolate
```
### Salida
```
SI
```
### Entrada
```
gomitas
caramelo
```
### Salida
```
NO
```

## Notas


## Temas identificados
### Matemáticas
- Comparación de cadenas.

### Programación
- Cadenas de caracteres.
- Comparación de strings.
- Entrada y salida estándar.
- Estructuras condicionales.

## Propuesta de solución
#### Autor: mae
Se deben comparar los dos dulces para verificar si son exactamente iguales. Si las cadenas coinciden, se imprime SI, de lo contrario, se imprime NO.


## Implementación
Se utilizan dos variables de tipo `string`, una para almacenar los dulces elegidos.

Se leen ambas cadenas mediante `cin` y posteriormente se utiliza el operador `==` para comprobar si son iguales.

Si la comparación devuelve verdadero, se imprime `SI`. En caso contrario, se imprime `NO`.


### C++

#### Autor: mae
```cpp
#include <bits/stdc++.h>

using namespace std;

int main()
{
    cin.tie(0); ios_base::sync_with_stdio(false);

    string f, b;
    cin >> f >> b;

    if (f == b){
        cout << "SI";
    } else
        cout << "NO";
    return 0;
}
```

