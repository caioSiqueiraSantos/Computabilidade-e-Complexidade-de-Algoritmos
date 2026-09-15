# Etapa (b) — Levantamento Bibliográfico

> **Como preencher:** este documento deve ser preenchido **em conjunto pelo grupo**, mas com registro individualizado da contribuição de cada integrante em cada passo. Substitua os campos entre `[ ]` pelas informações do seu grupo. Não apague as instruções em itálico — elas ajudam na avaliação do orientador.

---

## 1. Identificação do Grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | Computabilidade e Complexidade de Algoritmos / Ciência da Computação |
| Projeto de Pesquisa / IC | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientador(a) | Andrea Ono Sakai |
| Data de entrega desta etapa | 12/09/2026 |
| Integrantes do grupo | Caio, Elton, Fillipy, Leonardo, Leonel, Matheus |
| Tema (da etapa "a") | Análise comparativa de complexidade, escalabilidade, uso de memória e qualidade dos algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em sistemas RAG para suporte interno de TI. |

---

## FASE 1 — Planejamento da Busca

### Passo 1 — Pergunta de pesquisa e palavras-chave

**1.1 Problema/pergunta de pesquisa (versão de trabalho)**
*Ainda não precisa ser a versão final (isso vem na etapa "c"), mas deve orientar a busca desta fase.*

> Como a literatura compara a complexidade computacional, uso de memória, escalabilidade e qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte de TI?

**1.2 Conceitos-chave e sinônimos**
*Liste os conceitos centrais da pergunta e seus sinônimos, em português e inglês.*

| Conceito-chave | Sinônimos / termos relacionados (PT) | Sinônimos / termos relacionados (EN) |
|---|---|---|
| Busca Vetorial / Similaridade | Busca por vizinhos mais próximos, recuperação semântica, busca aproximada | Vector search, Nearest Neighbor Search (NNS), Approximate Nearest Neighbor Search (ANNS), similarity search |
| Algoritmos de Indexação | k-NN exato, força bruta, grafos navegáveis (HNSW), arquivo invertido (IVF), quantização de produto (PQ) | Exact k-NN, brute-force search, Hierarchical Navigable Small World (HNSW), Inverted File Index (IVF), Product Quantization (PQ), IVFADC |
| RAG / Chatbots | Geração aumentada por recuperação, assistentes virtuais, suporte de TI, recuperação de informação |Retrieval-Augmented Generation (RAG), conversational agents, IT support chatbots, dense passage retrieval |
| Complexidade e Desempenho | Complexidade assintótica temporal e espacial, tempo de indexação, latência, pegada de memória, revocação | Time complexity, space complexity, indexing time, build time, query latency, memory footprint, Recall@k, MRR@k, TTFT |


*Responsável por este passo: `Leonel, Leonardo e Caio`*

---

### Passo 2 — Strings de busca

*Combine os termos do passo 1 com operadores booleanos (`AND`, `OR`, `NOT`). Use aspas para termos compostos e truncamento (`*`) quando a base permitir.*

| Nº | String de busca | Base(s) em que será usada | Elaborada por |
|---|---|---|---|
| 1 | "RAG" OR "Retrieval-Augmented Generation" AND "busca vetorial" OR "busca semântica" OR "vector search" AND "latência" OR "latency" OR "recall" | SBC Open Lib | Leonel / Leonardo |
| 2 | "HNSW" OR "hierarchical navigable small world" AND "graph" OR "clustering" OR "Canopy" AND "complexidade" OR "complexity" OR "recall" | SBC Open Lib, IEEE Xplore | Caio / Matheus |
| 3 | "similarity search" OR "k-NN" OR "IVF" AND "GPU" OR "acceleration" OR "FAISS" OR "memory" | ResearchGate | Fillipy / Elton |

---

### Passo 3 — Bases de dados escolhidas

*Selecione de 2 a 4 bases relevantes ao tema. Registre a justificativa — isso vai para a seção de metodologia do artigo/relatório de IC.*

