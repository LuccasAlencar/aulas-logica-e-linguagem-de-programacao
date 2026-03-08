---
title: "Aula 12 — Exercícios práticos com decisões"
layout: default
---

## Antes de começar

Antes de mergulharmos nos detalhes da aula, pense em um aplicativo ou jogo que você usa regularmente. Como ele decide quais informações exibir primeiro? Isso é o resultado direto do uso de estruturas de decisão compostas na programação.

## O que você vai aprender nesta aula

- Entender e aplicar estruturas de decisão compostas em situações práticas.
- Criar um sistema simples para classificar tarefas com base em critérios específicos.
- Refletir sobre como esses conceitos são usados na vida real, além do mundo da programação.

## Estruturas de Decisão Compostas

Quando você usa um aplicativo de compras online, ele verifica várias coisas antes de permitir que você finalize uma compra. É como se o app dissesse: "Vamos checar seu endereço, método de pagamento e se há estoque do produto." Isso é basicamente o mesmo conceito das estruturas de decisão compostas em programação.

### Como Funciona

Imagine um código que precisa tomar decisões com base em várias condições. Em vez de fazer uma única verificação lógica, você pode criar múltiplas verificações e ações diferentes para cada condição ou combinação delas. Isso permite que o programa responda de maneiras mais complexas e adaptáveis às situações.

> 🤔 **Para refletir:** Como seria um código que decide se alguém é elegível para um cartão de crédito, considerando idade, renda e histórico de pagamentos?

### Exemplo Prático: Sistema de Avaliação de Risco

Agora vamos criar um exemplo simples de um sistema que pode ajudar uma empresa a decidir se deve conceder ou não um empréstimo a um cliente. Vamos pensar nas condições como:

- A idade do cliente está entre 25 e 60 anos?
- A renda anual é superior a $30,000?
- O histórico de crédito é bom?

Baseado nessas perguntas, o sistema pode tomar uma decisão sobre se o empréstimo deve ser concedido ou não.

### Atividade Prática

Vamos pensar juntos: Como você classificaria as condições acima para um cliente com 35 anos, renda de $40.000 e bom histórico de crédito? Escreva suas decisões como se fossem um código em pseudocódigo.

---

Como você acha que poderíamos expandir essa ideia para incluir mais variáveis ou condições no futuro?

> 🤔 **Para refletir:** Que outros critérios poderiam ser adicionados ao sistema de avaliação de risco?

## Aplicação Prática: Estruturas de Decisão Compostas

Olá pessoal! Hoje vamos falar sobre estruturas de decisão compostas em um contexto bem real e que vocês podem usar no dia a dia.

### Começando com Apps e Jogos

Sabem aquele aplicativo de tarefas ou jogo que usa cores para te lembrar o quão importante é uma coisa? Esses apps usam estruturas de decisão compostas para determinar se algo deve ser destacado ou não. É como quando você precisa decidir entre jogar mais um round no videogame ou terminar a lição de casa.

### Exemplo Prático: Sistema de Classificação de Tarefas

Imagine que estamos criando um sistema simples que classifica suas tarefas em base na urgência e importância. Você pode usar uma escala como 1 (não urgente/não importante) até 4 (urgente e importante). Vamos criar um exemplo com Python:

```python
def classificar_tarefa(urgencia, importancia):
    if urgencia >= 3 and importancia >= 3:
        return "Prioridade Alta"
    elif urgencia == 2 and importancia == 2:
        return "Importante, mas não urgente"
    else:
        return "Baixa Prioridade"

# Exemplo de uso
print(classificar_tarefa(3, 4))
```

> 🤔 **Para refletir:** Como você usaria essa função em seu próprio dia a dia para gerenciar melhor o tempo e as tarefas?

### Atividade Prática

Agora, eu quero que vocês pensem em uma tarefa que é importante mas não urgente. Coloque essas tarefs no sistema que criamos. Por exemplo:

```python
print(classificar_tarefa(2, 3))
```

Qual resultado esperado essa linha de código iria gerar? Lembrem-se de pensar como o programa pensa e analise as condições.

---

E ai pessoal, vocês conseguem visualizar como essas estruturas podem ser úteis na vida real? E se pensarmos em mais recursos para esse sistema, como notificações ou classificação de tarefas por categoria?

Qual é a próxima coisa que vocês gostariam de adicionar ao seu gerenciador pessoal de tarefas?

## Arquitetura da Informação

Quando você usa um app de redes sociais e vê apenas os posts que são relevantes para você, isso é resultado direto de estruturas de decisão compostas. É como magia, mas na verdade é programação! 🚀

### Estruturas de Decisão Compostas
Estruturas de decisão compostas ajudam a decidir quais informações mostrar primeiro ou deixar para depois. Elas são fundamentais em sistemas que precisam priorizar e organizar dados.

🤔 **Para refletir:** Como você pode perceber estruturas de decisão compostas na sua vida diária?

Imagine que você está criando um sistema de busca para um site escolar. Quer mostrar os resultados mais relevantes primeiro, como eventos da semana ou notícias importantes. Você teria que decidir o que é relevante e priorizar essa informação.

> **Atividade Prática:** Considere uma situação onde você precisa buscar uma matéria específica em seu livro de texto digital. Como estruturaria suas decisões para tornar a busca mais eficiente?

Essas decisões ajudam os usuários a encontrar rapidamente o que precisam, melhorando toda a experiência do site.

🤔 **Para refletir:** Por que é importante priorizar certos resultados em uma pesquisa online?

E agora, pense: como esses princípios de arquitetura da informação seriam aplicados se você quisesse criar um jogo de realidade aumentada para smartphones?

## Para fechar — com as suas palavras

Escreva algumas linhas sobre o que aprendeu hoje e como planeja usar estruturas de decisão compostas em seus projetos futuros.

## O que fica desta aula
```python
# Estrutura de decisão composta
def classificar_tarefa(urgencia, importancia):
    if urgencia >= 3 and importancia >= 3:
        return "Prioridade Alta"
    elif urgencia == 2 and importancia == 2:
        return "Importante, mas não urgente"
    else:
        return "Baixa Prioridade"

# Sistema de avaliação de risco
def avaliar_risco(idade, renda, historico):
    if idade >= 25 and idade <= 60 and renda > 30000 and historico == 'bom':
        return True
    else:
        return False
```

## Para ir além

- [Estruturas de Decisão Compostas em Python](https://www.geeksforgeeks.org/decision-making-in-python/)
- [Arquitetura da Informação e Estruturas de Decisão](https://www.interaction-design.org/literature/topics/architecture-of-information)

## Referências

- GeeksforGeeks. (2021). Decision Making in Python. Recuperado em 30/09/2021, de https://www.geeksforgeeks.org/decision-making-in-python/
- Interaction Design Foundation. (n.d.). Architecture of Information. Recuperado em 30/09/2021, de https://www.interaction-design.org/literature/topics/architecture-of-information