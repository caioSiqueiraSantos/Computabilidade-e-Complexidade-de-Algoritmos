## Identificação do Grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | Computabilidade e Complexidade de Algoritmos / Ciência da Computação |
| Projeto de Pesquisa / IC | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientador(a) | Andrea Ono Sakai |
| Data de entrega desta etapa | 12/09/2026 |
| Integrantes do grupo | Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires, Matheus Henrique da Trindade |
| Tema (da etapa "a") | Análise comparativa de complexidade, escalabilidade, uso de memória e qualidade dos algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em sistemas RAG para suporte interno de TI. |

## PARTE 1 — DEFINIR O OBJETIVO GERAL

### 1.1 Tema específico do grupo

**Pergunta:** Qual foi o tema específico que o grupo definiu?

> Resposta: Análise comparativa de complexidade, escalabilidade, uso de memória e qualidade dos algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em sistemas RAG para suporte interno de TI.

### 1.2 Passo a passo para chegar ao objetivo geral

**Passo 1 — Delimitação do tema**
Delimitem o tema específico por área, tempo, espaço ou aplicação.

> Resposta: O tema delimita-se na área de Ciência da Computação (subárea de Computabilidade e Complexidade de Algoritmos aplicada à Inteligência Artificial), concentrando-se na análise teórica e comparativa de três algoritmos fundamentais de busca vetorial: k-NN exato por força bruta (Flat), HNSW (*Hierarchical Navigable Small World* baseado em grafos de proximidade multicamadas) e IVF (*Inverted File Index* baseado em particionamento do espaço em clusters de Voronoi). A aplicação e o contexto restringem-se ao dimensionamento de chatbots e assistentes virtuais baseados em RAG (*Retrieval-Augmented Generation*) para suporte interno de TI (Helpdesk), comparando-os sob os critérios de complexidade assintótica de tempo (construção e consulta/latência), complexidade de espaço (pegada de memória RAM) e qualidade da recuperação (*Recall@k*).

**Passo 2 — Formulação da problemática**
Transformem o tema em uma pergunta que expresse o problema de pesquisa.

> Resposta: Como a literatura compara a complexidade computacional, o uso de memória, a escalabilidade e a qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte interno de TI?

**Passo 3 — Transformar a pergunta em objetivo geral**
Reescrevam a pergunta como uma afirmação, usando um verbo no infinitivo.

> Resposta: Analisar comparativamente a complexidade computacional (tempo e espaço), o consumo de memória, a escalabilidade e a qualidade de recuperação (Recall@k e latência) dos algoritmos de busca vetorial k-NN exato, HNSW e IVF na recuperação de informação de sistemas RAG para suporte interno de TI, com o propósito de evidenciar os principais trade-offs algorítmicos necessários ao dimensionamento eficiente de bases de conhecimento corporativas.

**Passo 4 — Ajustes finais**
Revisem o objetivo geral seguindo os critérios abaixo:

- [x] É claro, direto e mensurável?
- [x] Evitei verbos fracos como "estudar" ou "conhecer"?
- [x] Usei um verbo forte (explorar, analisar, investigar, compreender, avaliar, propor, desenvolver, aplicar, identificar)?

**Modelo genérico de referência:**
> "[Verbo no infinitivo] a aplicação de [conceito ou técnica] em [contexto específico], com o propósito de [finalidade principal]."

**Outros exemplos de objetivos gerais (referência):**
- Investigar o uso de árvores de decisão para prever exportações de vinho no Brasil, com base em dados da Embrapa entre 2000 e 2025.
- Analisar o impacto da classificação automática de vinhos finos e de mesa por meio de algoritmos de inteligência artificial, a fim de apoiar estratégias de exportação.
- Desenvolver um modelo computacional baseado em árvore binária de busca para otimizar a recomendação de rotas de ambulância em cenários urbanos.

### 1.3 Respostas finais da Parte 1

**1) Qual a problemática?**

> Resposta: Como a literatura compara a complexidade computacional, o uso de memória, a escalabilidade e a qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte interno de TI?

**2) Qual o objetivo geral?**