| Base de dados | Por que foi escolhida | Responsável pela busca nesta base |
|---|---|---|
| SBC Open Lib | Repositório oficial da Sociedade Brasileira de Computação, essencial para recuperar artigos nacionais recentes em anais de eventos consolidados (SBSI, ENIAC, ERIGO) sobre RAG e busca vetorial. | Leonardo |
| arXiv | Principal repositório de pré-prints de Ciência da Computação, onde são publicados os trabalhos seminais de código aberto em primeira mão (ex.: FAISS do Facebook AI Research). | Leonel e Caio |
| ResearchGate / IEEE Xplore | Plataforma acadêmica para acesso e compartilhamento das versões integrais de artigos avaliados por pares em periódicos internacionais de alto impacto (ex.: IEEE TPAMI para o HNSW). | Fillipy |

---

### Passo 4 — Critérios de inclusão e exclusão

**Critérios de inclusão:**
- Trabalhos publicados entre 2015 e 2026;
- Artigos revisados por pares ou relatórios técnicos seminais de grande impacto tecnológico (ex.: repositórios consolidados como arXiv vinculados a projetos de código aberto como FAISS/NMSLIB);
- Idioma em inglês ou português;
- Disponibilidade do texto completo na íntegra;
- Artigos que apresentem análise teórica, experimental ou sistemática de algoritmos de busca vetorial (k-NN, HNSW, IVF, PQ) ou métricas de desempenho em arquiteturas RAG (complexidade assintótica, latência, tempo de construção, uso de memória, Recall@k, MRR ou TTFT).

**Critérios de exclusão:**
- Artigos sem avaliação quantitativa ou teórica explícita de complexidade, latência ou memória;
- Trabalhos focados exclusivamente em modelos de linguagem (LLMs) proprietários sem detalhamento do mecanismo de recuperação vetorial;
- Artigos puramente teóricos de recuperação de informação clássica (puramente lexical/BM25) sem interface com embeddings ou busca vetorial densa;
- Resumos estendidos, pôsteres sem validação experimental ou artigos sem acesso integral;
- Duplicatas entre bases bibliográficas.

*Definidos em conjunto por: Caio, Elton, Fillipy, Leonardo, Leonel, Matheus*

---

## FASE 2 — Execução da Busca e Triagem

### Passo 5 — Execução das buscas e registro dos resultados

*Anote quantos resultados cada string trouxe em cada base (útil para o fluxograma tipo PRISMA, se o projeto exigir). Exporte as referências (BibTeX, RIS, CSV) para um gerenciador de referências.*

| Base | String usada (nº) | Data da busca | Nº de resultados | Executada por |
|---|---|---|---|---|
| SBC Open Lib (SOL) | 1 e 2 | 10/09/2026 | 8 | Leonel e Matheus |
| arXiv / ResearchGate | 2 e 3 | 10/09/2026 | 6 | Leonardo e Caio |

**Total de resultados brutos (soma de todas as buscas):** 14

**Gerenciador de referências utilizado:** Zotero
**Formato de exportação:** BibTeX

---

### Passo 6 — Triagem por título e resumo (1ª filtragem)

*Leia apenas título e resumo de cada resultado. Classifique: incluir / excluir / dúvida. Remova duplicatas entre bases.*

| Item de controle | Quantidade |
|---|---|
| Total de resultados antes da triagem | 14 |
| Duplicatas removidas | 2 |
| Classificados como "Incluir" | 6 |
| Classificados como "Excluir" | 5 |
| Classificados como "Dúvida" | 1 |

*A triagem detalhada, artigo por artigo, deve ser registrada na planilha de controle do projeto (aba "Triagem de Artigos"). Aqui, registre apenas o resumo quantitativo.*

