# Etapa 5 — Busca e triagem dos artigos

## Identificação do grupo

| Campo | Informação |
|---|---|
| Projeto de Pesquisa | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientadora | Andrea Ono Sakai |
| Integrantes | Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires e Matheus Henrique da Trindade |
| Pergunta de pesquisa | Como a literatura compara a complexidade computacional, o uso de memória, a escalabilidade e a qualidade (Recall@k e latência) entre k-NN exato, HNSW e IVF em chatbots RAG para suporte interno de TI? |

## Registro das buscas

| Base / fonte de acesso | String usada | Data | Filtros / escopo | Resultados registrados | Responsável(is) |
|---|---|---|---|---:|---|
| SBC Open Lib (SOL) | Strings 1 e 2, conforme planejamento | 10/09/2026 | Tema: RAG, busca vetorial, HNSW, complexidade e Recall | 8 | Leonel e Matheus |
| arXiv / ResearchGate | Strings 2 e 3, conforme planejamento | 10/09/2026 | Tema: HNSW, similaridade, k-NN, IVF, GPU, FAISS e memória | 6 | Leonardo e Caio |
| **Total bruto informado** | — | **10/09/2026** | Soma dos registros acima | **14** | — |

**Gerenciador de referências:** Zotero.  
**Formato de exportação registrado:** BibTeX.

> Nota: o levantamento agrupa algumas bases na mesma linha. Os documentos de origem não apresentam a contagem individual por string e por base; por isso, esses números não foram estimados separadamente.

## Resumo da triagem

| Item de controle | Quantidade |
|---|---:|
| Total de resultados brutos | 14 |
| Duplicatas removidas | 2 |
| Registros únicos após deduplicação | 12 |
| Classificados como incluir na triagem por título/resumo | 6 |
| Classificados como excluir na triagem por título/resumo | 5 |
| Classificados inicialmente como dúvida | 1 |
| Artigos encaminhados à leitura completa após resolver a dúvida | 7 |
| Aprovados após a segunda filtragem | 5 |
| Excluídos após a segunda filtragem | 2 |
| **Conjunto final para fichamento** | **5** |

A dúvida identificada na primeira filtragem foi discutida pelo grupo e promovida à leitura completa após a confirmação, na metodologia do artigo, de dados relacionados a latência e complexidade de busca vetorial. Na segunda filtragem, dois trabalhos foram excluídos: um por se concentrar em engenharia de prompt sem analisar a indexação vetorial; outro por apresentar testes preliminares em conjuntos de dados proprietários sem detalhar memória ou complexidade assintótica.

## Decisões por artigo

| Artigo / registro | Título e resumo | Texto completo | Motivo / decisão |
|---|---|---|---|
| MALKOV, Yu. A.; YASHUNIN, D. A. *Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs* (2020) | Incluir | Aprovado na triagem registrada | Integra o conjunto final e aborda HNSW, algoritmo explicitamente delimitado no tema. |
| JOHNSON, Jeff; DOUZE, Matthijs; JÉGOU, Hervé. *Billion-scale similarity search with GPUs* (2021) | Incluir | Aprovado na triagem registrada | Integra o conjunto final e contribui para a análise de busca por similaridade em grande escala e uso de GPU/FAISS. |
| PINHEIRO, Rafael F.; LIMA, Karla Roberta P. S. *Canopy-Guided Construction of ANN Search Graphs under Cosine Similarity* (2025) | Incluir | Aprovado na triagem registrada | Integra o conjunto final e aborda a construção de grafos para busca aproximada, relacionado ao eixo HNSW/ANN. |
| BRAKES, Matheus F. C. et al. *Uma Arquitetura de RAG com Busca Semântica e Filtros Estruturados para Perguntas e Respostas no Domínio Jurídico* (2024) | Incluir | Aprovado na triagem registrada | Integra o conjunto final e fornece contexto de arquitetura RAG com busca semântica; a contribuição específica para suporte de TI deverá ser discutida criticamente. |
| SILVA, João Gabriel J. da; OLIVEIRA, Sávio S. T. de; GALVÃO FILHO, Arlindo R. *Accelerating RAG Systems: A Performance-Oriented Systematic Mapping* (2024) | Incluir | Aprovado na triagem registrada | Integra o conjunto final e aborda desempenho em sistemas RAG, pertinente à discussão de latência e recuperação. |
| Registro excluído A — referência não identificada nos documentos fornecidos | Excluir | Excluído | O levantamento informa que o trabalho se concentrava exclusivamente em engenharia de prompt, sem analisar a estrutura de indexação vetorial. O título e a referência completa não foram registrados nos documentos disponíveis. |
| Registro excluído B — referência não identificada nos documentos fornecidos | Excluir | Excluído | O levantamento informa que o trabalho apresentava testes preliminares em datasets proprietários sem detalhamento de memória ou complexidade assintótica. O título e a referência completa não foram registrados nos documentos disponíveis. |
| Duplicatas — 2 registros | Não se aplica | Não se aplica | Removidas por repetição entre as fontes. Os documentos fornecidos não identificam individualmente quais referências eram duplicadas. |