> Resposta: Analisar comparativamente a complexidade computacional (tempo e espaço), o consumo de memória, a escalabilidade e a qualidade de recuperação (Recall@k e latência) dos algoritmos de busca vetorial k-NN exato, HNSW e IVF na recuperação de informação de sistemas RAG para suporte interno de TI, com o propósito de evidenciar os principais trade-offs algorítmicos necessários ao dimensionamento eficiente de bases de conhecimento corporativas.

---

## PARTE 2 — DEFININDO OS OBJETIVOS ESPECÍFICOS

### 2.1 Objetivo geral pesquisado

> Resposta: Analisar comparativamente a complexidade computacional (tempo e espaço), o consumo de memória, a escalabilidade e a qualidade de recuperação (Recall@k e latência) dos algoritmos de busca vetorial k-NN exato, HNSW e IVF na recuperação de informação de sistemas RAG para suporte interno de TI, com o propósito de evidenciar os principais trade-offs algorítmicos necessários ao dimensionamento eficiente de bases de conhecimento corporativas.

### 2.2 Assuntos da pesquisa

Escrevam de 4 a 5 assuntos que serão abordados na pesquisa.

- Conceituar árvore de decisão
- Conceituar inteligência artificial
- Quais são as estratégias de marketing para segmentação de clientes?
- Analisar a relação existente entre árvore de decisão e inteligência artificial
- Apresentar quais são os resultados das estratégias de marketing para segmentação de clientes sem e com IA

**Assuntos do grupo:**
1. Resposta: Conceituar arquiteturas RAG e a importância da busca vetorial por similaridade no contexto de suporte interno de TI
2. Resposta: Descrever e fundamentar o funcionamento algorítmico e as estruturas de dados de k-NN exato (Flat), HNSW (grafos) e IVF (arquivos invertidos)
3. Resposta: Analisar a complexidade assintótica temporal (indexação e consulta) e espacial (consumo de memória RAM) dos três algoritmos de busca
4. Resposta: Avaliar o impacto das abordagens aproximadas (ANN) sobre a qualidade da recuperação por meio da métrica de Recall@k
5. Resposta: Comparar os trade-offs de latência, consumo de recursos e escalabilidade entre busca exata e aproximada em cenários corporativos

### 2.3 Estrutura básica do artigo

Definam a estrutura do artigo, incluindo introdução e considerações finais.

**Estrutura do grupo:**
- Introdução
- Resposta: Fundamentação teórica de sistemas RAG e mecanismos de busca vetorial em suporte interno de TI
- Resposta: Algoritmos de busca vetorial: características estruturais de k-NN exato, HNSW e IVF
- Resposta: Análise comparativa da complexidade assintótica temporal, espacial e pegada de memória
- Resposta: Avaliação de desempenho e qualidade de recuperação: trade-offs entre latência, escalabilidade e Recall@k
- Considerações finais

### 2.4 Objetivos específicos classificados

Classifiquem os objetivos específicos em **Conceituais** e **Técnicos**.

**Objetivos específicos do grupo:**

- **Objetivos Conceituais**
  - Resposta: Conceituar a arquitetura RAG (Retrieval-Augmented Generation) e o papel dos embeddings e da recuperação semântica em bases de suporte de TI.
  - Resposta: Conceituar os princípios de indexação e busca vetorial, diferenciando os métodos exatos (k-NN Flat) dos métodos aproximados por grafos (HNSW) e por agrupamento/particionamento (IVF).

- **Objetivos Técnicos**
  - Resposta: Determinar e comparar formalmente a complexidade assintótica de tempo (construção e consulta) e de espaço (memória RAM) dos algoritmos k-NN exato, HNSW e IVF.
  - Resposta: Analisar a relação entre latência de consulta e a perda de precisão (métrica de Recall@k) introduzida pelos algoritmos aproximados frente à busca exata.
  - Resposta: Avaliar os trade-offs operacionais e a escalabilidade dos três algoritmos para orientar o dimensionamento eficiente de bases vetoriais em ambientes corporativos de Helpdesk.

---

## CHECKLIST FINAL DO GRUPO

- [x] O tema específico está delimitado (área, tempo, espaço ou aplicação)
- [x] A problemática está formulada como pergunta
- [x] O objetivo geral está no infinitivo, claro e mensurável
- [x] Foram listados de 4 a 5 assuntos do artigo
- [x] A estrutura do artigo foi definida (introdução, desenvolvimento, considerações finais)
- [x] Os objetivos específicos foram classificados em Conceituais e Técnicos


