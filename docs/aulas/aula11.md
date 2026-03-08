---
title: "Aula 11 — Condições aninhadas: SE dentro de SE"
layout: default
---

## Antes de começar

Você já parou para pensar em como os aplicativos que você usa todos os dias fazem escolhas tão precisas? Como aquele app de notas na sua escola que lhe dá uma classificação baseada no seu desempenho. Hoje, vamos aprender sobre estruturas de decisão compostas - `if`, `elif` e `else` - que nos permitem criar condições mais complexas em nosso código.

## O que você vai aprender nesta aula

- Como construir condições mais complexas usando `if`, `elif` e `else`.
- A diferença entre `elif` e `else` e como usá-las para avaliar múltiplas condições.
- Como aplicar estruturas aninhadas em problemas práticos, como calcular o preço do frete.

## Compreendendo Estruturas de Decisão Compostas

Você já parou pra pensar em como os aplicativos que você usa todos os dias fazem escolhas tão precisas? Como aquele app de notas na sua escola que lhe dá uma classificação baseada no seu desempenho. Hoje, vamos aprender sobre estruturas de decisão compostas - `if`, `elif` e `else` - que nos permitem criar condições mais complexas em nosso código.

### Construindo Condições Mais Complexas

Quando você escreve um código com `if`, `elif` e `else`, está dizendo ao computador: "Se essa condição for verdadeira, faça isso. Se não, veja se esta outra condição é verdadeira. E se nenhuma delas for verdadeira, então faça isso aqui." É como fazer um fluxograma na sua cabeça para decidir o que vai acontecer com cada situação.

> 🤔 **Para refletir:** Como você usaria `if`, `elif` e `else` em um jogo onde diferentes níveis trazem recompensas diferentes?

Vamos criar um exemplo simples de sistema de classificação de notas:

```python
nota = 85

if nota >= 90:
    print("Sua classificação é A.")
elif nota >= 80:
    print("Sua classificação é B.")
else:
    print("Você precisa melhorar sua pontuação!")
```

Agora, faça uma versão desse código que considere mais níveis de classificação. Por exemplo, adicione a classificação 'C' para notas entre 70 e 79.

### Prática em Ação

Incorporando o que você acabou de aprender, agora é sua vez de criar um sistema onde diferentes faixas de pontuação resultam em diferentes letras de graduação. Tente adicionar mais condições ao código acima para uma classificação 'C' e talvez até mesmo uma 'D'.

---

E agora, **como você adaptaria essa lógica para avaliar a performance de atletas baseada nos seus tempos?**

## Diferença entre Elif e Else

Você já notou como apps de redes sociais tratam suas publicações diferentes, dependendo da hora do dia? Eles podem destacar posts feitos à noite ou durante o fim de semana. Hoje vamos aprender como a linguagem Python faz algo parecido com as estruturas condicionais `elif` e `else`.

### Elif: Condicional Adicional

Quando você quer testar mais condições além da primeira, é aí que entra o `elif`. Ele permite que você avalie várias possibilidades em sequência. Por exemplo:

```python
idade = int(input("Qual sua idade? "))
if idade < 18:
    print("Menor de idade")
elif idade >= 18 and idade <= 60:
    print("Adulto")
else:
    print("Idoso")
```

### Else: Resposta Padrão

E o `else` aparece quando não se encaixa em nenhuma condição anterior. É como um "caso padrão", uma resposta geral caso todas as outras condições falhem.

Vamos usar isso para construir um pequeno sistema que verifica a idade de um usuário com base na data de nascimento:

```python
from datetime import date

def calcular_idade(data_nascimento):
    hoje = date.today()
    idade = hoje.year - data_nascimento.year - ((hoje.month, hoje.day) < (data_nascimento.month, data_nascimento.day))
    return idade

data_nasc_str = input("Digite sua data de nascimento no formato YYYY-MM-DD: ")
ano, mes, dia = map(int, data_nasc_str.split('-'))
idade_usuario = calcular_idade(date(ano, mes, dia))

if idade_usuario < 18:
    print(f"Você é menor de idade e tem {idade_usuario} anos.")
else:
    print("Parabéns! Você é maior de idade.")
```

> 🤔 **Para refletir:** Como você poderia melhorar este sistema para incluir categorias adicionais, como jovem adulto (18-30) ou adulto maduro (31-60)?

### Prática: Melhore o Sistema

Agora é sua vez! Tente expandir o código acima para incluir a categoria de "jovem adulto" entre 18 e 30 anos.

Qual próxima etapa você quer explorar na programação com Python?

## Aplicação Prática com Estruturas Aninhadas

Quando você usa apps de entrega, como iFood ou Rappi, já parou pra pensar em como eles decidem o valor do frete? É bem parecido com o que vamos aprender hoje.

### Resolvendo Problemas Complexos

> 🤔 **Para refletir:** Como acha que esses aplicativos levam em conta tanto o peso da encomenda quanto a distância até seu destino?

Imagine que estamos criando um programa simples para determinar o preço do frete. Vamos começar com algumas regras básicas:

- Se a distância for menor ou igual a 5 km, não há cobrança.
- Acima de 5 km:
  - Até 10 kg: R$3,00 por cada km além dos primeiros 5 km.
  - Acima de 10 kg: R$4,00 por cada km além dos primeiros 5 km.

### Prática

Agora, pense em uma situação onde a distância é de 7 km e o peso da encomenda é de 8 kg. O que você faria para calcular o preço do frete?

Para resolver isso, podemos usar estruturas aninhadas como condicionais dentro de condicionais:

```python
distancia = 7  # Em quilômetros
peso = 8      # Em quilogramas

if distancia > 5:
    if peso <= 10:
        preco_frete = (distancia - 5) * 3.00
    else:
        preco_frete = (distancia - 5) * 4.00
else:
    preco_frete = 0

print(f"O preço do frete é R${preco_frete:.2f}")
```

### Sua Vez!

Tente agora calcular o frete para uma distância de 12 km e um peso de 15 kg. Use a estrutura aninhada que acabamos de aprender.

> 🤔 **Para refletir:** Como você adaptaria esse programa se houvesse mais faixas de preço?

## Para fechar — com as suas palavras

Escreva uma breve explicação sobre o que aprendeu hoje, usando suas próprias palavras. Isso ajudará a solidificar seus conhecimentos e permitirá que você compartilhe suas ideias com os outros.

## O que fica desta aula
```python
# Estruturas de decisão compostas:
if condicao1:
    # Faça algo se a condição 1 for verdadeira.
elif condicao2:
    # Faça algo se a condição 2 for verdadeira e a condição 1 não for.
else:
    # Faça algo se nenhuma das condições anteriores for verdadeira.

# Estruturas aninhadas para problemas mais complexos:
if principal_condicao:
    if subcondicao:
        # Faça algo se a subcondição for verdadeira dentro da condição principal.
    else:
        # Faça algo se a subcondição não for verdadeira, mas a condição principal sim.
else:
    # Faça algo se a condição principal não for verdadeira.
```

## Para ir além

- [Estruturas de controle em Python](https://docs.python.org/3/tutorial/controlflow.html)
- [Prática com estruturas condicionais](https://www.w3schools.com/python/python_conditions.asp)

## Referências
- Documentação oficial do Python: https://docs.python.org/3/
- W3Schools Python Tutorial: https://www.w3schools.com/python/default.asp