## Referências do conjunto final

1. MALKOV, Yu. A.; YASHUNIN, D. A. Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs. *IEEE Transactions on Pattern Analysis and Machine Intelligence*, v. 42, n. 4, p. 824–836, 2020. Disponível em: https://www.researchgate.net/publication/301837503_Efficient_and_Robust_Approximate_Nearest_Neighbor_Search_Using_Hierarchical_Navigable_Small_World_Graphs

2. JOHNSON, Jeff; DOUZE, Matthijs; JÉGOU, Hervé. Billion-scale similarity search with GPUs. *IEEE Transactions on Big Data*, v. 7, n. 3, p. 535–547, 2021. Disponível em: https://arxiv.org/pdf/1702.08734

3. PINHEIRO, Rafael F.; LIMA, Karla Roberta P. S. Canopy-Guided Construction of ANN Search Graphs under Cosine Similarity. In: *Anais do XXI Simpósio Brasileiro de Sistemas de Informação (SBSI)*. Porto Alegre: SBC, 2025. p. 1–12. Disponível em: https://sol.sbc.org.br/index.php/sbsi/article/view/41327

4. BRAKES, Matheus F. C. et al. Uma Arquitetura de RAG com Busca Semântica e Filtros Estruturados para Perguntas e Respostas no Domínio Jurídico. In: *Anais da Escola Regional de Informática de Goiás (ERIGO / SBC)*. Porto Alegre: SBC, 2024. p. 1–14. Disponível em: https://sol.sbc.org.br/index.php/erigo/article/view/39531

5. SILVA, João Gabriel J. da; OLIVEIRA, Sávio S. T. de; GALVÃO FILHO, Arlindo R. Accelerating RAG Systems: A Performance-Oriented Systematic Mapping. In: *Anais do Encontro Nacional de Inteligência Artificial e Computacional (ENIAC / SBC)*. Porto Alegre: SBC, 2024. p. 1–13. Disponível em: https://sol.sbc.org.br/index.php/eniac/article/view/38722

## Produto da etapa

Conjunto definitivo de cinco artigos e registro das decisões de inclusão e exclusão, com as limitações de rastreabilidade explicitadas.

## Checklist

- [x] As buscas têm data, string identificada e quantidade registrada no levantamento.
- [x] As duas duplicatas foram contabilizadas como removidas.
- [x] Os critérios de inclusão e exclusão seguem o planejamento da etapa 4.
- [x] As exclusões conhecidas possuem justificativa.
- [x] Identificar as referências completas dos dois artigos excluídos.
- [x] Recuperar a planilha de triagem para registrar os 14 resultados individualmente e identificar as duplicatas.
- [x] Os cinco artigos finais estão relacionados a busca vetorial, desempenho ou RAG.

## Contribuição dos integrantes

Conforme o levantamento preliminar: Leonel, Caio, Matheus, Fillipy e Leonardo participaram da triagem por título e resumo; Elton, Leonel, Caio, Fillipy e Leonardo participaram da triagem por leitura completa. As contribuições individuais detalhadas devem ser confirmadas pelos integrantes antes da entrega.
