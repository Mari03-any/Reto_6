# Reto_6
Elaborado por: Maria Fernanda Parra Osorio_1014980661 <br>
Este reto se realizó en un notebook el cual está adjuntado en el repositorio
## Diagramas de Flujo 
Se realizaron diagramas de flujo para los tres primeros ejercicios
#### Ejercicio 1
```mermaid
flowchart TD
    A[ < bloque_prev> ] --> B(n = 1) --> c{while n <= 100}
    c -->|verdadero| D( print n, n**2 )
    c -->|Falso| E[ < bloque_siquiente> ]
    D --> F[ n += 1]
    F --> c
```
#### Ejercicio 2
```mermaid
flowchart TD
    A[ < bloque_prev> ] --> B(impar = 1) --> c{while impar <= 999}
    c -->|verdadero| D( print impar )
    c -->|Falso| E[ < bloque_siquiente> ]
    D --> F[ impar += 2]
    F --> c
    H[ < bloque_prev> ] --> I(par = 2) --> J{while par <= 1000}
    J -->|verdadero| K( print par )
    J -->|Falso| L[ < bloque_siquiente> ]
    K --> M[ par += 2]
    M --> J
```
#### Ejercicio 3
```mermaid
flowchart TD
    A[ if n >= 2 ] --> B(par = n )
    B --> C(if n % 2 == 0) --> E
    B --> D(else n - 1) --> E
    E{while par >= 2}
    E -->|verdadero| F( print par )
    E -->|Falso| G[ < bloque_siquiente> ]
    F --> H[ par -= 2]
    H --> E
```
