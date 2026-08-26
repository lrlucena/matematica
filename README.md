# Matemática Discreta

Clique no botão para abrir o ambiente de execução do Codespace

[![Execute direto no GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/lrlucena/matematica?quickstart=1)

https://github.com/codespaces/new/lrlucena/matematica?quickstart=1



## 1. Técnicas de Demonstração

### Definições

Definição: Um número inteiro `a` divide um número inteiro `b` quando existir um número inteiro `n` tal que `a x n = b`.

```python
def divide(a, b: Inteiro): Lógico = 
  para n de -100 até 100
    se a * n == b
    gere n
  fim.tamanho > 0
```

### Conjecturas

**Conjectura de Goldbach**: 
Todo número par maior que 2 pode ser escrito como a soma de dois números primos.

O programa a seguir testa se a conjectura é válida para os números pares de 4 até 100
```python
para n de 4 até 100 passo 2 faça
  para i em primos, j em primos faça
    se i <= j e n == i + j então
      escreva "{n} = {i} + {j}"
    fim
  fim
fim
```

### Contra-Exemplos

Objetivo: encontrar um contra-exemplo que mostre que uma afirmação é falsa.

**Afirmação**: 
`n² + n + 41` é um número primo para qualquer n >= 0.

Como achar um contra-exemplo? Escrevendo um programa que testa vários valores de n até encontrar um valor de `n` que quando aplicado à expressão não gera um número primo.

```python
para n de 0 até 30 faça  # até 50
  a = n * n + n + 41
  # procurando um contra-exemplo
  se não primo(a) então
    escreva "Achei um contra-exemplo!"
    escreva "n = {n}, {n}² + {n} + 41 = {a} não é primo"
  fim
fim
```

## 2. Conjuntos

## 3. Relações

## 4. Funções