**Como as dúvidas foram resolvidas?** *(ex.: discussão em grupo, consulta ao orientador)*
Após a remoção das 2 duplicatas, o grupo avaliou os 12 artigos únicos por título e resumo. O único artigo classificado como "Dúvida" foi discutido pela equipe para verificar se apresentava métricas de latência e complexidade de busca vetorial; com a confirmação desses dados na metodologia, ele foi promovido para inclusão, totalizando 7 artigos encaminhados para leitura completa.

*Responsável(is) por esta triagem: Leonel, Caio, Matheus, Fillipy e Leonardo*

---

### Passo 7 — Triagem por leitura completa (2ª filtragem)

*Para os artigos que passaram na primeira filtragem, leia introdução e conclusão. Aplique os critérios de inclusão/exclusão (passo 4) de forma mais rigorosa.*

| Item de controle | Quantidade |
|---|---|
| Total de artigos que entraram nesta filtragem | 7 |
| Aprovados (conjunto definitivo para fichamento) | 5 |
| Excluídos nesta etapa | 2 |

**Principais motivos de exclusão nesta filtragem:**
- Artigo com foco apenas na engenharia de prompt do chatbot, sem análise da estrutura de indexação vetorial (1 artigo);
- Artigo com testes preliminares em datasets proprietários sem detalhamento de memória ou complexidade assintótica (1 artigo).

*Responsável(is) por esta triagem: Elton, Leonel, Caio, Fillipy e Leonardo*

---

## 3. Lista Final de Artigos Selecionados (Conjunto Definitivo)

*Liste aqui os artigos que passaram por todas as filtragens e seguirão para o fichamento (etapa "j"). Referência completa no formato ABNT/APA definido pelo projeto.*

1. MALKOV, Yu. A.; YASHUNIN, D. A. Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs. IEEE Transactions on Pattern Analysis and Machine Intelligence, v. 42, n. 4, p. 824–836, 2020. Disponível em: ResearchGate: https://www.researchgate.net/publication/301837503_Efficient_and_Robust_Approximate_Nearest_Neighbor_Search_Using_Hierarchical_Navigable_Small_World_Graphs
2. JOHNSON, Jeff; DOUZE, Matthijs; JÉGOU, Hervé. Billion-scale similarity search with GPUs. IEEE Transactions on Big Data, v. 7, n. 3, p. 535–547, 2021. Disponível em: arXiv: https://arxiv.org/pdf/1702.08734.
3. PINHEIRO, Rafael F.; LIMA, Karla Roberta P. S. Canopy-Guided Construction of ANN Search Graphs under Cosine Similarity. In: Anais do XXI Simpósio Brasileiro de Sistemas de Informação (SBSI). Porto Alegre: SBC, 2025. p. 1–12. Disponível em: SBC Open Lib - SBSI: https://sol.sbc.org.br/index.php/sbsi/article/view/41327
4. BRAKES, Matheus F. C. et al. Uma Arquitetura de RAG com Busca Semântica e Filtros Estruturados para Perguntas e Respostas no Domínio Jurídico. In: Anais da Escola Regional de Informática de Goiás (ERIGO / SBC). Porto Alegre: SBC, 2024. p. 1–14. Disponível em: SBC Open Lib - ERIGO: https://sol.sbc.org.br/index.php/erigo/article/view/39531
5. SILVA, João Gabriel J. da; OLIVEIRA, Sávio S. T. de; GALVÃO FILHO, Arlindo R. Accelerating RAG Systems: A Performance-Oriented Systematic Mapping. In: Anais do Encontro Nacional de Inteligência Artificial e Computacional (ENIAC / SBC). Porto Alegre: SBC, 2024. p. 1–13. Disponível em: SBC Open Lib - ENIAC: https://sol.sbc.org.br/index.php/eniac/article/view/38722

*(Adicione quantas linhas forem necessárias.)*

---

## 4. Contribuição Individual dos Integrantes

> **Importante:** cada integrante deve descrever, com suas próprias palavras, o que efetivamente fez em cada passo desta etapa. Contribuições genéricas como "ajudei em tudo" não serão aceitas. Use verbos de ação e seja específico (ex.: "executei a busca no IEEE Xplore com a string 2 e obtive 84 resultados; fiz a triagem por título/resumo de 40 desses").

