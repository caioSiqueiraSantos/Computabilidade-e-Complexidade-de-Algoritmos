## 1. Identificação do Grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | Computabilidade e Complexidade de Algoritmos / Ciência da Computação |
| Projeto de Pesquisa / IC | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientador(a) | Andrea Ono Sakai |
| Data de entrega desta etapa | 08/09/2026 |
| Integrantes do grupo | Caio, Elton, Fillipy, Leonardo, Leonel, Matheus |

---

## 2. Tema Escolhido

### 2.1 Área geral de interesse
*Qual grande área do conhecimento/disciplina motivou a escolha (ex.: complexidade dos algoritmos, classes de problemas P, NP, Algoritmos Gulosos, Programação Dinâmica, Divisão e conquista)?*

Complexidade e escalabilidade de algoritmos de busca vetorial e indexação aplicados a Inteligência Artificial e RAG (Retrieval-Augmented Generation).

### 2.2 Tema delimitado (versão final)
*Escreva o tema já delimitado, de forma específica — não o tema amplo. Lembre-se: o tema deve ser enunciado em 1 a 2 frases, como um assunto (ainda não é uma pergunta de pesquisa, isso vem na etapa "c").*

> **Tema:** Análise comparativa de complexidade, escalabilidade, uso de memória e qualidade dos algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em sistemas RAG para suporte interno de TI.

### 2.3 Do amplo ao específico
*Mostre o raciocínio de delimitação — como vocês chegaram do tema amplo al tema específico.*

| Tema amplo (ponto de partida) | Tema delimitado (ponto de chegada) |
|---|---|
| IA Generativa, RAG e Suporte de TI | Como a literatura compara a complexidade computacional, uso de memória, escalabilidade e qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte de TI? |

---

## 3. Justificativa da Escolha

### 3.1 Relevância
*Por que esse tema é importante ou atual? Para quem ele importa (academia, mercado, sociedade)?*

Em arquiteturas de busca semântica e RAG, a eficiência da recuperação da informação depende fundamentalmente da estrutura de dados e dos algoritmos de indexação vetorial. Compreender as trocas computacionais (*trade-offs*) entre precisão absoluta, uso de memória RAM e tempo de resposta (latência) nos algoritmos de busca vetorial é essencial para a Ciência da Computação. O estudo beneficia a academia ao comparar métodos exatos e aproximados em cenários práticos de Helpdesk, bem como o mercado corporativo, permitindo dimensionar sistemas de suporte eficientes e escaláveis.

### 3.2 Viabilidade
*O grupo avaliou se tem tempo, recursos, acesso a dados/fontes e domínio mínimo do assunto para desenvolver esse tema até o fim do projeto?*

| Critério | Avaliação (Sim/Parcial/Não) | Observação |
|---|---|---|
| Tempo disponível é suficiente | Sim | Estudo teórico e analítico baseado em revisão de literatura e benchmarks existentes. |
| Há acesso a fontes/dados necessários | Sim | Ampla literatura científica e documentação técnica sobre algoritmos k-NN, HNSW e IVF. |
| O grupo já tem domínio mínimo do tema | Parcial | Domínio de estrutura de dados e grafos, aprofundando a análise assintótica para espaços vetoriais. |
| Recursos técnicos necessários estão disponíveis | Sim | Acesso a bibliotecas de código aberto (ex: FAISS) e artigos acadêmicos para análise comparativa. |

### 3.3 Originalidade / Não-redundância
*O grupo verificou rapidamente (via um levantamento preliminar) se o tema já é excessivamente explorado ou se existe um ângulo próprio a ser explorado?*

Em vez de avaliar serviços comerciais proprietários, a pesquisa concentra-se puramente na avaliação algorítmica. O trabalho isola no máximo três abordagens distintas de busca vetorial (Busca Exata k-NN, Busca baseada em Grafos HNSW e Busca por Particionamento IVF) sob o prisma de métricas formais (Recall@k, latência e pegada de memória), trazendo um ângulo voltado à análise de complexidade em cenários reais de atendimento técnico.

---

## 4. Validação com o Orientador

