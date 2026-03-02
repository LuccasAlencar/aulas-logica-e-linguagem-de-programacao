# 💻 Lógica de Programação — Aula 5

## Entrada de Dados (Input)

> **Hoje você vai aprender a primeira coisa que um programa precisa para existir:**
> Receber informações do usuário.

Sim — antes de jogos, apps e IA…
todo programa começa fazendo uma pergunta.

---

## 🧠 Pense nisso

Imagine um aplicativo de:

* Uber
* Instagram
* Caixa eletrônico
* Jogo
* Site de compras

Todos eles precisam de algo primeiro:

> **informação**

O computador **não adivinha**.
Ele **não pensa sozinho**.

Ele só trabalha com aquilo que você fornece.

Isso se chama:

# 🔹 DADOS

---

## O ciclo de todo programa

Todo programa do mundo funciona assim:

```
ENTRADA → PROCESSAMENTO → SAÍDA
```

| Etapa         | O que acontece                    |
| ------------- | --------------------------------- |
| Entrada       | O usuário fornece informações     |
| Processamento | O programa calcula ou decide algo |
| Saída         | O programa mostra o resultado     |

---

### Exemplo (vida real)

Caixa eletrônico:

* você digita a senha → **entrada**
* o banco verifica → **processamento**
* aparece “senha correta” → **saída**

---

### Outro exemplo

Calculadora:

* você digita 5 + 2 → entrada
* ela soma → processamento
* mostra 7 → saída

---

## O que é ENTRADA DE DADOS?

Entrada de dados é:

> O momento em que o usuário fornece informações para o algoritmo.

O algoritmo **precisa perguntar**.

Se ele não perguntar, ele não sabe nada.

---

## Tipos de dados que um programa pede

Anote:

| Tipo   | Exemplos                            |
| ------ | ----------------------------------- |
| Texto  | nome, cidade, email                 |
| Número | idade, salário, altura              |
| Opção  | sim/não, 1 ou 2, masculino/feminino |

---

## Como escrevemos isso em algoritmo?

Usamos um comando chamado:

# ✏️ LEIA (ou LER)

Ele significa:

> “Peça uma informação ao usuário.”

---

### Exemplo de algoritmo

```
Início
Leia nome
Escreva "Olá, ", nome
Fim
```

O que acontece?

O programa pergunta o nome
→ usuário responde
→ o programa usa a resposta

---

## Outro exemplo

```
Início
Leia idade
Escreva "Você tem ", idade, " anos"
Fim
```

Observe:

O programa não inventa a idade.
Ele **espera o usuário informar**.

---

## Muito importante ⚠️

O computador:

* não entende contexto
* não deduz
* não “imagina”

Ele só usa o que foi digitado.

Se não houver **entrada**, não existe programa útil.

---

## Variável (ideia fundamental)

Quando o programa recebe um dado, ele guarda numa “caixinha”.

Essa caixinha se chama:

# 📦 VARIÁVEL

Ela serve para **armazenar a resposta do usuário**.

Exemplo:

```
Leia nome
```

O que aconteceu?

O algoritmo criou:

📦 variável chamada **nome**
e guardou a resposta dentro dela.

---

## Exemplo completo

```
Início
Leia nome
Leia idade
Escreva "Seu nome é ", nome
Escreva "Sua idade é ", idade
Fim
```

Você acabou de escrever um programa de cadastro.

Sem perceber 🙂

---

# ✍️ ATIVIDADE (no caderno)

Crie um algoritmo que:

1. Pergunte o nome do aluno
2. Pergunte a idade
3. Pergunte a cidade
4. Mostre todas as informações na tela

Use:

* Início
* Leia
* Escreva
* Fim

---

## Desafio ⭐

Agora pense:

Um aplicativo de **cadastro de escola** precisa pedir o quê?

Escreva no caderno **5 perguntas** que o sistema deveria fazer ao aluno.

(Ex: nome, série…)

---

## O que você aprendeu hoje

Você aprendeu que:

* todo programa recebe dados
* isso se chama **entrada**
* usamos o comando **LEIA**
* os dados ficam guardados em **variáveis**
* sem entrada não existe software

Na próxima aula você vai descobrir:

> O que o programa FAZ com esses dados.

E aí começa a parte mais interessante da programação.


# 🧩 Exercícios — Entrada de Dados

> Faça tudo no caderno.
> Escreva os algoritmos completos.

---

## 1) Identifique

Em cada situação abaixo, diga:

* qual é a **entrada**
* qual é o **processamento**
* qual é a **saída**

### a) Login do Instagram

### b) Compra com cartão

### c) Digitar senha do celular

---

## 2) Complete o algoritmo

Complete:

```
Início
Leia ________
Escreva "Bem-vindo, ", ________
Fim
```

Qual informação o programa está pedindo?

---

## 3) Criando perguntas

Crie um algoritmo que pergunte:

* comida favorita
* filme favorito
* jogo favorito

Depois o programa deve mostrar tudo ao usuário.

---

## 4) Cadastro de aluno

Monte um algoritmo para cadastrar um aluno com:

* nome
* idade
* série
* escola

---

## 5) Desafio 🚀

Crie um algoritmo de **cadastro de jogo** que peça:

* nome do jogador
* personagem escolhido
* nível atual
* pontuação

Depois mostre uma ficha do jogador.

---

## 6) Verdadeiro ou Falso

( ) Um programa pode funcionar sem receber dados.
( ) Entrada é quando o usuário fornece informações.
( ) A variável serve para guardar dados.
( ) O comando LEIA mostra mensagens na tela.

---

## 7) Pensamento de programador

Responda:

Por que um aplicativo de delivery precisa de entrada de dados?

Explique com suas palavras.
