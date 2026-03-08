---
title: "Aula 10 — Condição composta: SE…SENÃO"
layout: default
---

## Antes de começar

Você já se perguntou como redes sociais decidem se você pode acessar certos conteúdos? Hoje, vamos explorar a lógica por trás dessas decisões e aprender a criar estruturas condicionais compostas em Python.

## O que você vai aprender nesta aula

- Como usar `if` e `else` para tomar decisões simples.
- Estruturar condições compostas usando operadores lógicos como `and`.
- Refletir sobre o impacto da ordem das condições na lógica do programa.

## Estruturas Condicionais Compostas

Quando você acessa uma rede social e vê aquele aviso dizendo que precisa ser maior de idade para continuar, essa mensagem é resultado de uma estrutura condicional. E hoje vamos aprender como criar algo parecido em Python!

### Aprendendo com Exemplos Reais
Imagina que queremos escrever um programa que verifica se você pode entrar na nossa rede social secreta da escola. Para isso, precisamos confirmar duas coisas:
1. Você é maior de idade.
2. Você é estudante.

Para fazer isso, usaremos **estruturas condicionais compostas**. Vamos ver como:

```python
idade = 18
e_estudante = True

if idade >= 18 and e_estudante:
    print("Bem-vindo à nossa rede social secreta!")
else:
    print("Desculpe, você não pode entrar ainda.")
```

> 🤔 **Para refletir:** Como essa lógica poderia ser usada para ajudar alguém a tomar decisões mais complexas?

### Sua Vez de Tentar
Agora, faça uma pequena modificação no código acima:
- Altere a variável `idade` para 17 anos.
- Mantenha `e_estudante = True`.

Rode o programa e veja o que acontece. Escreva esse novo código logo abaixo:

```python
# Sua vez de modificar as condições e ver como isso afeta os resultados
```

## Uso de if, elif e else

Imagine que você está jogando um jogo onde seu personagem precisa tomar decisões com base em diferentes níveis de experiência. Dependendo do nível alcançado, ele ganha habilidades especiais. Na programação, usamos `if`, `elif` (else if) e `else` para criar esses tipos de decisões.

### Exemplo: Sistema de classificação de notas

Vamos construir um sistema simples que classifica uma nota numérica em categorias como 'Aprovado', 'Recuperação' ou 'Reprovado'. Usaremos `if`, `elif` e `else`.

```python
nota = 75 # Suponha que esta seja a nota do aluno

if nota >= 90:
    print("Nota: A")
elif nota >= 80:
    print("Nota: B")
elif nota >= 70:
    print("Nota: C")
elif nota >= 60:
    print("Nota: D")
else:
    print("Nota: F")

# Agora, tente você mesmo! Altere o valor da variável `nota` e veja como as classificações mudam.
```

> 🤔 **Para refletir:** Se um aluno tiver uma nota exatamente igual a 70, ele cairia na categoria 'C' ou 'D'? Por quê?

## Ordem das Condições

Olá pessoal! Hoje vamos falar sobre uma parte importante da lógica de programação que pode te ajudar muito quando estiver fazendo seus jogos e apps. Já pensaram em como os sistemas sabem a sua idade ou status no jogo? É tudo baseado na ordem das condições.

Imagine você querendo entrar num app onde só podem acessar pessoas maiores de 18 anos e estudantes universitários. Como o sistema decide se pode te deixar entrar?

### Exemplo: Sistema de classificação

Vamos criar um simples programa que verifica a idade e o status do usuário para decidir se ele pode usar nosso aplicativo ou jogo.

```python
idade = int(input("Digite sua idade: "))
status_estudante = input("Você é estudante universitário? (s/n): ")

if idade >= 18:
    if status_estudante == "s":
        print("Bem-vindo! Você pode usar nosso app.")
    else:
        print("Desculpe, você precisa ser um estudante universitário para entrar.")
else:
    print("Você não tem a idade mínima permitida.")
```

Agora, pense se mudássemos a ordem das condições. Altere o código acima fazendo a verificação do status de estudante primeiro e depois da idade. O que acontece?

> 🤔 **Para refletir:** A mudança na ordem afetou o resultado? Por quê?

### Atividade Prática

Teste este código mudando as condições de lugar. Note como isso altera a mensagem exibida.

Agora, pense: existem outras formas de estruturar essa lógica sem perder informações importantes sobre os usuários?

## Para fechar — com as suas palavras
Escreva em suas próprias palavras o que você aprendeu hoje sobre condições compostas e a ordem das condições. Por exemplo:
- O que é uma condição composta?
- Como a ordem das condições pode afetar o resultado de um programa?

## O que fica desta aula

```python
# Condições compostas: usam operadores lógicos como 'and' e 'or'.
# if, elif e else: permitem criar estruturas condicionais complexas.
# Ordem das condições: a ordem em que as condições são verificadas pode afetar o resultado final do programa.
```

## Para ir além
- [Documentação oficial Python](https://docs.python.org/3/tutorial/controlflow.html#if-statements)
- [Estruturas condicionais no Codecademy](https://www.codecademy.com/learn/introduction-to-python/modules/python-control-flow/cheatsheet)

## Referências
- Livro "Python Crash Course" por Eric Matthes.
- Documentação oficial do Python.