| Campo | Informação |
|---|---|
| Data da conversa/validação | 25/08/2026 |
| Tema aprovado pelo orientador? | `Sim com ajustes` |
| Observações ou ajustes solicitados pelo orientador | Retirar produtos comerciais do centro do trabalho; limitar o escopo a no máximo 3 algoritmos de busca vetorial (k-NN exato, HNSW e IVF) e definir critérios claros de comparação (complexidade, memória, latência e Recall@k). |

---

## 5. Contribuição Individual dos Integrantes

> **Importante:** cada integrante deve descrever, com suas próprias palavras, o que efetivamente fez nesta etapa. Contribuições genéricas como "ajudei em tudo" não serão aceitas. Use verbos de ação e seja específico (ex.: "pesquisei 5 temas candidatos e apresentei prós/contras ao grupo").

### Integrante 1 — Caio
- **O que fez nesta etapa:** Pesquisou a fundamentação teórica sobre o algoritmo de busca exata k-NN (força bruta) e redigiu a seção de relevância acadêmica e prática da busca vetorial (item 3.1).
- **Tempo dedicado (aprox.):** 3h
- **Evidência da contribuição:** Link do documento compartilhado no Google Docs contendo o rascunho dos conceitos de k-NN e referências teóricas.

### Integrante 2 — Elton
- **O que fez nesta etapa:** Formulou a reestruturação do funil metodológico (item 2.3) e redigiu a nova pergunta de pesquisa focada em complexidade, memória e qualidade dos algoritmos.
- **Tempo dedicado (aprox.):** 3h
- **Evidência da contribuição:** Registro das mensagens e propostas de texto no grupo de comunicação da equipe.

### Integrante 3 — Fillipy
- **O que fez nesta etapa:** Mapeou a viabilidade técnica e as propriedades de complexidade temporal e espacial do algoritmo HNSW (estruturas em grafo) no item 3.2.
- **Tempo dedicado (aprox.):** 2h
- **Evidência da contribuição:** Tabela comparativa dos trade-offs do HNSW inserida na pasta do Google Drive do grupo.

### Integrante 4 — Leonardo
- **O que fez nesta etapa:** Realizou o levantamento preliminar sobre o algoritmo IVF (Inverted File Index / particionamento em clusters) para a verificação de originalidade (item 3.3).
- **Tempo dedicado (aprox.):** 3h
- **Evidência da contribuição:** Histórico de buscas bibliográficas e lista de artigos sobre IVF organizados no documento de rascunho.

### Integrante 5 — Leonel
- **O que fez nesta etapa:** Reestruturou a área geral de interesse (item 2.1) para focar em Ciência da Computação pura e ajustou o tema conforme os critérios solicitados no feedback da professora.
- **Tempo dedicado (aprox.):** 2h
- **Evidência da contribuição:** Atas das discussões e mapa conceitual atualizado na plataforma de trabalho do grupo.

### Integrante 6 — Matheus
- **O que fez nesta etapa:** Consolidou a nova versão do documento em formato Markdown, adequou o checklist final e reorganizou o quadro-resumo de participação dos integrantes.
- **Tempo dedicado (aprox.):** 2h
- **Evidência da contribuição:** Histórico de edições e commits no repositório de entrega da equipe.

### 5.1 Quadro-resumo de participação

| Integrante | Contribuição principal | % estimado de participação nesta etapa |
|---|---|---|
| Caio | Pesquisa sobre k-NN exato e redação da relevância | 17% |
| Elton | Formulação da pergunta de pesquisa e funil metodológico | 17% |
| Fillipy | Análise de viabilidade e complexidade do HNSW | 17% |
| Leonardo | Levantamento de literatura e análise do algoritmo IVF | 17% |
| Leonel | Adequação do tema ao feedback e delimitação da área | 16% |
| Matheus | Consolidação em Markdown, revisão geral e checklist | 16% |

---

## 6. Checklist Final da Etapa

- [x] Tema delimitado e redigido em 1-2 frases
- [x] Justificativa de relevância escrita
- [x] Viabilidade avaliada pelo grupo
- [x] Verificação preliminar de originalidade realizada
- [x] Tema validado com o orientador (aprovado com os ajustes solicitados)
- [x] Contribuição individual de cada integrante registrada
- [x] Quadro-resumo de participação preenchido (soma = 100%)

---
