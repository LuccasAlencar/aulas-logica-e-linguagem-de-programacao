# Aula 4 — Variáveis e Tipos de Dados

> **Componente:** Lógica e Linguagem de Programação  
> **Unidade:** Estrutura Básica  
> **Duração:** 50 minutos  

---

## 🧠 O que você vai aprender hoje

Até agora você aprendeu que algoritmos são sequências de passos e que fluxogramas são a representação visual desses passos. Mas um sistema de verdade precisa **guardar informações** enquanto está rodando — o nome do usuário, a pontuação de um jogo, o total de uma compra.

Hoje você vai aprender sobre **variáveis**: o mecanismo fundamental que todo programa usa para armazenar e manipular dados.

---

## 📦 O que é uma variável?

Imagine que você tem uma **caixa**. Nessa caixa você coloca alguma coisa, escreve um nome na tampa e pode consultar ou trocar o conteúdo quando quiser.

Isso é exatamente uma variável:
- A **caixa** = espaço na memória do computador
- O **nome na tampa** = nome da variável
- O **conteúdo** = o valor armazenado

```
  ┌─────────────────┐
  │   "João Silva"  │  ← valor
  └─────────────────┘
        nomeUsuario   ← nome da variável
```

Quando o programa precisar saber quem é o usuário logado, ele simplesmente "abre a caixa" chamada `nomeUsuario` e lê o valor de dentro.

> 💡 O nome "variável" vem do fato de que o conteúdo pode **variar** ao longo do tempo. A caixa pode ser esvaziada e preenchida com outro valor.

---

## 🔤 Tipos de dados

Nem toda informação é do mesmo tipo. Um nome é diferente de uma idade, que é diferente de um preço, que é diferente de uma resposta "sim ou não". Por isso, variáveis têm **tipos**.

Conheça os principais:

---

### 1. Inteiro (`int` / `inteiro`)

Números **sem casas decimais**. Usados para contagens, idades, quantidades.

**Exemplos de valores:** `0`, `7`, `42`, `-3`, `1000`

**Exemplos de uso:**
```
idadeUsuario = 17
totalEntrevistados = 0
quantidadeAcoes = 15
```

---

### 2. Real / Decimal (`float` / `real`)

Números **com casas decimais**. Usados para preços, medidas, notas.

**Exemplos de valores:** `3.14`, `9.8`, `1500.50`, `-0.5`

**Exemplos de uso:**
```
precoIngresso = 25.50
mediaNotas = 8.75
temperaturaAtual = 36.6
```

> ⚠️ Em programação, usamos **ponto** (`.`) como separador decimal, não vírgula!

---

### 3. Texto (`string` / `cadeia de caracteres`)

Qualquer sequência de letras, números e símbolos tratada como **texto**. Sempre fica entre aspas.

**Exemplos de valores:** `"João"`, `"Ação"`, `"12/02/2025"`, `"Olá, mundo!"`

**Exemplos de uso:**
```
nomeUsuario = "Maria"
generoFavorito = "Ficção Científica"
email = "maria@email.com"
```

> 💡 Mesmo que o valor seja um número, **se estiver entre aspas, é texto!**  
> `"42"` é texto. `42` é inteiro. São coisas diferentes para o computador.

---

### 4. Lógico / Booleano (`bool` / `logico`)

Só pode ter **dois valores**: verdadeiro (`true` / `verdadeiro`) ou falso (`false` / `falso`). Parece pouco, mas é o tipo mais usado em decisões!

**Exemplos de valores:** `verdadeiro`, `falso`

**Exemplos de uso:**
```
usuarioLogado = verdadeiro
pesquisaConcluida = falso
maiorDeIdade = verdadeiro
```

---

## 📋 Tabela resumo — cole no caderno!

| Tipo | Palavra-chave | Exemplo de valor | Quando usar |
|---|---|---|---|
| Inteiro | `int` | `17`, `0`, `-5` | Idades, contagens, quantidades |
| Real | `float` | `9.8`, `25.50` | Preços, notas, medidas |
| Texto | `string` | `"Maria"`, `"Ação"` | Nomes, frases, e-mails |
| Lógico | `bool` | `verdadeiro`, `falso` | Condições sim/não |

---

## 📝 Como declarar uma variável

"Declarar" uma variável é o ato de **criar** ela no seu algoritmo, dizendo o nome e o tipo. Em pseudocódigo (a linguagem que usamos para escrever algoritmos antes de programar de verdade), fica assim:

```
DECLARE nomeUsuario: texto
DECLARE idadeUsuario: inteiro
DECLARE mediaNotas: real
DECLARE pesquisaFinalizada: logico
```

Depois de declarada, você **atribui** um valor a ela:

```
nomeUsuario ← "Carlos"
idadeUsuario ← 19
mediaNotas ← 7.5
pesquisaFinalizada ← falso
```

