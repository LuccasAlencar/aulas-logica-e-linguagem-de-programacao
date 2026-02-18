**Aula 13: Peradores Relacionais**
=====================================

**Objetivos de Aprendizagem**
---------------------------

* Conhecer estruturas de decisão composta a partir da linguagem Python no contexto de lógica de programação;
* Compreender a estrutura complementar elif para regras de tomada de decisão;
* Aplicar operadores relacionais e lógicos na construção de expressões condicionais em algoritmos e pseudocódigos.

**Cronograma**
-------------

| Tempo | Atividade | Tipo |
|-------|-----------|------|
| 0-10min | Introdução | Intro |
| 10-20min | Desenvolvimento | Conteúdo |
| 20-30min | Atividade Prática | Prática |
| 30-40min | Discussão e Revisão | Discussão |
| 40-50min | Fechamento | Fechamento |

**Tópicos Principais**
-------------------

1. Estrutura If e Else
2. Estrutura Elif
3. Exemplos de Uso de Estruturas Condicionais Compostas

**Momentos Interativos Planejados**
--------------------------------

* 15min: Discussão sobre a importância de estruturas de decisão composta em programação
* 35min: Atividade prática - Aplicação de estruturas condicionais compostas em um exemplo real

**Fluxo Pedagógico**
------------------

1. Introdução: Apresentação dos objetivos da aula e revisão prévia dos conceitos
2. Desenvolvimento: Explicação dos conceitos de estruturas de decisão composta e estrutura elif
3. Prática: Atividade prática que aplique os conceitos aprendidos
4. Fechamento: Discussão e revisão dos conceitos aprendidos e avaliação dos objetivos alcançados

### Introdução (0-10min)
Olá, estudantes! Hoje vamos explorar as estruturas de decisão composta em Python, que são fundamentais para criar programas com lógica condicional mais complexa. Você já usou estruturas de decisão em algum projeto? Compartilhe suas experiências!

### Desenvolvimento (10-20min)
#### Estrutura If e Else
A estrutura `if` é usada para executar um bloco de código quando uma determinada condição é verdadeira. Veja o exemplo:

```python
idade = 18
if idade >= 18:
    print("Você é maior de idade.")
```

E a estrutura `else` é usada para especificar um bloco de código caso a condição do `if` não seja satisfeita. Veja o exemplo:

```python
idade = 15
if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

#### Estrutura Elif
A estrutura `elif` é usada para verificar múltiplas condições em sequência, permitindo que o programa tome diferentes ações dependendo de qual condição é satisfeita primeiro. Veja o exemplo:

```python
idade = 15
if idade >= 18:
    print("Você é maior de idade.")
elif idade < 18 and idade >= 13:
    print("Você é um adolescente.")
else:
    print("Você é uma criança.")
```

### Atividade Prática (20-30min)
Vamos criar um programa que forneça recomendações de atividades baseadas na temperatura atual. Use a estrutura `elif` para criar condições que sejam satisfeitas em sequência.

```python
temperatura = 30
if temperatura >= 30:
    print("Vá à praia!")
elif temperatura >= 20:
    print("Um dia perfeito para um passeio no parque.")
elif temperatura >= 10:
    print("Que tal um filme em casa?")
else:
    print("Melhor ficar em casa, está muito frio lá fora.")
```

### Discussão e Revisão (30-40min)
Vamos discutir a importância de estruturas de decisão composta em programação e como elas podem ser usadas para criar programas mais complexos. Além disso, vamos revisar os conceitos aprendidos e responder a perguntas.

### Fechamento (40-50min)
Vamos recapitular os conceitos aprendidos e avaliar os objetivos alcançados. Além disso, vamos discutir como as estruturas de decisão composta podem ser usadas em projetos reais e como elas podem ser aplicadas em diferentes contextos.

**REFINAMENTOS**

* Coerência e Fluxo: Verifique se a progressão de ideias está lógica e elimine repetições desnecessárias.
* Qualidade Pedagógica: Melhore exemplos tornando-os mais práticos e relevantes, e ajuste atividades para serem mais engajadoras.
* Clareza e Didática: Simplifique explicações complexas e adicione analogias onde apropriado.
* Formatação e Visual: Garantir uso consistente de emojis e melhorar organização de tabelas.
* Engajamento: Tornar introduções mais cativantes e adicionar elementos de gamificação onde possível.
* Completude: Verifique se todos os tópicos prometidos foram abordados e adicione dicas extras para o professor.