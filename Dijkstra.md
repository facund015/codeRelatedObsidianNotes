### Facundo Vecchi A01283666

##### Ejercicio 1
###### Tabla de distancias
|     |  1  |  2  |  3  |  4  |
|:---:|:---:|:---:|:---:|:---:|
| A-A |  0  |  0  |  0  |  0  |
| A-B | inf | 10  |  7  |  7  |
| A-C | inf |  3  |  3  |  3  |
| A-D | inf | inf | 11  |  9  |
| A-E | inf | inf |  5  |  5  |

| Node | Shortest Distance |    Path    |
|:----:|:-----------------:|:----------:|
|  B   |         7         |  A->C->B   |
|  C   |         3         |    A->C    |
|  D   |         9         | A->C->B->D |
|  E   |         5         |  A->C->E   |


##### Ejercicio 2

###### Tabla de distancias
|     |  1  |  2  |  3  |  4  |  5  |  6  |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| A-A |  0  |  0  |  0  |  0  |  0  |  0  |
| A-B | inf |  2  | inf |     |     |     |
| A-C | inf | inf |  3  |     |     |     |
| A-D | inf |  1  |  1  |     |     |     |
| A-E | inf | inf |     |     |     |     |
| A-F | inf | inf |     |     |     |     |
| A-G | inf | inf |     |     |     |     |

| Node | Shortest Distance | Path |
|:----:|:-----------------:|:----:|
|  B   |                   |      |
|  C   |                   |      |
|  D   |         1         | A->D |
|  E   |                   |      |
|  F   |                   |      |
|  G   |                   |      |
