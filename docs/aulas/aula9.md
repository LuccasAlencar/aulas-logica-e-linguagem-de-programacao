---
title: "Aula 9 — Condição simples: introdução ao SE"
layout: default
---

## Antes de começar

Antes de mergulharmos no conteúdo desta aula, pense em uma situação do cotidiano onde você precisa tomar uma decisão baseada em uma condição. Como seria essa tomada de decisão se fosse codificada?

## O que você vai aprender nesta aula
- Entender o conceito básico de estrutura condicional simples (SE).
- Escrever pseudocódigo para resolver problemas usando estruturas condicionais.
- Criar uma pequena atividade prática baseada em condições.

## Estrutura de Decisão Simples

Olá pessoal! Vamos começar falando sobre algo que vocês usam todos os dias. Quando você tenta acessar uma rede social e o aplicativo pergunta por sua senha, isso é um exemplo de **estrutura de decisão simples**. O programa está perguntando: "Essa pessoa tem autorização para entrar?" E aí faz alguma coisa com base na resposta.

### Introdução à Estrutura Condicionada Simples (SE)
Vamos entender como isso funciona no código. Quando escrevemos um programa, queremos que ele tome decisões de acordo com as condições existentes. Em pseudocódigo, usamos a palavra **SE** para fazer isso.

> 🤔 **Para refletir:** Como vocês imaginam o sistema da rede social decidindo se você tem permissão ou não para entrar?

### Exemplo: Sistema de Acesso
Vamos criar um exemplo simples em pseudocódigo. Imagine que queremos escrever um programa que verifica se uma pessoa é maior de 18 anos antes de permitir acesso a algum recurso.

```pseudocode
SE idade >= 18 ENTAO
    PERMITIR acesso ao recurso
SENÃO
    IMPEDIR acesso ao recurso
FIM SE
```

### Atividade: Escreva sua própria estrutura de decisão simples!
Agora, vocês precisam criar uma pequena estrutura que decida se um jogador pode participar de um jogo online. O jogo só permite jogadores com nível acima de 5.

Pensem na condição necessária e como o programa deve reagir dependendo dessa condição.

## Para fechar — com as suas palavras
Escreva em suas próprias palavras sobre a estrutura condicional simples que aprendemos hoje. Como você descreveria essa ideia para alguém que nunca ouviu falar dela?

## O que fica desta aula
```python
# Estrutura de decisão simples (SE)
estrutura_condicional_simples = "Uma lógica onde o programa toma uma decisão com base em uma condição."
```

## Para ir além
- [Estruturas condicionais no Python](https://docs.python.org/3/tutorial/controlflow.html#if-statements) — Documentação oficial do Python sobre estruturas condicionais.
- [Exercícios de prática](http://codingbat.com/java/Logic-1) — Exercícios práticos para praticar lógica e estruturas condicionais.

## Referências
- Livro "Python Crash Course" por Eric Matthes.
- Documentação oficial do Python.