# Unifor - RLA
## lista de exercícios - AULA 3
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
2 DECLARE N1, N2, N3, N4 : INTEIRO
		  media
3 INICIO
4 ESCREVA Digite as notas:
5 LEIA N1, N2, N3, N4
6 media ← (N1 + N2 + N3 + N4) /4
7 ESCREVA media
8 FIM_CalMedia
```
#### TESTE
| N1 | N2 | N3 | N4 | media | SAIDA |
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
2	DECLARE celsius :INTEIRO
		fahrenheit
3   INICIO
4   ESCREVA Digite a temperatura em celsius(C):
5 	LEIA celsius
6 	fahrenheit ← celsius * 1.8 + 32
7 	ESCREVA fahrenheit
8 	FIM_CelsiusFahrenheit
```
#### TESTE
| celsius | fahrenheit | SAIDA | 
|--- |--- |--- |
|16|60.8|"Em Fahrenheit: 60.8"|
|-10|14.0|"Em Fahrenheit: 14.0"|
|32|89.6|"Em Fahrenheit: 89.6"|

### 3 - Calculadora
```mermaid
flowchart TD
A([Inicio]) --> B{{Digite um número:}}
B --> C[/n1/]
C --> D{{"Escolha um operador: (+,-,*,/) "}}
D --> E[/operador/]
E --> F{{digite o segundo número:}}
F --> G[/n2/]
G --> H{"operador === +"}
G --> I{"operador === -"}
G --> J{"operador === *"}
G --> K{"operador === /"}

H --> O[resultado = n1 + n2]
I --> P[resultado = n1 - n2]
J --> Q[resultado = n1 * n2]
K --> R[resultado = n1 / n2]

O --> Z{{resultado}}
P --> Z{{resultado}}
Q --> Z{{resultado}}
R --> Z{{resultado}}
Z --> ZZ([Fim])
```
#### Pseudocódigo
```
1	ALGORITIMO CalculadoraSimples
2	DECLARE n1, n2 :INTEIRO
			operador
			resultado
3   INICIO
4   ESCREVA Digite um número:
5	LEIA n1
6	ESCREVA Escolha um operador: (+,-,*,/)
7 	LEIA operador
8 	ESCREVA digite o segundo número:
9 	LEIA n2 
10 	SE operador === + ENTAO
11		resultado = n1 + n2
12		SE SENAO operador === - ENTAO
13			resultado = n1 - n2
14				SE SENAO operador === * ENTAO
15					resultado = n1 * n2
16 						SE SENAO operador === / entao
17							resultado = n1 / n2
18	ESCREVA resultado
19	FIM_CalculadoraSimples
```
#### TESTE
| n1 | operador | n2 | resultado | SAIDA |
|--- |--- |--- |--- |--- |
|5|*|3|15|"resultado: 15|
|9|/|3|1|"resultado: 1"|
|9|+|-2|7|"resultado: 7"|
|11.5|-|1.2|10|"resultado: 10.3"|

### 4 - Classificar idade
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite a idade:}}
B --> C[/idade/]
C --> D{idade >= 5 or idade <= 7}
D --TRUE--> E{{Infantil A}}
D --FALSE--> F{idade >= 8 or idade <= 10}
F --TRUE--> G{{Infantil B}}
F --FALSE--> H{idade >= 11 or idade <= 13}
H --TRUE-->  I{{Juvenil A}}
H --FALSE--> J{idade >= 14 or idade <= 17}
J --TRUE--> Q{{Juvenil B}}
J --FALSE--> K{idade >= 18}
K --TRUE--> L{{Adulto}}
K --FALSE--> M{{Invalido}}
E --> Z([Fim])
G --> Z
I --> Z
Q --> Z
L --> Z
M --> Z
```
#### Pseudocódigo
```
1	ALGORITIMO ClassificarIdade
2	DECLARE idade
3   INICIO
4   ESCREVA Digite a idade:
5	LEIA idade
6	SE idade >= 5 or idade <= 7 ENTAO
7 		ESCREVA Infantil A
8 		SE SENAO idade >= 8 or idade <= 10 ENTAO
9 			ESCREVA Infantil B
10 			SE SENAO idade >= 11 or idade <= 13 ENTAO
11				ESCREVA Juvenil A
12				SE SENAO idade >= 14 or idade <= 17 ENTAO
13					ESCREVA Juvenil B
14					SE SENAO idade >= 18 ENTAO
15						ESCREVA Adulto
16 					SENAO 
17					ESCREVA Inválido 
18	FIM_ClassificarIdade
```
#### TESTE
| idade | idade >= 5 or idade <= 7 | idade >= 8 or idade <= 10 | idade >= 11 or idade <= 13 | idade >= 14 or idade <= 17 | idade >= 18| SAIDA
|--- |--- |--- |--- |--- |--- |--- |
|5|T|F|F|F|F|Infantil A
|9|F|V|F|F|F|Infantil B
|19|F|F|F|F|V|Adulto
|15|F|F|F|V|F|Juvenil B
