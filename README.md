<h1>Análise de Linguagem Ofensiva no Twitter</h1>
<p>Este trabalho é baseado na tarefa <b>OffensEval</b> que acontecem no âmbito das competições anuais de <b>Semântica Computacional - SEMEVAL</b>, edições de 2019 e 2020.</p>

### Seguem links para consulta:

<a href="https://alt.qcri.org/semeval2019/">SemEval 2019</a>

<a href="https://competitions.codalab.org/competitions/20011">OffensEval 2019</a>

A linguagem ofensiva é massivamente difundida nas mídias sociais. Os indivíduos freqüentemente se aproveitam do anonimato nas comunicações mediadas por computador, para se envolver em comportamentos, os quais não considerariam na vida real. Comunidades on-line, plataformas de mídia social e empresas de tecnologia têm investido fortemente em maneiras de lidar com linguagem ofensiva para evitar comportamentos abusivos nas mídias sociais.

Uma das estratégias mais eficazes para resolver esse problema é usar métodos computacionais para identificar ofensas, agressões e discursos de ódio no conteúdo gerado pelo usuário (por exemplo, postagens, comentários, microblogs etc.). Em Processamento de Linguagem Natural (PLN), considera-se esta uma aplicação de classificação textual (Text Classification)

### Objetivos
Neste projeto, são propostas duas abordagens para analisar discursos ofensivos em tweets:

<b>(A) Subtarefa A - Identificação de Linguagem Ofensiva</b>

- (NOT) Not Offensive - o tweet ou texto NÃO contem ofensa ou profanidade.
- (OFF) Offensive - o tweet ou texto contem qualquer tipo de linguagem não-aceitável (ofensa ou profanidade) ou uma ofensa direcionada (velada ou direta).

<b>(B) Subtarefa B: Categorização dos tipos de ofensa</b>

- (TIN) Targeted Insult and Threats - o tweet contem um insulto ou ameaça a um indivíduo, um grupo ou outros.
- (UNT) Untargeted - o tweet contem insultos, palavrões, ou ofensas não-direcionadas.

### Datasets
<b>Dados de Treinamento (arquivo texto simples "olid-training-v1.0.tsv")</b>

Um conjunto com 13.240 tweets anotados com os seguintes dados:

- id do tweet
- texto do tweet
- label para subtarefa A
- label para subtarefa B
- label para subtarefa C (desconsiderar)

### Entregas

<b>Pré-processamento dos textos:</b>

- Tokenização
- Lematização
- POS Tagging
- Normalização (hashtags, menções, emojis e símbolos especiais)
- NER (entidades nomeadas)
- Remoção stop-words

<b>Representação Semântica:</b>

- Uso de bases de conhecimento externas
- Identificação de tópicos
- Representação vetorial das palavras e textos

<b>Analise da Linguagem Ofensiva - Subtarefas A e B:</b>

- Resultado da subtarefa A para um conjunto de teste a ser fornecido
- Resultado da subtarefa B para um conjunto de teste a ser fornecido