### Integrante 1 — `Caio Siqueira Santos`
- **Passo(s) em que atuou:** 1, 2, 3, 5, 6 e 7
- **O que fez em cada passo:** Estruturou os conceitos-chave de busca exata e aproximada no Passo 1; elaborou a String de Busca 2 voltada a HNSW e grafos no Passo 2; participou da justificativa da base arXiv no Passo 3; executou a rotina de buscas no portal arXiv/ResearchGate no Passo 5; participou da triagem por título/resumo no Passo 6 e realizou a leitura completa do artigo do FAISS (Johnson et al.) com foco em GPU e k-NN exato no Passo 7.
- **Tempo dedicado (aprox.):** 7h
- **Evidência da contribuição** Documento do Word contendo o fichamento técnico dos operadores de GPU do FAISS e tabela de triagem registrada no caderno do OneNote compartilhado pelo grupo.

### Integrante 2 — `Elton Dos Santos Rodrigues`
- **Passo(s) em que atuou:** 2, 4 e 7
- **O que fez em cada passo:** Formulou a String de Busca 3 com termos voltados para quantização de produto e similaridade vetorial no Passo 2; redigiu os critérios de inclusão e exclusão com base em métricas assintóticas no Passo 4; participou da leitura completa dos artigos aprovados no Passo 7, verificando o alinhamento com a disciplina de complexidade.
- **Tempo dedicado (aprox.):** 3h
- **Evidência da contribuição:** Documento do Word com a especificação formal dos critérios metodológicos e ata da discussão de exclusão registrada na página do OneNote da equipe.

### Integrante 3 — `Fillipy Mendes Vilela`
- **Passo(s) em que atuou:** 2, 3, 4, 6 e 7
- **O que fez em cada passo:** Desenvolveu a String de Busca 3 focada em índices invertidos e memória no Passo 2; justificou o uso do portal ResearchGate/IEEE Xplore no Passo 3; refinou os critérios de exclusão no Passo 4; realizou a leitura e triagem por título/resumo de 12 artigos no Passo 6; analisou a metodologia e complexidade assintótica do artigo HNSW (Malkov & Yashunin) no Passo 7.
- **Tempo dedicado (aprox.):** 6h
- **Evidência da contribuição:** Anotações no OneNote sobre as propriedades estruturais do grafo HNSW e documento do Word com a análise comparativa de complexidade assintótica.

### Integrante 4 — `Leonardo Masanao`
- **Passo(s) em que atuou:** 1, 2, 3, 5, 6 e 7
- **O que fez em cada passo:** Definiu sinônimos técnicos no Passo 1; formulou a String 1 em conjunto no Passo 2; justificou a escolha da SBC Open Lib no Passo 3; localizou e disponibilizou os dois artigos internacionais seminais (HNSW e FAISS) via ResearchGate e arXiv, registrando 6 resultados no Passo 5; atuou na 1ª filtragem no Passo 6 e na leitura completa do artigo de Canopy-HNSW (Pinheiro & Lima) no Passo 7.
- **Tempo dedicado (aprox.):** 8h
- **Evidência da contribuição:** Página no OneNote com o histórico de links, resumos executivos dos artigos seminais e documento do Word detalhando a análise do Canopy Clustering.

### Integrante 5 — `Leonel Santos Caires`
- **Passo(s) em que atuou:** 1, 2, 3, 5, 6 e 7
- **O que fez em cada passo:** Formulou a versão preliminar da pergunta de pesquisa e tabela conceitual no Passo 1; elaborou a String 1 focada em RAG e busca semântica no Passo 2; redigiu a justificativa do repositório arXiv no Passo 3; executou as buscas nos anais da SBC Open Lib (obtendo 8 resultados) no Passo 5; avaliou resumos na 1ª filtragem no Passo 6 e realizou a leitura analítica dos artigos de RAG da SBC (Brakes et al. e Silva et al.) no Passo 7.
- **Tempo dedicado (aprox.):** 7h
- **Evidência da contribuição:** Documento do Word com a análise detalhada das métricas de latência e Recall em RAG, acompanhado de registros das buscas arquivados no OneNote.

