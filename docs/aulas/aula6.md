---
title: "Aula 6 — Processamento de dados"
layout: default
---

## Antes de começar

### Pergunta inicial instigante:
Como você acha que os aplicativos em seu celular decidem quando mostrar um alerta ou recomendação personalizada?

## O que você vai aprender nesta aula

- Como usar estruturas de decisão simples (`if-else`) para tomar decisões baseadas em condições.
- Utilizar operadores lógicos para combinar múltiplas condições e criar decisões mais complexas.
- Aplicar esses conceitos na resolução de problemas do dia a dia através da programação.

## Estrutura de Decisão Simples

Vamos começar com algo do seu dia a dia. Quando você usa apps que verificam se você atingiu sua meta diária de passos no celular, eles usam uma estrutura de decisão para decidir se mostrar um alerta "Parabéns!" ou não.

A estrutura if-else é como essa lógica funciona nos programas. Ela permite que o programa tome decisões com base em condições específicas. Se a condição for verdadeira, ele segue uma rota; caso contrário, outra. Assim, o algoritmo pode adaptar seu comportamento conforme as circunstâncias.

Vamos usar um exemplo prático: imagine um aplicativo que verifica se você é maior de idade para entrar em certos lugares na internet ou mesmo em eventos restritos por idade.

```python
idade = 18 # Suponha que esta seja a sua idade

if idade >= 18:
    print("Você pode acessar conteúdos e locais com restrição de idade.")
else:
    print("Desculpe, você deve ser maior de 18 anos para acessar este conteúdo.")
```

> 🤔 **Para refletir:** Como seria o código se quiséssemos verificar uma faixa etária mais específica, como entre 25 e 30 anos?

Agora, tente criar um pequeno bloco de código que verifica se alguém pode votar no Brasil (idade mínima é 16 anos). Coloque a sua idade em uma variável e escreva o if-else necessário.

Pronto! Agora você entende como os programas podem tomar decisões baseadas nas informações fornecidas. 

Qual seria o próximo passo se quiséssemos adicionar mais condições à nossa decisão, por exemplo, verificar diferentes permissões com base em faixas de idade?

## Operadores Lógicos

Olha, você já parou pra pensar em quantas vezes por dia o seu telefone te avisa sobre algo importante? Apps de tempo são um ótimo exemplo. Quando eles combinam várias condições, como "está chovendo" e "tem vento forte", para recomendar que você pegue guarda-chuva e casaco... Isso é exatamente do que estamos falando hoje: operadores lógicos.

### Usando 'and' na Programação

Aqui está um exemplo rápido pra ilustrar isso. Vamos supor que temos uma variável `estaChovendo` que retorna verdadeira se estiver chovendo e outra variável `temVentoForte` para saber se o vento é forte.

```python
estaChovendo = True  # Supondo que está chovendo
temVentoForte = False  # Supondo que não tem vento forte

# Agora, vamos combinar essas condições usando 'and'
if estaChovendo and temVentoForte:
    print("Pegue guarda-chuva e casaco!")
```

> 🤔 **Para refletir:** Como você acha que o código mudaria se `temVentoForte` fosse verdadeiro também? Seria necessário adicionar algum novo operador ou lógica?

### Atividade Prática

Agora, vamos fazer um pequeno exercício. Se `estaChovendo` for verdadeira e `temSol` for falsa (não está sol), o que você faria para sugerir que a pessoa use guarda-chuva? Dê uma sugestão de código.

## Aplicação Prática: Resolvendo Problemas do Dia a Dia com Programação

Olá, pessoal! Já repararam que usamos aplicativos e jogos todos os dias? Bem, muitas dessas ferramentas contêm pequenas porções de código que fazem coisas incríveis para tornar nossa vida mais fácil.

Vamos começar falando sobre um conceito básico da programação: estruturas condicionais. Elas são como nossos cérebros quando tomamos decisões diárias, mas na forma de código.

### Exemplo Prático

Imagine que você está desenvolvendo um app simples para calcular a idade de uma pessoa e exibir mensagens diferentes dependendo se ela é maior ou menor de 18 anos. Como faríamos isso usando estruturas condicionais?

Aqui vai um exemplo básico:

```python
idade = int(input("Digite sua idade: "))
if idade >= 18:
    print("Você pode comprar álcool!")
else:
    print("Espere mais um pouco para beber, jovem!")
```

> 🤔 **Para refletir:** Como você acha que as redes sociais usam estruturas condicionais para controlar o acesso de usuários?

Agora, vamos praticar! Abra seu editor de código preferido e escreva um programa parecido com o exemplo acima. Depois, mude os textos das mensagens exibidas para algo mais divertido ou informativo.

Pronto? Agora pense em como você poderia estender este conceito para outros contextos da vida real. **Qual outro tipo de decisão na vida cotidiana poderíamos modelar usando estruturas condicionais em código?**

## Para fechar — com as suas palavras

Escreva um breve resumo do que aprendeu hoje sobre estruturas condicionais e operadores lógicos.

## O que fica desta aula
```markdown
- Estrutura de decisão simples (`if-else`): permite tomar decisões baseadas em condições.
- Operador lógico `and`: combina duas ou mais condições para criar decisões complexas.
```

## Para ir além

1. Explore como os aplicativos de fitness usam estruturas condicionais e operadores lógicos para fornecer feedback personalizado aos usuários.
2. Pesquise sobre a implementação de estruturas condicionais em linguagens de programação diferentes.

## Referências
- Livro "Python Crash Course" por Eric Matthes
- Documentação oficial do Python: https://docs.python.org/3/tutorial/controlflow.html#defining-functions