> 💡 A seta `←` significa "recebe". Lê-se: *"nomeUsuario recebe Carlos"*.

---

## 🔄 Variáveis mudam — e isso é o ponto!

Uma variável pode ter seu valor **trocado** ao longo do algoritmo:

```
contador ← 0
(usuário responde à pesquisa)
contador ← contador + 1
```

Lê-se: *"contador recebe o valor atual de contador mais um"*. Se `contador` era `0`, agora passa a ser `1`. Se era `5`, passa a ser `6`.

Isso é como programas contam coisas!

---

## ✏️ Atividade 1 — Identificando tipos (10 min)

**No caderno**, determine qual tipo de dado é mais adequado para cada situação abaixo:

| Informação | Tipo (`int`, `float`, `string` ou `bool`) |
|---|---|
| Nome completo do entrevistado | |
| Quantidade de votos em "Ação" | |
| O usuário é maior de 18 anos? | |
| Nota média dos alunos | |
| Gênero de filme preferido | |
| Número de filmes assistidos no mês | |
| A pesquisa já foi respondida? | |
| Preço da assinatura do streaming | |

---

## ✏️ Atividade 2 — Declarando variáveis (15 min)

### Contexto

Lembra da pesquisa de gênero de filme da aula passada? Agora vamos pensar nas **variáveis que esse sistema precisaria**.

A pesquisa coleta:
- Nome do entrevistado
- Idade
- Nível de escolaridade (Fundamental, Médio, Superior)
- Gênero favorito (Ação, Comédia, Drama ou Ficção Científica)
- Contagem de votos para cada gênero
- Se a pesquisa já foi concluída no dia

**No caderno:**

1. Escreva a declaração de **pelo menos 6 variáveis** que esse sistema usaria
2. Indique o tipo de cada uma
3. Atribua um valor de exemplo para cada variável

**Exemplo de resposta:**
```
DECLARE nomeEntrevistado: texto
nomeEntrevistado ← "Ana Souza"
```

---

## ✏️ Atividade 3 — Algoritmo com variáveis (15 min)

Agora misture tudo: escreva um **algoritmo em pseudocódigo** (pode ser em português, em lista de passos) para o seguinte problema:

> *O sistema deve perguntar o gênero favorito do usuário e adicionar +1 ao contador daquele gênero.*

Use variáveis! Veja um início para te ajudar:

```
DECLARE generoEscolhido: texto
DECLARE contadorAcao: inteiro
DECLARE contadorComedia: inteiro
DECLARE contadorDrama: inteiro
DECLARE contadorFiccao: inteiro

contadorAcao ← 0
contadorComedia ← 0
contadorDrama ← 0
contadorFiccao ← 0

INÍCIO
  Exibir "Qual é o seu gênero favorito? (Ação / Comédia / Drama / Ficção)"
  Ler generoEscolhido

  SE generoEscolhido = "Ação" ENTÃO
    contadorAcao ← contadorAcao + 1
  ... (continue!)
FIM
```

---

## 🔍 Conexão com o fluxograma

Variáveis e fluxogramas andam juntos! Quando você desenhou o fluxograma na aula passada, cada caixa de **entrada** (`/Ler gênero favorito/`) está, por baixo dos panos, **guardando um valor em uma variável**.

Agora, ao criar um fluxograma, você pode **nomear** os dados que estão sendo coletados:

```
  /Ler generoEscolhido (texto)/
          |
          ↓
  < generoEscolhido = "Ação"? >
       /           \
     SIM           NÃO
      |              |
      ↓              ↓
[contadorAcao  < generoEscolhido = "Comédia"? >
← contadorAcao      ...
     + 1]
```

---

## 📌 Resumindo o que aprendemos

- **Variável** é um espaço nomeado na memória para guardar um valor
- Os 4 tipos principais são: **inteiro**, **real**, **texto (string)** e **lógico (bool)**
- Você **declara** a variável (cria ela) e depois **atribui** um valor com `←`
- Variáveis podem **mudar de valor** ao longo do algoritmo — é por isso que se chamam variáveis!
- Escolher o **tipo certo** é essencial: o computador precisa saber o que pode fazer com aquele dado

---

## 🚀 Quer saber mais?

- 📺 [O que é "o tal do Algoritmo"? – DIOLINUX](https://www.youtube.com/watch?v=z1XTcKKRbKM)  
- 📺 [Variáveis e Tipos de Dados – Curso em Vídeo (Gustavo Guanabara)](https://www.youtube.com/watch?v=Mhp5aMTa2fE)
- 📖 CORMEN et al. *Algoritmos - Teoria e Prática*. GEN LTC, 2012.

---

*Educação Profissional Paulista — Técnico em Desenvolvimento de Sistemas | Secretaria da Educação do Estado de São Paulo*