### Integrante 6 — `Matheus Henrique da Trindade`
- **Passo(s) em que atuou:** 2, 4, 5, 6
- **O que fez em cada passo:** Auxiliou na construção da String 2 no Passo 2; validou os critérios de inclusão e exclusão no Passo 4; operou a biblioteca central no Zotero, realizando a identificação e remoção das 2 duplicatas no Passo 5 e 6; padronizou as referências bibliográficas finais na norma ABNT NBR 6023 (Seção 3) e consolidou o documento final em Markdown.
- **Tempo dedicado (aprox.):** 3h
- **Evidência da contribuição:** Documento do Word com as referências formatadas em ABNT e notas no OneNote documentando a conferência e remoção de duplicatas.

*(Copie o bloco acima para cada integrante adicional do grupo.)*

### 4.1 Quadro-resumo de participação por passo

| Passo | Responsável(is) | % estimado de participação de cada um |
|---|---|---|
| 1. Pergunta e palavras-chave | Leonel, Leonardo e Caio | Leonel 33%, Leonardo 34%, Caio 33% |
| 2. Strings de busca | Leonel, Leonardo, Caio, Matheus, Fillipy, Elton | Leonel 20%, Leonardo 24%, Caio 24%, Matheus 6%, Fillipy 20%, Elton 6% |
| 3. Bases de dados | Leonardo, Leonel, Caio, Fillipy | Leonardo 30%, Leonel 25%, Caio 25%, Fillipy 20% |
| 4. Critérios de inclusão/exclusão | Caio, Elton, Fillipy, Leonardo, Leonel, Matheus | Caio 22%, Elton 7%, Fillipy 22%, Leonardo 22%, Leonel 20%, Matheus 7% |
| 5. Execução das buscas | Leonel, Matheus, Leonardo, Caio | Leonel 30%, Matheus 25%, Leonardo 25%, Caio 20% |
| 6. Triagem título/resumo | Leonel, Caio, Matheus, Fillipy, Leonardo | Leonel 20%, Caio 20%, Matheus 20%, Fillipy 20%, Leonardo 20% |
| 7. Triagem texto completo | Elton, Leonel, Caio, Fillipy, Leonardo | Elton 20%, Leonel 20%, Caio 20%, Fillipy 20%, Leonardo 20% |

### 4.2 Quadro-resumo geral de participação na etapa

| Integrante | % estimado de participação total nesta etapa |
|---|---|
| Leonardo | 25% |
| Leonel | 24% |
| Caio | 23% |
| Fillipy | 15% |
| Matheus | 8% |
| Elton | 5% |

*A soma das porcentagens deve ser igual a 100%. Divergências de percepção sobre a participação devem ser discutidas em grupo antes do envio — o orientador pode solicitar esclarecimentos individuais em caso de disparidade relevante.*

---

## 5. Checklist Final da Etapa

**Fase 1 — Planejamento**
- [X] Pergunta de pesquisa de trabalho definida
- [X] Conceitos-chave e sinônimos (PT/EN) listados
- [X] Strings de busca elaboradas com operadores booleanos
- [X] Bases de dados escolhidas e justificadas
- [X] Critérios de inclusão e exclusão definidos

**Fase 2 — Execução e triagem**
- [X] Buscas executadas e resultados registrados por base/string
- [X] Referências exportadas para o gerenciador de referências
- [X] Triagem por título/resumo concluída (com duplicatas removidas)
- [X] Triagem por texto completo (introdução/conclusão) concluída
- [X] Conjunto definitivo de artigos para fichamento compilado

**Documentação**
- [X] Contribuição individual de cada integrante registrada por passo
- [X] Quadro-resumo de participação preenchido (soma = 100%)

---


