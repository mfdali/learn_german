# learn_german

# 🇩🇪 Deutsche Grammatik — Dativ & Akkusativ

> Caderno criado com **NotebookLM** para revisão gramatical dos casos do alemão: **Dativ** e **Akkusative**.

🔗 **[Acessar o NotebookLM](https://notebooklm.google.com/notebook/8d50371c-9816-449b-9f41-4abc4b6495ff)**

***

## 📌 Contexto e Objetivos

O alemão possui quatro casos gramaticais (*Fälle*) que determinam a função de um substantivo na frase e impactam diretamente os artigos, pronomes e adjetivos. Entre eles, o **Dativo** e o **Acusativo** são os que mais geram confusão para falantes de português, pois nossa língua não possui marcação morfológica equivalente no uso cotidiano.

### Objetivos de Estudo

- Compreender a diferença funcional entre Dativo (objeto indireto) e Acusativo (objeto direto)
- Memorizar as declinações de artigos definidos, indefinidos e pronomes pessoais em cada caso
- Identificar preposições que regem exclusivamente Dativo, exclusivamente Acusativo e as de dupla regência
- Praticar a construção de frases com verbos que exigem complementos em cada caso
- Construir um repertório de exemplos reutilizáveis para revisão ativa

***

## 📚 Curadoria de Fontes

As seguintes fontes abertas foram selecionadas e carregadas no NotebookLM por cobrirem o conteúdo de forma clara, gratuita e acessível:

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | **Deutsche Welle — Grammatik** | Web / PDF | [dw.com/de/deutsch-lernen](https://www.dw.com/de/deutsch-lernen/grammatik/s-32441) |
| 2 | **Deutsch im Blick — Kapitel 4 (UT Austin)** | PDF aberto | [coerll.utexas.edu/dib](https://coerll.utexas.edu/dib/) |
| 3 | **Lingolia Deutsch — Dativ & Akkusativ** | Web | [deutsch.lingolia.com](https://deutsch.lingolia.com/de/grammatik/kasus) |
| 4 | **Grammatikübungen — ego4u** | Web | [ego4u.com](https://www.ego4u.com/de/cram-up/grammar/case) |
| 5 | **Wikipedia DE — Kasus** | Web | [de.wikipedia.org/wiki/Kasus](https://de.wikipedia.org/wiki/Kasus) |

> **Critério de seleção:** fontes gratuitas e abertas, com linguagem clara para nível B1/B2, contendo tabelas de declinação, exemplos em contexto e exercícios.

***

## 🧪 Engenharia de Prompts e "Cicatrizes"

Esta seção documenta as perguntas estratégicas elaboradas, variações testadas e os aprendizados do processo de extração de conhecimento com o NotebookLM.

### Prompt 1 — Levantamento inicial

```
Qual é a diferença principal entre o Dativo e o Acusativo no alemão?
Explique com exemplos simples e uma tabela comparativa.
```

**Resposta obtida:** O NotebookLM gerou uma explicação clara diferenciando o acusativo como objeto direto (quem/o quê sofre a ação) e o dativo como objeto indireto (para quem/a quem). Incluiu tabela com artigos e exemplos como *Ich sehe **den** Mann* (Akk.) vs. *Ich helfe **dem** Mann* (Dat.).

**Dificuldade encontrada:** A resposta inicial foi genérica. Foi necessário especificar "com base nas fontes carregadas" para obter referências cruzadas entre os materiais.

***

### Prompt 2 — Tabela de declinações

```
Gere uma tabela completa com as declinações dos artigos definidos
e indefinidos para Nominativo, Acusativo e Dativo, separados por gênero
(maskulin, feminin, neutrum, Plural).
```

**Resposta obtida:** Tabela 4×3 gerada com precisão. Destaque para o ponto de maior confusão: no masculino, apenas o Nominativo difere do Acusativo (`der` → `den`); no feminino e neutro, Nominativo e Acusativo são iguais.

**Insight:** Ao pedir para "destacar os casos em que Nominativo e Acusativo diferem", a IA filtrou o ruído e focou no masculino, reduzindo a carga cognitiva de memorização.

***

### Prompt 3 — Preposições com dupla regência

```
Quais preposições em alemão podem reger tanto Dativo quanto Acusativo?
Explique a regra de quando usar cada um e dê exemplos com "in" e "auf".
```

**Resposta obtida:** As *Wechselpräpositionen* (an, auf, hinter, in, neben, über, unter, vor, zwischen) regem:
- **Dativo** → estado/localização (responde *wo?*): *Das Buch liegt **auf dem** Tisch.*
- **Acusativo** → movimento/direção (responde *wohin?*): *Ich lege das Buch **auf den** Tisch.*

**Cicatriz:** Na primeira tentativa, o prompt não incluía "dê exemplos com movimento e localização", e a resposta ficou teórica demais. A segunda versão com exemplos concretos foi muito mais útil.

***

### Prompt 4 — Verbos que regem Dativo

```
Liste os 10 verbos mais comuns do alemão que exigem obrigatoriamente
o complemento no Dativo (não no Acusativo), com exemplos de uso.
```

**Resposta obtida:** Lista incluindo *helfen, danken, gefallen, gehören, folgen, glauben, antworten, vertrauen, begegnen, gratulieren*. Cada um com exemplo de frase.

**Dificuldade:** A IA inicialmente misturou verbos com complemento duplo (Dat. + Akk.) com verbos exclusivamente dativos. Foi preciso refinar: *"Foque apenas nos verbos que têm UM complemento e ele é obrigatoriamente Dativo."*

***

### Prompt 5 — Variação de teste

```
Crie 5 frases incorretas (com erro de caso) e corrija-as, explicando
o motivo da correção.
```

**Resposta obtida:** Exercício de alta qualidade para fixação. Exemplo:
- ❌ *Ich helfe **den** Mann.*
- ✅ *Ich helfe **dem** Mann.* — *helfen* exige Dativo.

**Insight:** Prompts baseados em "erro e correção" são mais memoráveis do que definições abstratas. O NotebookLM manteve consistência com as fontes ao justificar cada correção.

***

## 📖 Miniguia de Estudo

### Resumos Estruturados

#### O Acusativo (Akkusativ)
O acusativo marca o **objeto direto** da frase — aquilo que recebe diretamente a ação do verbo. É o caso que responde à pergunta *Wen? / Was?* (Quem? / O quê?).

- **Artigos definidos:** `den` (mask.) / `die` (fem.) / `das` (neut.) / `die` (pl.)
- **Artigos indefinidos:** `einen` (mask.) / `eine` (fem.) / `ein` (neut.) / `—` (pl.)
- **Mudança visível:** apenas no **masculino** (`der` → `den`, `ein` → `einen`)
- **Preposições exclusivas:** *durch, für, gegen, ohne, um*

**Exemplo:** *Ich kaufe **einen** Kaffee.* (Ich kaufe was? → einen Kaffee)

***

#### O Dativo (Dativ)
O dativo marca o **objeto indireto** da frase — a pessoa ou coisa *para quem* a ação é feita. Responde à pergunta *Wem?* (A quem? / Para quem?).

- **Artigos definidos:** `dem` (mask.) / `der` (fem.) / `dem` (neut.) / `den` (pl.)
- **Artigos indefinidos:** `einem` (mask.) / `einer` (fem.) / `einem` (neut.) / `—` (pl.)
- **Atenção:** No plural, substantivos recebem `-n` final: *den Männer**n***
- **Preposições exclusivas:** *aus, bei, mit, nach, seit, von, zu, gegenüber, außer*

**Exemplo:** *Ich gebe **dem** Mann das Buch.* (Ich gebe wem? → dem Mann)

***

#### Tabela de Declinações

| Caso | Maskulin | Feminin | Neutrum | Plural |
|------|----------|---------|---------|--------|
| **Nominativ** | der / ein | die / eine | das / ein | die / — |
| **Akkusativ** | **den / einen** | die / eine | das / ein | die / — |
| **Dativ** | **dem / einem** | **der / einer** | **dem / einem** | **den / —** |

> 💡 **Dica de memorização:** No masculino, o Nominativo usa `-r` (der/ein**er**); o Dativo usa `-m` (de**m**/eine**m**); o Acusativo usa `-n` (de**n**/eine**n**). No feminino, o Dativo usa `-r` (de**r**/eine**r**).

***

#### Preposições de Dupla Regência (Wechselpräpositionen)

> an · auf · hinter · in · neben · über · unter · vor · zwischen

| Pergunta | Caso | Sentido | Exemplo |
|----------|------|---------|---------|
| *Wo?* (Onde?) | **Dativ** | Estado/localização | *Das Buch liegt auf **dem** Tisch.* |
| *Wohin?* (Para onde?) | **Akkusativ** | Movimento/direção | *Ich lege das Buch auf **den** Tisch.* |

***

### 📝 Glossário de Conceitos

| Termo | Definição |
|-------|-----------|
| **Kasus** | Caso gramatical; indica a função do substantivo na frase |
| **Nominativ** | Caso do sujeito da frase (*wer/was?*) |
| **Akkusativ** | Caso do objeto direto (*wen/was?*) |
| **Dativ** | Caso do objeto indireto (*wem?*) |
| **Genitiv** | Caso de posse (*wessen?*) |
| **Wechselpräposition** | Preposição de dupla regência (Dat. ou Akk. conforme contexto) |
| **Dativverb** | Verbo que exige complemento no Dativo (ex: *helfen*, *danken*) |
| **Deklinationstabelle** | Tabela de declinação de artigos/pronomes por caso e gênero |
| **Maskulin/Feminin/Neutrum** | Gêneros gramaticais do alemão (masculino/feminino/neutro) |
| **Plural** | Forma plural; no Dativo, substantivos recebem sufixo `-n` |
| **Wo-Frage** | Pergunta de localização → resposta em Dativo |
| **Wohin-Frage** | Pergunta de direção/movimento → resposta em Acusativo |

***

### 🔄 Prompts Reutilizáveis para Revisão Futura

Estes prompts podem ser reaproveitados em sessões futuras no NotebookLM ou em outros modelos de linguagem:

```
# Diagnóstico de dúvida específica
"Explique por que o verbo [VERBO] exige [DATIVO/ACUSATIVO] e dê
3 exemplos de frases com ele."

# Geração de exercícios
"Crie 10 frases com lacunas para eu preencher com o artigo correto
(Dativo ou Acusativo). Nível B1. Inclua o gabarito ao final."

# Erro e correção
"Aqui estão 5 frases que escrevi. Identifique erros de caso gramatical
e explique cada correção: [FRASES]"

# Comparação contextual
"Mostre a mesma frase com [PREPOSIÇÃO] em Dativo e em Acusativo,
explicando como o significado muda."

# Mnêmico e resumo
"Crie uma regra mnemônica em português para memorizar as terminações
dos artigos no Dativo masculino e feminino."

# Quiz de revisão
"Faça 5 perguntas de múltipla escolha sobre Dativo e Acusativo,
com 4 alternativas cada. Revele as respostas ao final."
```

***

## 🛠️ Ferramentas Utilizadas

- **[NotebookLM](https://notebooklm.google.com)** — Google, 2024
- Fontes abertas listadas na seção de Curadoria

***

*Repositório criado como entrega do desafio de caderno temático com NotebookLM.*
