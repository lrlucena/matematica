# Definições, Conjecturas e Contra-exemplos

## Definição

```python
## a divide b (a|b) se existe n tal que a*n = b
def divide(a, b: Inteiro): Lógico = 
  para n de -100 até 100
    se a * n == b
    gere n
  fim.tamanho > 0

## a é par se 2|a
def par(a: Inteiro): Lógico = divide(2, a)
```

> Execute no terminal `potigol definicoes.poti`

## Conjectura

```python
# Conjectura de Goldbach
# Todo número par maior que 2 pode ser escrito como a soma de dois números primos.
escreva "Conjectura de Goldbach"
para n de 4 até 20 passo 2 faça
  para i em primos, j em primos faça
    se i <= j e n == i + j então
      escreva "{n} = {i} + {j}"
    fim
  fim
fim
```

> Execute no terminal `potigol conjectura.poti`

## Contra-Exemplo

### Afirmação

`n² + n + 41` é um número primo para qualquer n >= 0.

Como achar um contra-exemplo? Escrevendo um programa que teste vários valores de n até encontrar um valor que torne a afirmação falsa.

```python
para n de 1 até 30 faça  # até 50
  a = n * n + n + 41
  # procurando um contra-exemplo
  se não primo(a) então
    escreva "Achei um contra-exemplo!"
    escreva "n = {n}, {n}² + {n} + 41 = {a} não é primo"
  fim
fim
```

> Execute no terminal `potigol contra_exemplo.poti`
