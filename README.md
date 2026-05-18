# learn_german

# 🇩🇪 Deutsche Grammatik — Dativ & Akkusativ

> Caderno temático criado com **NotebookLM** para revisão sistemática dos casos gramaticais do alemão, com foco em **Dativo** e **Acusativo**.

🔗 **[Acessar o NotebookLM](https://notebooklm.google.com/notebook/8d50371c-9816-449b-9f41-4abc4b6495ff)**

***

## 📌 Contexto e Objetivos

O alemão possui quatro casos gramaticais (*Fälle*) que determinam a função de um substantivo na frase e impactam diretamente os artigos, pronomes e adjetivos. Entre eles, o **Dativo** e o **Acusativo** são os que mais geram confusão para falantes de português, pois nossa língua não possui marcação morfológica equivalente no uso cotidiano.

O caderno cobre os quatro casos (Nominativo, Genitivo, Dativo e Acusativo), com atenção especial às nuances das preposições de direção *nach*, *in* e *zu* — que se aplicam a contextos geográficos e de edificações distintos — além de tópicos avançados como orações relativas, conjunções temporais e partículas modais para uma fala mais natural.

### Objetivos de Estudo

- Compreender a diferença funcional entre os quatro casos gramaticais
- Dominar as declinações de artigos e pronomes em cada caso
- Distinguir preposições que regem exclusivamente Dativo, exclusivamente Acusativo e as de dupla regência (*Wechselpräpositionen*)
- Entender o uso das preposições de direção *nach*, *in* e *zu* em contexto
- Combinar memorização de tabelas com prática consistente para fixação real

***

## 📚 Curadoria de Fontes

As seguintes fontes abertas foram selecionadas e carregadas no NotebookLM:

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | **Deutsche Welle — Grammatik** | Web / PDF | [dw.com/de/deutsch-lernen](https://www.dw.com/de/deutsch-lernen/grammatik/s-32441) |
| 2 | **Deutsch im Blick — UT Austin** | PDF aberto | [coerll.utexas.edu/dib](https://coerll.utexas.edu/dib/) |
| 3 | **Lingolia Deutsch — Kasus** | Web | [deutsch.lingolia.com](https://deutsch.lingolia.com/de/grammatik/kasus) |
| 4 | **Grammatikübungen — ego4u** | Web | [ego4u.com](https://www.ego4u.com/de/cram-up/grammar/case) |
| 5 | **Wikipedia DE — Kasus** | Web | [de.wikipedia.org/wiki/Kasus](https://de.wikipedia.org/wiki/Kasus) |

> **Critério de seleção:** fontes gratuitas e abertas, com linguagem clara para nível A2/B1, contendo tabelas de declinação, exemplos em contexto e exercícios práticos.

***

## 🧪 Engenharia de Prompts e "Cicatrizes"

Esta seção documenta as perguntas estratégicas elaboradas no NotebookLM, as variações testadas e os aprendizados do processo.

### Prompt 1 — Levantamento inicial dos casos

```
Qual é a diferença principal entre o Dativo e o Acusativo no alemão?
Explique com exemplos simples e uma tabela comparativa.
```

**Resposta obtida:** Explicação diferenciando o Acusativo como objeto direto (*wen/was?*) e o Dativo como objeto indireto (*wem?*), com tabela de artigos e exemplos contextualizados.

**Cicatriz:** A resposta inicial foi genérica. Foi necessário adicionar "com base nas fontes carregadas" para obter referências cruzadas entre os materiais e respostas mais precisas.

***

### Prompt 2 — Tabela de declinações

```
Gere uma tabela completa com as declinações dos artigos definidos e indefinidos
para Nominativo, Acusativo e Dativo, separados por gênero
(maskulin, feminin, neutrum, Plural).
```

**Resposta obtida:** Tabela 4×3 com as formas de todos os artigos. Destaque para o ponto crítico: no masculino, apenas o Nominativo difere do Acusativo (`der` → `den`); no feminino e neutro, as formas são idênticas.

**Insight:** Pedir para "destacar os casos em que Nominativo e Acusativo diferem" filtrou o excesso de informação e focou no ponto de maior confusão.

***

### Prompt 3 — Preposições de direção

```
Explique as diferenças entre "nach", "in" e "zu" como preposições de direção.
Em quais contextos cada uma é usada? Dê exemplos práticos.
```

**Resposta obtida:** 
- *nach* → países e cidades sem artigo (*Ich fahre nach Berlin.*)
- *in* → países com artigo e destinos físicos com ideia de "dentro" (*Ich gehe in die Schule.*)
- *zu* → pessoas e edificações específicas (*Ich fahre zum Bahnhof.*)

**Cicatriz:** Na primeira tentativa, sem especificar "preposições de direção", a IA misturou preposições de localização com as de movimento. Refinar o escopo foi essencial.

***

### Prompt 4 — Preposições com dupla regência

```
Quais preposições em alemão podem reger tanto Dativo quanto Acusativo?
Explique a regra com exemplos usando "in" e "auf".
```

**Resposta obtida:** As *Wechselpräpositionen* (an, auf, hinter, in, neben, über, unter, vor, zwischen) regem:
- **Dativo** → estado/localização (*wo?*): *Das Buch liegt auf **dem** Tisch.*
- **Acusativo** → movimento/direção (*wohin?*): *Ich lege das Buch auf **den** Tisch.*

**Cicatriz:** Sem pedir exemplos com "movimento e localização" explicitamente, a resposta ficou teórica demais para ser útil na prática.

***

### Prompt 5 — Quiz (entrega gerada pelo NotebookLM)

```
Create a quiz in german language to help me understand and truly learn
dative and accusative cases.
The quiz must have 10 questions (maximum).
The quiz must focus on a student A2/B1 level that sometimes forget
the grammar rules learned during A1.
```

**Resposta obtida:** Quiz com 10 questões de lacuna em alemão, cobrindo artigos, pronomes e preposições em contexto de frases do cotidiano. Nível calibrado para A2/B1, com gabarito ao final.

**Insight:** Especificar o nível e o perfil do estudante ("que às vezes esquece regras do A1") resultou em frases mais simples no vocabulário, mas desafiadoras na gramática — exatamente o equilíbrio necessário.

***

### Prompt 6 — Infográfico (entrega gerada pelo NotebookLM)

```
Use a clean and minimalist way to teach accusative and dative german cases
to a student level A2.
```

**Resposta obtida:** Infográfico visual com tabelas de declinação simplificadas, separação por cores entre Dativo e Acusativo, lista das preposições exclusivas de cada caso e exemplos de frases curtas.

**Insight:** O comando "clean and minimalist" foi determinante para evitar sobrecarga de informação — o NotebookLM reduziu o conteúdo ao essencial para o nível A2.

***

## 📖 Miniguia de Estudo

### Resumos Estruturados

#### Os Quatro Casos (*Fälle*)

O alemão usa casos para marcar a função de cada substantivo na frase. Os quatro casos são:

| Caso | Pergunta | Função | Exemplo |
|------|----------|--------|---------|
| **Nominativ** | *Wer/Was?* | Sujeito | ***Der** Mann schläft.* |
| **Akkusativ** | *Wen/Was?* | Objeto direto | *Ich sehe **den** Mann.* |
| **Dativ** | *Wem?* | Objeto indireto | *Ich helfe **dem** Mann.* |
| **Genitiv** | *Wessen?* | Posse | *Das Auto **des** Mannes.* |

***

#### Tabela de Declinações

| Caso | Maskulin | Feminin | Neutrum | Plural |
|------|----------|---------|---------|--------|
| **Nominativ** | der / ein | die / eine | das / ein | die / — |
| **Akkusativ** | **den / einen** | die / eine | das / ein | die / — |
| **Dativ** | **dem / einem** | **der / einer** | **dem / einem** | **den / —** |

> 💡 **Dica:** No masculino, o Dativo usa `-m` (de**m**) e o Acusativo usa `-n` (de**n**). No feminino, o Dativo usa `-r` (de**r**). No plural dativo, os substantivos recebem sufixo `-n`.

***

#### Preposições de Direção: *nach*, *in*, *zu*

| Preposição | Uso | Exemplo |
|------------|-----|---------|
| **nach** | Países e cidades **sem** artigo | *Ich fahre nach Berlin / nach Deutschland.* |
| **in** | Países **com** artigo; destinos com sentido de "dentro" | *Ich fahre in die Türkei. / Ich gehe in die Schule.* |
| **zu** | Pessoas e edificações específicas | *Ich fahre zum Bahnhof. / Ich gehe zur Ärztin.* |

***

#### Preposições Exclusivas por Caso

**Somente Acusativo:** *durch, für, gegen, ohne, um*

**Somente Dativo:** *aus, bei, mit, nach, seit, von, zu, gegenüber, außer*

**Dupla regência (*Wechselpräpositionen*):** *an, auf, hinter, in, neben, über, unter, vor, zwischen*
- → *wo?* (onde?) = **Dativo** | → *wohin?* (para onde?) = **Acusativo**

***

### 📝 Glossário de Conceitos

| Termo | Definição |
|-------|-----------|
| **Kasus** | Caso gramatical; marca a função do substantivo na frase |
| **Nominativ** | Caso do sujeito (*wer/was?*) |
| **Akkusativ** | Caso do objeto direto (*wen/was?*) |
| **Dativ** | Caso do objeto indireto (*wem?*) |
| **Genitiv** | Caso de posse (*wessen?*) |
| **Wechselpräposition** | Preposição de dupla regência (Dat. ou Akk. conforme contexto) |
| **Dativverb** | Verbo que exige complemento exclusivamente no Dativo (ex: *helfen*, *danken*) |
| **Deklinationstabelle** | Tabela de declinação de artigos por caso e gênero |
| **Wo-Frage** | Pergunta de localização → resposta em Dativo |
| **Wohin-Frage** | Pergunta de direção/movimento → resposta em Acusativo |
| **Modalpartikel** | Partícula modal que suaviza ou matiza o tom da frase (ex: *doch, ja, mal*) |
| **Relativsatz** | Oração relativa; exige atenção ao caso do pronome relativo |

***

### 🔄 Prompts Reutilizáveis para Revisão Futura

```
# Quiz de prática
Create a quiz in german language to help me understand and truly learn
dative and accusative cases.
The quiz must have 10 questions (maximum).
The quiz must focus on a student A2/B1 level that sometimes forget
the grammar rules learned during A1.

# Infográfico / resumo visual
Use a clean and minimalist way to teach accusative and dative german
cases to a student level A2.

# Diagnóstico de dúvida específica
Explique por que o verbo [VERBO] exige [DATIVO/ACUSATIVO] e dê
3 exemplos de frases com ele.

# Erro e correção
Aqui estão 5 frases que escrevi. Identifique erros de caso gramatical
e explique cada correção: [FRASES]

# Preposições em contexto
Mostre a mesma frase com [PREPOSIÇÃO] em Dativo e em Acusativo,
explicando como o significado muda.

# Conjunções temporais
Explique as conjunções temporais mais usadas no alemão A2/B1
(als, wenn, nachdem, bevor) com exemplos de frases do cotidiano.
```

***

## 🛠️ Ferramentas Utilizadas

- **[NotebookLM](https://notebooklm.google.com)** — Google, 2024
- Fontes abertas listadas na seção de Curadoria

***

*Repositório criado como entrega do desafio de caderno temático com NotebookLM.*
