# Unifor - RLA
## lista de exercícios
### 1 - Calculo de média
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite as notas}}
B --> C[/N1, N2, N3, N4/]
C --> D["media = (N1 + N2 + N3 + N4) /4"]
D --> E{{media}}
E --> F([Fim])
```  

### 2 - Celsius para Fahrenheit
```mermaid
flowchart TD
A([INICIO]) --> B{{"Digite a temperatura em Celsius(C)"}}
B --> C[/temp/]
C --> D[fahrenheit = temp * 1.8 + 32]
D --> E{{fahrenheit}}
E --> F([Fim])
```
### 3 - Polegadas para Milímetros
```mermaid
flowchart TD 
A([Inicio]) --> B{{Digite a quantidade de chuva em Polegadas}}
B --> C[/poleg/]
C --> D[resultado = poleg * 25.4]
D --> E{{resultado}}
E --> F([Fim])
```
### 4 - Custo de um carro
```mermaid
flowchart TD
A([Inicio]) --> B{{"Qual o valor do carro? (sem taxas)"}}
B --> C[/valorcarro/]
C --> D[/porcentdistribuidor = 0,12/]
D --> E[/porcentimposto = 0,45/]
E --> F[valor1 = valorcarro * porcentimposto] 
F --> G[valor2 = valorcarro * porcentdistribuidor]
G --> H[resultado = valorcarro + valor1 + valor2]
H --> I{{resultado}}
I --> J([fim])
```
### 5 - Número ao quadrado
```mermaid 
flowchart TD
A([INICIO]) --> B{{Digite um numero}}
B --> C[/N1/]
C --> D[resultado = N1 * N1]
D --> E{{resultado}}
E --> F([Fim])
```

### 6 - Cardápio de uma lanchonete
```mermaid
flowchart TD
A([Inicio]) --> B{{
```

### 7


### 20 - Calculadora 
```mermaid
flowchart TD
A([Inicio]) --> B{{digite um número}}
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
