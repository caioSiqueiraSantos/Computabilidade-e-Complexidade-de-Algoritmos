# Etapa 4 — Planejamento da busca bibliográfica

## Identificação do grupo

| Campo | Informação |
|---|---|
| Curso / Disciplina | Computabilidade e Complexidade de Algoritmos / Ciência da Computação |
| Projeto de Pesquisa | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientadora | Andrea Ono Sakai |
| Integrantes | Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires e Matheus Henrique da Trindade |
| Tema | Análise comparativa de complexidade, escalabilidade, uso de memória e qualidade dos algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em sistemas RAG para suporte interno de TI. |
| Responsáveis pela elaboração | Leonel, Leonardo e Caio, com contribuição do grupo |

## Conceitos e termos

| Conceito principal | Sinônimos em português | Termos em inglês |
|---|---|---|
| Busca vetorial e similaridade | Busca por vizinhos mais próximos, recuperação semântica, busca aproximada | Vector search, nearest neighbor search (NNS), approximate nearest neighbor search (ANNS), similarity search |
| Algoritmos de indexação | k-NN exato, busca por força bruta (Flat), grafos navegáveis HNSW, índice de arquivo invertido IVF, quantização de produto | Exact k-NN, brute-force search, Hierarchical Navigable Small World (HNSW), Inverted File Index (IVF), Product Quantization (PQ), IVFADC |
| RAG e chatbots | Geração aumentada por recuperação, assistentes virtuais, suporte de TI, recuperação de informação | Retrieval-Augmented Generation (RAG), conversational agents, IT support chatbots, dense passage retrieval |
| Complexidade e desempenho | Complexidade temporal e espacial, tempo de indexação, latência, consumo de memória, revocação | Time complexity, space complexity, indexing/build time, query latency, memory footprint, Recall@k, MRR@k, TTFT |

## Strings de busca

As strings abaixo preservam a estratégia registrada no levantamento preliminar. A aplicação de parênteses pode variar conforme os recursos de cada base; recomenda-se testar e registrar a expressão efetivamente executada.

| Nº | String completa | Base em que será usada | Responsáveis indicados no levantamento |
|---|---|---|---|
| 1 | `("RAG" OR "Retrieval-Augmented Generation") AND ("busca vetorial" OR "busca semântica" OR "vector search") AND ("latência" OR "latency" OR "recall")` | SBC Open Lib | Leonel e Leonardo |
| 2 | `("HNSW" OR "Hierarchical Navigable Small World") AND ("graph" OR "clustering" OR "Canopy") AND ("complexidade" OR "complexity" OR "recall")` | SBC Open Lib e IEEE Xplore | Caio e Matheus |
| 3 | `("similarity search" OR "k-NN" OR "IVF") AND ("GPU" OR "acceleration" OR "FAISS" OR "memory")` | ResearchGate; complementar com arXiv quando pertinente | Fillipy e Elton |

## Bases de dados

| Base | Justificativa da escolha |
|---|---|
| SBC Open Lib | Repositório da Sociedade Brasileira de Computação, adequado para localizar trabalhos nacionais publicados em anais de eventos como SBSI, ENIAC e ERIGO, incluindo estudos de RAG e busca vetorial. |
| arXiv | Repositório de preprints de Ciência da Computação, útil para localizar trabalhos técnicos e estudos associados a ferramentas de busca vetorial, como FAISS. |
| IEEE Xplore | Base de publicações científicas e técnicas da IEEE, relevante para pesquisas sobre algoritmos, estruturas de dados e avaliação de desempenho. |
| ResearchGate | Plataforma usada no levantamento para localizar versões e páginas de artigos científicos; deve ser registrada como local de acesso, distinguindo-a da base bibliográfica original sempre que possível. |

## Critérios de inclusão

- Trabalhos publicados entre 2015 e 2026.
- Textos em português ou inglês.
- Artigos revisados por pares ou relatórios técnicos seminais de relevância tecnológica, quando ligados a projetos ou ferramentas consolidadas.
- Texto completo disponível para consulta.
- Estudos com análise teórica, experimental ou sistemática de algoritmos de busca vetorial, incluindo k-NN, HNSW, IVF e PQ, ou de métricas de desempenho relevantes.
- Relação direta com pelo menos um dos critérios da pesquisa: complexidade temporal, complexidade espacial/uso de memória, tempo de construção do índice, latência, escalabilidade, Recall@k, MRR ou TTFT.
- Preferência por estudos que permitam discutir o uso de busca vetorial em sistemas RAG e o contexto de suporte interno de TI, sem exigir que todos os trabalhos estudem especificamente um chatbot de Helpdesk.

## Critérios de exclusão

- Duplicatas recuperadas em mais de uma base.
- Trabalhos sem avaliação teórica ou quantitativa explícita de complexidade, latência, memória ou qualidade de recuperação.
- Trabalhos focados exclusivamente em modelos de linguagem proprietários, sem detalhamento do mecanismo de recuperação vetorial.
- Estudos exclusivamente sobre recuperação lexical/BM25, sem relação com embeddings ou busca vetorial densa.
- Resumos estendidos, pôsteres sem validação experimental ou textos sem acesso integral.
- Trabalhos fora do escopo dos algoritmos e métricas delimitados pelo grupo.

## Produto da etapa

Plano de busca bibliográfica com conceitos, termos em português e inglês, strings booleanas, bases de consulta e critérios definidos previamente à triagem.

## Checklist

- [x] Há termos em português e inglês.
- [x] As strings combinam `AND` e `OR` com agrupamento por parênteses para explicitar a lógica.
- [x] As bases são pertinentes ao tema.
- [x] Os critérios de inclusão e exclusão foram definidos antes da triagem.

## Observação metodológica

O levantamento preliminar registra buscas realizadas em 10/09/2026 e informa 14 resultados brutos. Este documento organiza o planejamento com base nesses registros; não representa uma nova execução das buscas.
