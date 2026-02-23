**Aula 20: Aplicações com SE (Atividade Prática)**

## Objetivos de Aprendizagem
- Desenvolver habilidades em pensamento lógico e estruturas de decisão compostas.
- Implementar a estrutura de decisão composta utilizando condições lógicas e operadores relacionais.
- Desenvolver programas simples utilizando estrutura SE aplicando condições reais.

## Cronograma
| Tempo | Atividade | Tipo |
|-------|-----------|------|
| 0-10min | Apresentação do tema e contextualização | Introdução |
| 10-25min | Exposição e explicação da estrutura de decisão composta | Conteúdo |
| 25-35min | Atividade prática: Desenvolvimento de programas utilizando estrutura SE | Prática |
| 35-40min | Discussão e correção de erros | Discussão |
| 40-50min | Fechamento e revisão dos conceitos | Fechamento |

## Tópicos Principais
1. Estrutura de Decisão Composta
2. Condições Lógicas e Operadores Relacionais
3. Desenvolvimento de Programas Utilizando Estrutura SE

## Momentos Interativos Planejados
- 20min: Discussão sobre a aplicabilidade da estrutura de decisão composta em problemas reais.
- 40min: Atividade prática em grupo: Desenvolvimento de programas utilizando estrutura SE.

## Fluxo Pedagógico
1. Introdução: Apresentação do tema e contextualização.
2. Desenvolvimento: Exposição e explicação da estrutura de decisão composta e condições lógicas.
3. Prática: Atividade prática: Desenvolvimento de programas utilizando estrutura SE.
4. Fechamento: Discussão e correção de erros, revisão dos conceitos.

### Conteúdo Didático

#### Estrutura de Decisão Composta

A estrutura de decisão composta é uma forma de tomar decisões em algoritmos, utilizando condições lógicas e operadores relacionais. Ela permite que o programador defina condições mais complexas para tomar decisões, utilizando operadores como `OU` e `E`.

Exemplo:

```python
if condicao1 OU condicao2:
    # Código a executar se a condicao1 for verdadeira OU a condicao2 for verdadeira
```

#### Condições Lógicas e Operadores Relacionais

As condições lógicas são utilizadas para definir as condições que devem ser verificadas para tomar decisões. Os operadores relacionais são utilizados para combinar as condições lógicas.

Exemplo:

```python
if 5 > 3:
    # Código a executar se a condicao for verdadeira
```

#### Desenvolvimento de Programas Utilizando Estrutura SE

A estrutura de decisão composta pode ser utilizada para desenvolver programas que tomam decisões mais complexas.

Exemplo:

```python
if idade >= 18:
    # Código a executar se a idade for maior ou igual a 18
elif idade < 18:
    # Código a executar se a idade for menor que 18
```

### Atividade Prática

#### Exercício 1

Uma academia de artes tem um processo de admissão que inclui o envio de um portfólio e uma audição. A academia admite candidatos que:

* Tenham um portfólio forte OU;
* Tenham uma audição excelente e tenham feito pelo menos 2 anos de treinamento prévio.

Escreva um programa que determine se um candidato será admitido ou não.

```python
portfolio_forte = False
audicao_excelente = True
treinamento_previo_anos = 2

if portfolio_forte or (audicao_excelente and treinamento_previo_anos >= 2):
    print("Parabéns, você foi admitido na academia!")
else:
    print("Infelizmente, você não foi admitido na academia.")
```

#### Exercício 2

Um banco oferece empréstimos para clientes que:

* Tenham uma renda mensal de pelo menos R$ 2000 E;
* Tenham um score de crédito de pelo menos R$ 600 OU;
* Tenham um fiador com um score de crédito de pelo menos R$ 700.

Escreva um programa que determine se um cliente é elegível para um empréstimo.

```python
renda_mensal = 2500
score_credito = 650
fiador_score_credito = 680

if renda_mensal >= 2000 and (score_credito >= 600 or fiador_score_credito >= 700):
    print("Você é elegível para o empréstimo.")
else:
    print("Você não é elegível para o empréstimo.")
```

### Discussão e Correção de Erros

Agora é hora de discutir e corrigir os exercícios!

* Qual foi o resultado do seu programa?
* Você encontrou algum erro?
* Como você pode melhorar o programa?

### Fechamento e Revisão dos Conceitos

Agora que você completou a atividade prática, é hora de revisar os conceitos!

* Qual é a estrutura de decisão composta?
* Qual é o uso das condições lógicas e operadores relacionais?
* Como você pode utilizar a estrutura de decisão composta em programas reais?

**REFINAMENTOS OBRIGATÓRIOS:**

1. **Coerência e Fluxo**
   - Verificar se a progressão de ideias está lógica
   - Garantir transições suaves entre seções
   - Eliminar repetições desnecessárias

2. **Qualidade Pedagógica**
   - Melhorar exemplos tornando-os mais práticos e relevantes
   - Refinar perguntas para discussão (mais provocativas)
   - Ajustar atividades para serem mais engajadoras
   - Garantir alinhamento com objetivos de aprendizagem

3. **Clareza e Didática**
   - Simplificar explicações complexas
   - Adicionar analogias onde apropriado
   - Melhorar instruções de atividades
   - Tornar linguagem mais acessível

4. **Formatação e Visual**
   - Garantir uso consistente de emojis
   - Melhorar organização de tabelas
   - Adicionar destaques visuais em pontos-chave
   - Verificar hierarquia de títulos

5. **Engajamento**
   - Tornar introduções mais cativantes
   - Adicionar elementos de gamificação onde possível
   - Melhorar chamadas para ação
   - Criar senso de progressão

6. **Completude**
   - Verificar se todos os tópicos prometidos foram abordados
   - Adicionar dicas extras para o professor
   - Incluir sugestões de adaptação se necessário

**IMPORTANTE:**
- NÃO mude a estrutura fundamental
- NÃO adicione seções novas
- APENAS refine, melhore e pula o que já está bom
- Mantenha o mesmo formato Markdown
- Foco em QUALIDADE, não quantidade

Retorne o plano de aula REFINADO E POLIDO.