---
title: "Aula 7 — Saída de dados"
layout: default
---

## Antes de começar

Antes de mergulharmos nos detalhes desta aula sobre operadores lógicos, comparadores e estruturas lógicas na programação, pense comigo: quando você posta um vídeo no TikTok, quantas condições precisam ser verdadeiras para que ele seja publicado?

## O que você vai aprender nesta aula

- Como usar os operadores AND, OR e NOT em situações do dia a dia.
- A diferença entre os operadores de comparação `==` e `!=`.
- Como criar estruturas lógicas simples para tomar decisões baseadas em condições específicas.

## Operadores Lógicos AND, OR e NOT

Pensando em algo do seu dia a dia... quando você posta um vídeo no TikTok, ele só aparece na sua timeline se for carregado com sucesso **e** estiver dentro dos limites de tamanho. Isso é exatamente como o operador lógico AND: duas condições precisam ser verdadeiras para que algo aconteça.

### AND
O AND combina duas ou mais condições, mas lembre-se: se uma delas for falsa, tudo vira mentira! Na programação, isso é super útil quando você precisa de várias coisas certas ao mesmo tempo.

> 🤔 **Para refletir:** Quando você postou um vídeo no TikTok recentemente, quantos passos ou condições precisaram ser verdadeiras para que o vídeo fosse publicado?

Agora, vamos colocar isso em prática. Imagine que você está criando uma função no código que verifica se um jogador pode ganhar um item especial na sua próxima partida de jogo:
```python
def pode_ganhar_item_nivel(nivel_jogador, qtd_vitorias):
    return nivel_jogador >= 10 and qtd_vitorias > 3
```
Se o nível do jogador for maior ou igual a 10 **e** ele tiver mais de três vitórias, então pode ganhar um item especial. Vamos testar algumas entradas diferentes.

### OR e NOT
Pronto para algo novo? Agora vamos ao OR! Se pelo menos uma das condições for verdadeira, tudo vira verdade. Isso é como quando você quer ver um filme e basta que pelo menos um de seus amigos esteja disponível.

E o NOT inverte tudo: se algo está verdadeiro, ele torna falso e vice-versa. Imagine negar a condição "estou feliz" com NOT: se estiver feliz, vira triste (na lógica)!

> 🤔 **Para refletir:** Como você usaria o OR na sua rotina para tomar decisões?

Qual operador você já está pensando em usar mais?

## Comparadores

Quando você está navegando pelas redes sociais e vê duas opções de compra, tipo aquele novo celular que todo mundo tem, já pensou em comparar os preços? É exatamente isso que fazemos com frequência na programação, mas com um toque tecnológico.

### Operadores de Comparação

Em linguagens de programação, usamos operadores como `==` para verificar se dois valores são iguais e `!=` para ver se eles são diferentes. São básicos, mas fundamentais pra qualquer código que faz comparações.

> 🤔 **Para refletir:** Como você decidiria qual desses dois smartphones comprar sem comparar seus preços?

Agora, faça uma pequena atividade: imagine que temos duas variáveis `preco_smartphone_1` e `preco_smartphone_2`. Escreva um código para verificar se o preço do primeiro smartphone é diferente do segundo. É como você faria na vida real!

E aí? Agora, vamos pensar em como esses operadores podem ajudar não só com compras, mas também em jogos e aplicativos que você usa diariamente.

Qual outro tipo de comparação você faz todos os dias que pode ser útil para aprender mais sobre comparadores na programação?

## Estruturas Lógicas

Quando você usa um app de compras online e vê descontos aparecendo automaticamente, sabe que algo está acontecendo por trás dos panos. Hoje vamos entender como esses sistemas funcionam usando estruturas lógicas.

### Aplicação na Vida Real

Vamos pensar em um exemplo simples: um aplicativo de cupons onde o desconto é maior para compras acima de R$100,00. Como você acha que isso funciona?

> 🤔 **Para refletir:** Como podemos criar uma condição lógica para decidir se alguém ganha ou não ganha um desconto extra?

Vamos começar com algo simples: escreva um algoritmo em pseudocódigo que decida se um cliente recebe 10% de desconto na compra, baseado no valor da compra ser maior do que R$150,00.

### Atividade Prática

```
COMEÇAR
    LEIA (valorCompra)
    SE valorCompra > 150 ENTÃO
        ESCREVA ("Parabéns! Você ganhou um desconto de 10%. Sua nova fatura é: " + (valorCompra * 0,9))
    SENÃO
        ESCREVA ("Sua compra não se qualifica para o desconto especial.")
    FIM SE
FIM
```

Agora você entendeu como uma estrutura lógica pode ajudar a decidir sobre algo simples. Essas regras podem ficar mais complexas, mas seguem a mesma ideia fundamental.

### Próximo Passo

Como podemos expandir essa lógica para incluir diferentes tipos de descontos baseados em várias condições? Vamos descobrir na próxima aula!

## Atividades Práticas

Quando você usa um aplicativo de redes sociais e ele te mostra as postagens mais relevantes primeiro, percebe que há alguém por trás disso fazendo a mágica acontecer. Esse alguém é quem desenvolve sistemas computacionais para resolver problemas específicos.

### Desenvolver Sistemas Computacionais

Imagine criar um programa que classifica os estudantes da sua turma com base em notas e frequência. Isso ajuda o professor a identificar quem precisa de mais apoio. 🚀 Vamos dar uma olhada rápida nisso hoje.

> 🤔 **Para refletir:** Como você pode melhorar essa ideia para ajudar outros estudantes além da sua turma?

Agora, faça um breve esboço de como o programa poderia funcionar. Pense em pelo menos uma maneira que ele poderia ser útil na vida real.

Queremos ouvir suas ideias! Como você acha que isso pode se conectar com outras áreas do seu estudo técnico?

## Para fechar — com as suas palavras

Escreva um breve resumo sobre o que aprendeu nesta aula, usando suas próprias palavras. Que conceitos novos te chamaram mais atenção e por quê?

## O que fica desta aula
```python
# AND: duas condições precisam ser verdadeiras para algo acontecer.
exemplo_and = (nivel_jogador >= 10) and (qtd_vitorias > 3)

# OR: pelo menos uma condição precisa ser verdadeira para algo acontecer.
exemplo_or = (tem_amigos_disponiveis) or (pode_ir_sozinho)

# NOT: inverte a lógica de uma condição.
exemplo_not = not (estou_feliz)
```

## Para ir além
- [W3Schools - Operadores Lógicos](https://www.w3schools.com/python/python_operators.asp)
- [GeeksforGeeks - Estruturas Condicionais em Python](https://www.geeksforgeeks.org/decision-making-python/)

## Referências
- W3Schools. (2021). Operadores Lógicos em Python.
- GeeksforGeeks. (2021). Estruturas Condicionais em Python.