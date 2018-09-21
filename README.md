# Python para iniciantes

Estes conteúdo é baseado nas aulas dos professores, [Andrey Masiero](https://github.com/amasiero) e [Fabio Versolatto](https://www.linkedin.com/in/fabio-versolatto-a9740ba4/?originalSubdomain=br).

## Requerido
Para executar os exemplos utilizados neste repositório você precisa ter o **Python** instalado localmente na sua maquína ou você pode executa-los através do site: [repl.it](https://repl.it)

## Primitivos
**Atenção** Sobre os tipos primitivos iremos focar somentes em 4, caso você tenha interesse em conhecer mais sobre os tipos primitivos acesse: [tipos primitivos](https://pt.wikibooks.org/wiki/Python/Conceitos_básicos/Tipos_e_operadores)

1. **String**: O tipo *string* são todos os valores que estão dentro de aspas simples ou duplas **ex: 'Hello', "World"**
2. **Inteiro**: O tipo *inteiro* são os números inteiros positivos e negativos **ex: 1, 2, -4**
3. **Float**: O tipo *float* são os números que possuem **ex: 1.1, 2.333, -4.147**
4. **Boolean**: O tipo *boolean* são os valores que possuem apenas duas posibilidades podendo ser verdadeiro ou falso  **ex: True e False**

## Declaração

Para declararmos uma varíavel em *python* é um processo muito simples e fácil, basta dar um nome para a varíavel e definir um valor com algum dos tipos primitivos listados acima

Exemplo 1:
```python
# Essa varíavel é do tipo primitivo STRING
nome = "Obi Wan Kenoby" 
```

Exemplo 2:
```python
# Essa varíavel é do tipo primitivo INTEIRO
idade = 32 
```

Exemplo 3:
```python
# Essa varíavel é do tipo primitivo FLOAT
altura = 1.75 
```
Exemplo 4:
```python
# Essa varíavel é do tipo primitivo BOOLEAN
vilao = False 
```

Exemplo 5:
```python
# Essa varíavel é do tipo primitivo BOOLEAN
heroi = True 
```

As varíaveis em **Python** é algo de extrema importância partindo da ideia que podemos atribuir qualquer valor a elas.

**Varíaveis na prática**

Exemplo 1:
```python
numero1 = 10
numero2 = 5
calcular = numero1 + numero2
resultado = calcular

print(resultado) # saída =  15
```

Exemplo 2:
```python
nome = "João"
sobrenome = "de Oliveira"
nomeCompleto = nome + " " + sobrenome
resultado = nomeCompleto

print(nomeCompleto) # saída =  João de Oliveira
```

## Capturando uma entrada do usuário no Python
Para capturarmos uma entrda do usuário iremos utilizar a função **input()** do **Python**, para isso iremos criar uma varíavel com o nome **entradaUsuario** e iremos atribuir a função **input()** a ela. 

**Observação:** A função **input()** receber como parâmetro uma mensagem para o usuário, o retorno da função **input()** no **Python** é do tipo primitivo **STRING**, então caso queira fazer a captura de um valor número é necessário fazer um conversão para o tipo **INTEIRO ou FLOAT**, mas não se preocupe iremos tratar disto logo à frente.

Exemplo:
```python
entradaUsuario = input('Informe o seu primeiro nome! ')
resultado = entradaUsuario
print(resultado) # saida = "o nome digitado pelo usuário"
```

## Funções
Funções no python são importantes para executarmos algumas tarefas e operações matemáticas.

**Atenção** Lembrando que este repositório é para ajudar os alunos de programação em python até um pequeno ponta pé inicial o sobre o assunto, caso você tenha interesse em conhecer mais sobre as Funções acesse: [Funções no python](https://wiki.python.org.br/PrincipiosFuncionais#Definindo_Fun.2BAOcA9Q-es_em_Python)

Para criarmos uma definição iremos fazer uso de uma palavra reservada do **Python** chamada **def** e o **nome** da sua função, veja logo abaixo como criar suas primeira função.

Exemplo:
```python
def digaSeuNome():
  print("Meu nome é Ronaldo!")
```

Uma função no python pode receber um parâmetro ou varios, e pode também não receber nenhum parâmetro como no exemplo acima, nos exemplos abaixo iremos mostrar a declaração de algumas funções recebendo 1 e 2 parâmetros.

**Atenção:** a quantidade de parâmetros que uma função irá receber depende estritamente a sua necessidade, não tendo assim um limite padrão ou minímo e mámixo para ela.


Exemplo 1:
```python
def informeSeuNome(nome):
  print("O seu nome é " + nome)

informeSeuNome("Thalita Silva")
```

Exemplo 2:
```python
def informeSeuNomeEDataNacimento(nome, dataNascimento):
  print("O seu nome é " + nome + " e sua da de Nascimento é " + dataNascimento)
   # saida = "O seu nome é Thalita Silva e sua da de Nascimento é 14/04/1500"

informeSeuNomeEDataNacimento("Thalita Silva", "14/04/1500")
```

## Operadores 
 
O **Python** assim como em outras liguagem de programação temos os operadores aritmeticos que são utilizado para a execução de operações matemáticas, dentre os operadores python acredito que entre os mais conhecidos estão os operadores abaixos:

### Aritmeticos

Operação      | Operador
------------- | ---------
adição        | +
subtração     | -
multiplicação | *
divisão       | /


O temos o menos conhecidos mas importantes também que são os operadores para exponenciação, obtenção da parte inteira de uma divisão, extração do módulo da divisão, conforme pode ser visto na tabela a seguir

Operação         | Operador
---------------- | ---------
exponenciação    | **
parte inteira	   | //
módulo           | %

Exemplos da ultilização de cada um deles

Exemplo:
```python
# adição
print(5 + 2)  # saida 7

# subtração
print(5 - 2)  # saida 3

# multiplicação
print(5 * 2)  # saida 10

# divisão
print(15 / 3 ) # saida 5

# exponenciação
print(2 ** 2)  # saida 32

# parte inteira
print(10 // 9)   # saida 1

# módulo ou mod
print(4 % 2)  # saida 0

```

### Lógicos

Descrição       | Operador
--------------- | ---------
Maior que       | >
Menor que       | <
Maior ou igual  | >=
Menor ou igual  | <=
Igual a         | ==
Deferente de    | !=

Exemplos da ultilização de cada um deles

Exemplo:
```python
# Maior que
print(5 > 2)  # saida True

# Menor que
print(5 < 2)  # saida True

# Maior ou igual
print(5 >= 6)  # saida False

# Menor ou igual
print(15 <= 3 ) # saida False

# Igual a 
print(2 == 2)  # saida True

# Diferente de 
print(2 != 2)  # saida false

```

## Condicional

Nas estruturas condicionais em **Python** temos os **if, elif, else** que são muito úteis na tomada de decição de uma tarefa.

### Simples
Nas condicionais simples temos apenas uma possibilidade de comparação para uma tomada de decisão.

Exemplo 1:

Digamos que estão somando dois valores e queremos ter certeza que o resultado seja maiso que **0**, podemos checar essa possibilidade com uma condicional bem simples como no código em python abaixo:

```python

soma = 10 + 5

if soma > 0:
  print("O resultado da soma é maior que zero")
else:
  print("O resultado da soma não é maior que zero")
```

Exemplo 2:

Digamos que estão verificando se o nome de uma pessoa está correto, podemos checar também com uma condicional bem simples como no código em python abaixo:
```python

nome = "Alexandre"

if nome == "Alexandre":
  print("O nome está correto!")
else:
  print("O nome está errado!")
```

### Composta
Nas condicionais composta temos comparar varias possibilidade para uma determinada decisão, mas não se assuste pois assim como as anteriores a implementação delas são bastantes simples.

Exemplo 1:

Imagine um cenário onde queremos identificar se o nome de uma pessoa está correto e se ela é maior de idade, para fazermos essa checagem usaremos um operador que ainda não foi visto por nós nesse guia para iniciantes que é o **and**


```python
nome = "Alexandre"
idade = 17

if nome == "Alexandre" and idade >= 18:
  print("O seu está correto e você é maior de idade")
else:
  print("O nome está errado ou você não é maior de idade!")
```

Exemplo 2:

Imagine um cenário onde temos que comparar se a idade de uma pessoa é maior que 18 e menor que 30 iremos fazer essa checagem usaremos o operador **or**


```python
idade = 25

if idade > 18 or idade < 30:
  print("Sua idade está dentro da faixa etária permitida")
else:
  print("Sua idade está fora da faixa etária permitida")
```


## O que é Algoritmo?
Algoritmo é o conjunto das regras e procedimentos lógicos perfeitamente definidos que levam à solução de um problema em um número finito de etapas.

**Exemplo de algoritmo**

Neste exemplo iremos mostrar como criar um algoritmo para somar os números definidos entrada A e B.
```
Inicio
  Ler: Número definido para A
  Ler: Número definido para B
  resultado Soma: A + B
  escrever: Mostrar resultado do calcúlo
fim
```
Escrevendo o mesmo algoritmo acima em **Python**.
```python
entradaA = int(input('Digite um número inteiro! '))
entradaB = int(input('Digite outro número inteiro! '))

resultado = entradaA + entradaB

print('O resultado dessa operação é: ', resultado)
```

Explicando o algoritmo acima passo a passo!
1. Estamos criando uma varíavel com o nome **entradaA**
2. Na varível **entradaA** definimos uma conversão dos valores recebidos no **input()** com o **int()**
3. Fazemos o mesmos passos para a **entradaB**
4. No varíavel do resultado iremos atribuir o calculo desta operação
5. No print estamos monstrando na tela do usuário o resultado da soma de dois números

## Contribuir
Caso você tenha interesse, faça um fork do projeto e ajude-nos a mater esse guia para iniciantes

## Autor
[Alexandre dos Santos Soares](https://github.com/alexandrejuk)
