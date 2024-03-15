# Unifor - RLA
## lista de exercícios
### 1 - Calculo de média
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite as notas:}}
B --> C[/N1, N2, N3, N4/]
C --> D["media = (N1 + N2 + N3 + N4) /4"]
D --> E{{media}}
E --> F([Fim])
```  
#### Pseudocódigo
```
1 ALGORITIMO CalMedia
2 DECLARE N1, N2, N3, N4
		  media
3 INICIO
4 ESCREVA Digite as notas:
5 LEIA N1, N2, N3, N4
6 media ← (N1 + N2 + N3 + N4) /4
7 ESCREVA media
8 FIM
```
#### TESTE
| N1 | N2 | N3 | N4 | media | saida |
|--- |--- |--- |--- |--- |--- |
|5.0|5.5|7.0|6.0|5.8|"média = 5.8"
|4.0|15.0|9.0|26.0|27.0|"média = 27.0"
|6.0|6.0|6.0|6.0|6.0|"média = 6.0"

### 2 - Celsius para Fahrenheit
```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite a temperatura em Celsius(C):"}}
B --> C[/celsius/]
C --> D[fahrenheit = celsius * 1.8 + 32]
D --> E{{fahrenheit}}
E --> F([Fim])
```
#### Pseudocódigo
```
1	ALGORITIMO CelsiusFahrenheit
2	DECLARE celsius
			fahrenheit
3   INICIO
4   ESCREVA Digite a temperatura em celsius(C):
5 	LEIA celsius
6 	fahrenheit ← celsius * 1.8 + 32
7 	ESCREVA fahrenheit
8 	FIM
```

### 3 - Calculadora
```mermaid
flowchart TD
A([Inicio]) --> B{{Digite um número}}
B --> C[/n1/]
C --> D{{"escolha um operador: (+,-,*,/) "}}
D --> E[/operador/]
E --> F{{digite o segundo número}}
F --> G[/n2/]
G --> H{"operador === +"}
G --> I{"operador === -"}
G --> J{"operador === *"}
G --> K{"operador === /"}

H --> O[resultado = n1 + n2]
I --> P[resultado = n1 - n2]
J --> Q[resultado = n1 * n2]
K --> R[resultado = n1 / n2]

O --> Z([resultado])
P --> Z([resultado])
Q --> Z([resultado])
R --> Z([resultado])
Z --> ZZ([Fim])
```

