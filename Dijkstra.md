### Facundo Vecchi A01283666

##### Ejercicio 1
###### Tabla de distancias
|     |     |     |     |     |
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
|     |     |     |     |     |     |     | 
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| A-A |  0  |  0  |  0  |  0  |  0  |  0  |
| A-B | inf |  2  |  2  |  2  |  2  |  2  |
| A-C | inf | inf |  3  |  3  |  3  |  3  |
| A-D | inf |  1  |  1  |  1  |  1  |  1  |
| A-E | inf | inf |  3  |  3  |  3  |  3  |
| A-F | inf | inf |  9  |  8  |  6  |  6  |
| A-G | inf | inf |  5  |  5  |  5  |  5  |


| Node | Shortest Distance |    Path    |
|:----:|:-----------------:|:----------:|
|  B   |         2         |    A->B    |
|  C   |         3         |  A->D->C   |
|  D   |         1         |    A->D    |
|  E   |         3         |  A->D->E   |
|  F   |         6         | A->D->E->F | 
|  G   |         5         |  A->D->G   |


0.0.0. 1 1 1 1 1 1 0 0
0.0.0. 0 0 0 0 0 0 1 1
0.0.0.3

1 1 1 1 1 0 0 0
0 0 0 0 0 1 1 1
0.0.0.7