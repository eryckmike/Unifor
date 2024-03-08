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
6 media → (N1 + N2 + N3 + N4) /4
7 ESCREVA media
8 FIM
```
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
1	ALGORITIMO CelsiusFahrenheit
2	DECLARE celsius
					  fahrenheit
3  INICIO
4  ESCREVA Digite a temperatura em celsius(C):
5 	LEIA celsius
6 	fahrenheit → celsius * 1.8 + 32
7 	ESCREVA fahrenheit
8 	FIM

### 3 - Polegadas para Milímetros
```mermaid
flowchart TD 
A([Inicio]) --> B{{Digite a quantidade de chuva em Polegadas:}}
B --> C[/poleg/]
C --> D[resultado = poleg * 25.4]
D --> E{{resultado}}
E --> F([Fim])
```
#### Pseudocódigo
1	 ALGORITIMO PolgMilm
2 	DECLARE poleg
					  resultado
3	 INICIO
4	 ESCREVA Digite a quantidade de chuva em Polegadas:
5 	LEIA poleg
6 	resultado → poleg * 25.4
7 	ESCREVA resultado
8	 FIM

### 4 - Custo de um carro
```mermaid
flowchart TD
A([Inicio]) --> B{{"Digite o valor do carro (sem taxas):"}}
B --> C[/valorcarro/]
C --> D[/porcentdistribuidor = 0.12/]
D --> E[/porcentimposto = 0.45/]
E --> F[valor1 = valorcarro * porcentimposto] 
F --> G[valor2 = valorcarro * porcentdistribuidor]
G --> H[resultado = valorcarro + valor1 + valor2]
H --> I{{resultado}}
I --> J([fim])
```
#### Pseudocódigo
1 ALGORITIMO CustoCarro
2 DECLARE valorcarro
					  porcentdistribuidor
					  porcentimposto
					  valor1
					  valor2
					  resultado
3 	     INICIO
4 	     ESCREVA Digite o valor do carro (sem taxas):
5	     LEIA valorcarro
6       porcentdistribuidor → 0.12
7	     porcentimposto → 0.45
8 		 valor1 → valorcarro * porcentimposto
9 		  valor2 → valorcarro * porcentdistribuidor
10	 resultado → valorcarro + valor1 + valor2
11    ESCREVA resultado
12    FIM

### 5 - Número ao quadrado
```mermaid 
flowchart TD
A([INICIO]) --> B{{Digite um numero:}}
B --> C[/N1/]
C --> D[resultado = N1 * N1]
D --> E{{resultado}}
E --> F([Fim])
```
#### Pseudocódigo
1	 ALGORITIMO NumQuad
2 	DECLARE N1
					  resultado
3	 INICIO
4	 ESCREVA Digite um numero:
5 	LEIA N1
6 	resultado → N1 * N1
7 	ESCREVA resultado
8	 FIM

### 6 - Cardápio de uma lanchonete
```mermaid
flowchart TD
A([Inicio]) --> B{{Quantidade de Hambúrgueres consumidos:}}
B --> C[/a/]
C --> D{{Quantidade de Cheeseburgers consumidos:}}
D --> E[/b/]
E --> F{{Quantidade de Porções de Fritas consumidas:}}
F --> G[/c/]
G --> H{{Quantidade de Refrigerantes consumidos:}}
H --> I[/d/]
I --> J{{Quantidade de Milkshakes consumidos:}}
J --> K[/e/]
K --> L[th = a * 3.00]
L --> M[tc = b * 2.50]
M --> N[tf = c * 2.50]
N --> O[tr = d * 1.00]
O --> P[tm = e * 3.00]
P --> Q[total = th + tc + tf + tr + tm]
Q --> R{{total}}
R --> S([Fim])
```
#### Pseudocódigo
1	 ALGORITIMO Lanchonete
2 	DECLARE a, b, c, d, e
					  th, tc, tf, tr, tm
					  total
3	 INICIO
4	 ESCREVA Quantidade de Hambúrgueres consumidos:
5	 LEIA a
6   ESCREVA Quantidade de Cheeseburgers consumidos:
7   LEIA b
8   ESCREVA Quantidade de Porções de Fritas consumidas:
9   LEIA c
10 ESCREVA Quantidade de Refrigerantes consumidos:
11 LEIA d
12 ESCREVA Quantidade de Milkshakes consumidos:
13 LEIA e
14 th → a * 3.00
15 tc → b * 2.50
16 tf → c * 2.50
17 tr → d * 1.00
18 tm → e * 3.00
19 total → th + tc + tf + tr + tm
20 ESCREVA total
21 FIM

### 7 - Calculo do salário final do vendedor
```mermaid 
flowchart TD
A([INICIO]) --> B[/salario = 500/]
B --> C{{Digite o nome do vendedor:}}
C --> D[/nome/]
D --> E{{Digite o número de carros vendidos:}}
E --> F[/numcarvndds/]
F --> G{{Digite o valor total de vendas:}}
G --> H[/valttlvnds/]
H --> I[resultado = salario + numcarvndds * 50 + valttlvnds * 0.05]
I --> J{{resultado}}
J --> K([Fim])
```
#### Pseudocódigo
1	 ALGORITIMO CalcSalario
2 	DECLARE salario
					  nome
					  numcarvndds
					  valttlvnds
					  resultado
3	 INICIO
4   salario → 500
5	 ESCREVA Digite o nome do vendedor:
6   LEIA nome
7   ESCREVA Digite o número de carros vendidos:
8   LEIA numcarvndds
9   ESCREVA Digite o valor total de vendas:
10 LEIA valttlvnds
11 resultado → salario + numcarvndds * 50 + valttlvnds * 0.05
12 ESCREVA resultado
11 FIM

### 8 - Calculo da média do aluno na disciplina RLA
```mermaid 
flowchart TD
A([INICIO]) --> B{{Digite o nome do aluno}}
B --> C[/nome/]
C --> D{{Digite as notas}}
D --> E[/N1, N2/]
E --> F["media = (N1*2 + N2*1) /3"]
F --> G{{media}}
G --> H([Fim])
```

### 9 - Ficha do usuário
```mermaid 
flowchart TD
A([INICIO]) --> B{{Digite o nome do aluno}}
B --> C[/nome/]
C --> D{{Digite o numero da matrícula}}
D --> E[/nummatricula/]
E --> F{{Digite a idade}}
F --> G[/idade/]
G --> H{{Digite o e-mail}}
H --> J[/email/]
J --> K{{"'Nome: ' + nome 'Matrícula: ' + nummatricula 'Idade: ' + idade 'E-mail:' + email"}}
K --> L([Fim])
```
### 10 - 
### 20 - Calculadora
```mermaid
flowchart TD
A([Inicio]) --> B{{Digite um número}}
B --> C[/n1/]
C --> D{{"escolha um operador: (+,-,*,/,//,%,**, **) "}}
D --> E[/operador/]
E --> F{{digite o segundo número}}
F --> G[/n2/]
G --> H{"operador === +"}
G --> I{"operador === -"}
G --> J{"operador === *"}
G --> K{"operador === /"}
G --> L{"operador === //"}
G --> M{"operador === %"}
G --> N{"operador === **"}
H --> O[resultado = n1 + n2]
I --> P[resultado = n1 - n2]
J --> Q[resultado = n1 * n2]
K --> R[resultado = n1 / n2]
L --> S[resultado= n1 // n2]
O --> Z([resultado])
P --> Z([resultado])
Q --> Z([resultado])
R --> Z([resultado])
Z --> ZZ([Fim])
```
