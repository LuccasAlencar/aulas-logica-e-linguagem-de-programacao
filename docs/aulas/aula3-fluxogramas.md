# Aula 3 — Fluxogramas e Representação Visual

> **Componente:** Lógica e Linguagem de Programação  
> **Unidade:** Estrutura Básica  
> **Duração:** 50 minutos  

---

## 🧠 O que você vai aprender hoje

Na aula passada você conheceu o que é um algoritmo e até tentou criar um. Mas escrever passos em texto pode ficar confuso quando o problema começa a ter **decisões** — *"e se o usuário errar a senha? E se não tiver saldo?"*.

Hoje você vai aprender a **desenhar** esses passos usando uma linguagem visual universal: o **fluxograma**. É a ferramenta que programadores, designers e analistas usam para planejar um sistema antes de escrever uma linha de código.

---

## 🗺️ O que é um fluxograma?

Um fluxograma é um **diagrama** que representa visualmente a sequência de passos de um processo ou algoritmo. Em vez de escrever "se o usuário digitar a senha certa, deixa entrar; se não, mostra erro", você **desenha** isso com formas e setas.

É como o GPS do seu código: antes de sair dirigindo (programando), você planeja o caminho.

---

## 🔷 Os símbolos padrão

Existe uma notação universal. No seu caderno, copie essa tabela:

| Símbolo | Forma | O que representa |
|---|---|---|
| **Oval / Cápsula** | `( Início )` ou `( Fim )` | Início ou fim do processo |
| **Retângulo** | `[ Processar dados ]` | Uma ação ou processamento |
| **Losango** | `< Condição? >` | Uma decisão (sim/não, verdadeiro/falso) |
| **Paralelogramo** | `/Ler nome do usuário/` | Entrada ou saída de dados |
| **Seta** | `→` | Indica a direção do fluxo |

> 💡 **Dica:** Você não precisa ser artista! Um retângulo torto ainda é um retângulo. O que importa é a **lógica**, não o desenho perfeito.

---

## 📐 Regras básicas

1. **Todo fluxograma começa com um oval de INÍCIO e termina com um oval de FIM.**
2. **As setas nunca ficam sem destino** — todo bloco precisa de uma saída.
3. **O losango sempre tem duas saídas:** geralmente `Sim` e `Não`.
4. O fluxo segue de **cima para baixo** e da **esquerda para a direita** (convenção mais comum).

---

## 🎂 Exemplo 1 — Fazendo um bolo (revisando a última aula)

Na aula anterior vimos o algoritmo do bolo em lista. Agora veja como fica em fluxograma:

```
        ( INÍCIO )
             |
             ↓
    [ Preaquecer o forno ]
             |
             ↓
    [ Separar os ingredientes ]
             |
             ↓
    [ Misturar ingredientes secos ]
             |
             ↓
    [ Adicionar ingredientes líquidos ]
             |
             ↓
    [ Bater até massa homogênea ]
             |
             ↓
    [ Untar a forma e despejar a massa ]
             |
             ↓
    [ Levar ao forno ]
             |
             ↓
    < Palito saiu limpo? >
       /             \
     NÃO             SIM
      |               |
      ↓               ↓
[Aguardar mais  [ Retirar do forno ]
  10 minutos ]        |
      |               ↓
      └──────→ [ Deixar esfriar ]
                      |
                      ↓
               [ Desenformar ]
                      |
                      ↓
                  ( FIM )
```

Perceba o losango `Palito saiu limpo?` — ele representa uma **decisão**. O fluxo pode seguir por dois caminhos diferentes dependendo da resposta. Isso é o coração da lógica de programação!

---

## 💻 Exemplo 2 — Login num aplicativo

Agora um exemplo mais próximo do mundo real. Imagine o fluxo de login de um app:

```
          ( INÍCIO )
               |
               ↓
   /Usuário digita e-mail e senha/
               |
               ↓
   < Dados estão corretos? >
        /              \
      NÃO              SIM
       |                |
       ↓                ↓
[ Mostrar mensagem  [ Abrir tela  ]
  "Senha inválida" ]   principal  ]
       |                |
       ↓                ↓
[ Limpar campo     ( FIM do fluxo )
     de senha ]
       |
       ↓
  (volta para o
  início do login)
```

---

## ✏️ Atividade 1 — Leitura de fluxograma (5 min)

**No caderno**, responda:

Observe o fluxograma de login acima e responda:

1. O que acontece quando o usuário erra a senha?
2. Existe algum ponto onde o fluxo pode se repetir? Qual?
3. Quantos caminhos possíveis existem a partir do losango de decisão?

---

## ✏️ Atividade 2 — Seu primeiro fluxograma (25 min)

### Contexto

Você está num processo seletivo para uma **empresa de streaming de filmes** (tipo Netflix) na área de análise de dados. A empresa precisa de um sistema que **pesquise a preferência de gênero de filme** dos usuários.

### O que o sistema precisa fazer:

- Perguntar ao usuário **qual gênero ele prefere**: Ação, Comédia, Drama ou Ficção Científica
- Registrar a resposta
- Perguntar a **faixa etária** do usuário
- Perguntar o **nível de escolaridade**
- Ao final, exibir um **resumo** das respostas coletadas

### Sua missão

**No caderno**, desenhe um fluxograma que represente esse processo, seguindo os símbolos que aprendemos. Lembre-se:

- Use oval para início e fim
- Use paralelogramo para entrada de dados (perguntas ao usuário)
- Use retângulo para ações (registrar resposta, exibir resumo)
- Use losango se quiser representar alguma decisão (ex: *"Deseja responder mais um usuário?"*)
- Conecte tudo com setas

> 💡 **Dica extra:** Comece simples. Desenhe o fluxo mais básico primeiro e depois adicione detalhes.

---

## 🔍 Checklist do seu fluxograma

Antes de entregar, confira:

- [ ] Tem um `INÍCIO` e um `FIM`?
- [ ] As setas estão indicando a direção correta?
- [ ] Todo losango (decisão) tem duas saídas?
- [ ] O fluxo faz sentido se você "percorrer" seguindo as setas?

---

## 📌 Resumindo o que aprendemos

- Um **fluxograma** é a representação visual de um algoritmo
- Existem **símbolos padrão**: oval (início/fim), retângulo (processo), losango (decisão), paralelogramo (entrada/saída)
- O losango é o símbolo mais poderoso — ele representa **escolhas**, que são a base da lógica de programação
- Desenhar o fluxo **antes** de programar evita erros e poupa tempo

---

## 🚀 Quer saber mais?

- 📺 [O que é "o tal do Algoritmo"? – DIOLINUX](https://www.youtube.com/watch?v=z1XTcKKRbKM)
- 📺 [Como ensinar programação para uma criança – Baricentro da Mente](https://www.youtube.com/watch?v=pdhqwbUWf4U)
- 📖 CORMEN et al. *Algoritmos - Teoria e Prática*. GEN LTC, 2012.

---

*Educação Profissional Paulista — Técnico em Desenvolvimento de Sistemas | Secretaria da Educação do Estado de São Paulo*
