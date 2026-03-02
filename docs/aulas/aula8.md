---
title: "Aula 8 — Exercícios integrados (entrada, processamento e saída)"
layout: default
---

## Antes de começar

Antes de mergulharmos nos detalhes desta aula sobre estruturas condicionais em programação, pense comigo: quantas vezes por dia você toma uma decisão baseada em condições específicas? Seja decidir se precisa levar um guarda-chuva ou escolher entre várias opções no menu de um aplicativo. Essa é exatamente a lógica que usamos ao programar!

## O que você vai aprender nesta aula

- Como usar estruturas condicionais simples (`if-else`) para tomar decisões baseadas em condições.
- A importância e o uso dos operadores lógicos `&&`, `||` e `!`.
- Como criar menus interativos com opções de escolha usando estruturas condicionais.

## Estruturas de Decisão Simples

Olá, pessoal! Vamos falar sobre algo que vocês usam todos os dias sem nem perceber: estruturas de decisão simples em programação. Já imaginaram como as redes sociais determinam se você é maior de idade para ver certos conteúdos? Pois bem, isso tudo tem a ver com `if-else`.

### A Magia por Trás do Botão "Entrar"

Quando você clica no botão "entrar" em um jogo ou aplicativo que exige que você seja maior de 18 anos para acessar certos conteúdos, acontece um processo parecido com isso: o programa verifica se a sua idade é igual ou superior a 18. Se for, você entra sem problemas; caso contrário, o programa mostra uma mensagem dizendo que precisa esperar mais um pouco.

```python
idade = int(input("Qual é a sua idade? "))
if idade >= 18:
    print("Bem-vindo! Você pode acessar todos os conteúdos.")
else:
    print("Desculpe, você ainda não tem permissão para entrar nessa área.")
```

Agora, pega uma papel e caneta. Vamos fazer um teste rápido:

- Escreva uma condição `if-else` que verifica se a temperatura está acima de 30°C e imprime "Está quente demais!" ou "Que tempo maravilhoso!" dependendo da situação.

> 🤔 **Para refletir:** Como você usaria essa estrutura em um aplicativo para decidir se o usuário pode comprar álcool?

Vamos continuar explorando como essas decisões podem ser mais complexas e interessantes na próxima aula. Quem tem uma ideia legal sobre como usar `if-else`?

## Operadores Lógicos na Prática

Quando você olha o aplicativo do tempo no seu celular, ele usa lógica e operadores como `&&`, `||` e `!` para decidir se vai chover hoje. Vamos entender isso!

### && (e)
Primeiro, vamos ver o `&&`. Ele é usado quando duas coisas precisam ser verdade para que algo aconteça. Por exemplo:
```javascript
if(clima == "chuva" && temperatura < 15) {
    console.log("Vá de casaco!");
}
```
Isso significa: se estiver chovendo e a temperatura for abaixo de 15 graus, é melhor pegar o casaco.

### || (ou)
Agora, olhe para o `||`. Ele entra em cena quando qualquer uma das condições pode ser verdadeira. Por exemplo:
```javascript
if(clima == "chuva" || clima == "nublado") {
    console.log("Pegue um guarda-chuva!");
}
```
Se estiver chovendo ou nublado, é melhor levar o guarda-chuva.

### ! (não)
E para terminar, temos o `!`, que nega uma condição. Como usar?
```javascript
if(!sol) {
    console.log("Pegue um casaco!");
}
```
Se não estiver ensolarado, é melhor pegar o casaco.

> 🤔 **Para refletir:** Quando você toma decisões baseadas em condições meteorológicas, como usa esses operadores lógicos na sua rotina?

Agora, tente criar uma condição simples usando os operadores que aprendemos. Por exemplo: escreva um código para decidir se a luz precisa ser ligada com base na hora do dia e na presença de pessoas em casa.

Qual será o próximo passo depois de entender esses operadores?

## Aplicação Prática de Estruturas Condicionais

Olá pessoal! Já pararam pra pensar em quantas vezes por dia vocês interagem com menus? Nos apps, redes sociais, jogos... Sempre tem aquela tela inicial que te pergunta "O que deseja fazer agora?"

Agora, imagine como esses menus funcionam. Quando você clica na opção para enviar uma mensagem no WhatsApp ou postar algo no Instagram, o app está usando estruturas condicionais. É tipo um "se" e "senão", sabe? Se você clicou nesse botão, faça isso; senão, faça aquilo.

### Exemplo: Programa de Menu Simples

Vamos criar um programa que mostra um menu simples e faz algo dependendo da sua escolha. Por exemplo:

- **1** - Ver Notas
- **2** - Adicionar Nota
- **3** - Sair

Se você digitar '1', o programa vai mostrar suas notas; se for '2', ele adicionará uma nova nota e assim por diante.

Aqui está um esqueleto do que podemos fazer:

```python
escolha = input("Escolha uma opção: ")

if escolha == "1":
    # Código para exibir as notas
elif escolha == "2":
    # Código para adicionar uma nova nota
else:
    print("Saindo...")
```

Tente escrever um pequeno programa seguindo esse modelo. Pense em pelo menos duas coisas diferentes que você gostaria de fazer com base na opção selecionada.

> 🤔 **Para refletir:** Como você pode usar estruturas condicionais para criar uma experiência do usuário mais personalizada no seu próximo projeto?

Pronto! Agora vamos explorar como podemos expandir essa ideia usando loops. Vocês já pensaram em como os jogos permitem que você jogue repetidamente até perder? É a mesma lógica! Vamos lá, prontos para o próximo passo?

## Para fechar — com as suas palavras

Escreva um breve resumo sobre o que aprendeu nesta aula. Use suas próprias palavras e inclua exemplos de como você aplicaria esses conceitos em projetos futuros.

## O que fica desta aula
```python
# Estruturas condicionais simples (if-else)
idade = int(input("Qual é a sua idade? "))
if idade >= 18:
    print("Bem-vindo! Você pode acessar todos os conteúdos.")
else:
    print("Desculpe, você ainda não tem permissão para entrar nessa área.")

# Operadores lógicos
clima = "chuva"
temperatura = 10

if clima == "chuva" and temperatura < 15:
    print("Vá de casaco!")

# Menu interativo com estruturas condicionais
escolha = input("Escolha uma opção: ")
if escolha == "1":
    # Exibir notas
elif escolha == "2":
    # Adicionar nota
else:
    print("Saindo...")
```

## Para ir além

- **Livro:** *Estruturas de Dados e Algoritmos* por Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest e Clifford Stein.
- **Website:** [W3Schools](https://www.w3schools.com/) - Recursos interativos para aprender a programar.

## Referências

- Estruturas condicionais: https://docs.python.org/3/tutorial/controlflow.html
- Operadores lógicos: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#logical_operators