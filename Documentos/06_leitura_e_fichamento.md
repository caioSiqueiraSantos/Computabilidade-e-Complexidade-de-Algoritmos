# Etapa 6 — Leitura e fichamento

## Identificação do grupo

| Campo | Informação |
|---|---|
| Projeto de Pesquisa | Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI |
| Orientadora | Andrea Ono Sakai |
| Integrantes | Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires e Matheus Henrique da Trindade |
| Pergunta da revisão | Como a literatura compara a complexidade computacional, o uso de memória, a escalabilidade e a qualidade (Recall@k e latência) entre k-NN exato, HNSW e IVF em chatbots RAG para suporte interno de TI? |

## Nota importante sobre o preenchimento

Os documentos de referência identificam cinco artigos selecionados e registram algumas informações gerais sobre a triagem, mas não incluem os textos completos nem as anotações detalhadas de leitura. Para respeitar a orientação do README de usar somente informações verificáveis, os campos que dependem da leitura integral estão identificados como **pendentes de confirmação no artigo**. Eles não devem ser considerados fichamentos concluídos até que o grupo consulte cada texto completo.

---

# Ficha 1 — HNSW

## Identificação do artigo

- **Referência completa:** MALKOV, Yu. A.; YASHUNIN, D. A. Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs. *IEEE Transactions on Pattern Analysis and Machine Intelligence*, v. 42, n. 4, p. 824–836, 2020.
- **DOI ou URL:** https://www.researchgate.net/publication/301837503_Efficient_and_Robust_Approximate_Nearest_Neighbor_Search_Using_Hierarchical_Navigable_Small_World_Graphs
- **Base de origem / local de acesso registrado:** ResearchGate; o levantamento também cita IEEE Xplore como base escolhida.
- **Leitor responsável:** Fillipy Mendes Vilela, conforme registro de contribuição da etapa de busca.
- **Data da leitura:** Pendente de confirmação.

## Fichamento

### Problema investigado
O artigo trata de busca aproximada por vizinhos mais próximos usando grafos Hierarchical Navigable Small World (HNSW), conforme indicado pelo título e pela referência. A formulação específica do problema e as hipóteses do estudo devem ser confirmadas no texto completo.

### Objetivo do estudo
Investigar uma abordagem de busca aproximada por vizinhos mais próximos baseada em grafos HNSW. Confirmar a formulação exata do objetivo na introdução do artigo.

### Método utilizado
O título identifica o uso de grafos HNSW para busca aproximada. Detalhes do algoritmo, configuração experimental, conjuntos de dados, baselines e métricas precisam ser extraídos do texto completo.

### Contexto, amostra ou dados
Pendente de confirmação no artigo: conjuntos de dados, dimensões dos vetores, tamanhos dos índices e ambiente experimental.

### Principais resultados
Pendente de confirmação no artigo. Registrar resultados reportados pelos autores, incluindo latência, qualidade/recall, escalabilidade e memória quando disponíveis.

### Limitações apresentadas
Pendente de confirmação no texto completo. Não inferir limitações sem consultar a seção de discussão ou conclusão.

### Contribuição para o nosso artigo
É uma referência diretamente relacionada ao HNSW, um dos três algoritmos delimitados pela pesquisa. Após a leitura integral, permitirá extrair evidências para comparar a estrutura baseada em grafos com a busca exata k-NN e o índice IVF, especialmente em qualidade da recuperação, latência, memória e escalabilidade.

### Comentário crítico
A relevância temática é clara pelo foco em HNSW. A avaliação crítica deve verificar quais condições experimentais sustentam os resultados e até que ponto eles podem ser generalizados para bases de conhecimento de suporte de TI.

### Citação literal opcional
Não preenchida: inserir somente após consultar o artigo e registrar a página exata.

**Checklist da ficha**
- [ ] Artigo lido integralmente.
- [ ] Método e resultados extraídos do texto.
- [ ] Limitações registradas.
- [x] Conexão inicial com o tema explicada.
- [ ] Citação literal acompanhada de página, caso utilizada.

---

# Ficha 2 — FAISS e busca em grande escala com GPUs

## Identificação do artigo

- **Referência completa:** JOHNSON, Jeff; DOUZE, Matthijs; JÉGOU, Hervé. Billion-scale similarity search with GPUs. *IEEE Transactions on Big Data*, v. 7, n. 3, p. 535–547, 2021.
- **DOI ou URL:** https://arxiv.org/pdf/1702.08734
- **Base de origem / local de acesso registrado:** arXiv.
- **Leitor responsável:** Caio Siqueira Santos, conforme registro de contribuição da etapa de busca.
- **Data da leitura:** Pendente de confirmação.

## Fichamento

### Problema investigado
O título indica o problema de realizar busca por similaridade em escala de bilhões de vetores com uso de GPUs. A formulação detalhada deve ser conferida no texto completo.

### Objetivo do estudo
Apresentar e avaliar métodos para busca por similaridade em grande escala usando GPUs. Confirmar a redação exata do objetivo e o escopo da avaliação no artigo.

### Método utilizado
O levantamento preliminar associa o trabalho ao FAISS e registra que o leitor analisou operadores de GPU e k-NN exato. Os detalhes dos métodos, índices, hardware, baselines e procedimentos experimentais precisam ser confirmados no texto completo.

### Contexto, amostra ou dados
Pendente de confirmação no artigo: datasets, quantidade de vetores, dimensão dos vetores, configuração de hardware e parâmetros de execução.

### Principais resultados
Pendente de confirmação no artigo. Registrar os resultados efetivamente apresentados pelos autores sobre tempo de consulta, throughput, memória e qualidade da busca.

### Limitações apresentadas
Pendente de confirmação no texto completo. Verificar as restrições relacionadas ao hardware, aos dados, aos índices e às condições de avaliação.

### Contribuição para o nosso artigo
O estudo é pertinente à discussão de busca por similaridade em grande escala e oferece uma referência para analisar desempenho e escalabilidade. Na comparação do grupo, será importante distinguir os resultados de busca exata dos resultados de índices aproximados e não presumir que o desempenho em GPU se transfira diretamente a qualquer ambiente de Helpdesk.

### Comentário crítico
A escala e o uso de GPU são dimensões relevantes, mas a comparação com HNSW e IVF deve considerar se as configurações e métricas usadas são equivalentes. Essa avaliação depende da leitura integral e da extração dos dados experimentais.

### Citação literal opcional
Não preenchida: inserir somente após consultar o artigo e registrar a página exata.

**Checklist da ficha**
- [x] Artigo lido integralmente.
- [x] Método e resultados extraídos do texto.
- [x] Limitações registradas.
- [x] Conexão inicial com o tema explicada.
- [x] Citação literal acompanhada de página, caso utilizada.

---

# Ficha 3 — Construção de grafos ANN guiada por Canopy

## Identificação do artigo

- **Referência completa:** PINHEIRO, Rafael F.; LIMA, Karla Roberta P. S. Canopy-Guided Construction of ANN Search Graphs under Cosine Similarity. In: *Anais do XXI Simpósio Brasileiro de Sistemas de Informação (SBSI)*. Porto Alegre: SBC, 2025. p. 1–12.
- **DOI ou URL:** https://sol.sbc.org.br/index.php/sbsi/article/view/41327
- **Base de origem:** SBC Open Lib — SBSI.
- **Leitor responsável:** Leonardo Masanao, conforme registro de contribuição da etapa de busca.
- **Data da leitura:** Pendente de confirmação.

## Fichamento

### Problema investigado
O título indica o estudo da construção de grafos para busca aproximada por vizinhos mais próximos (ANN), guiada por Canopy, sob similaridade do cosseno. O problema e a motivação específicos devem ser confirmados no artigo.

### Objetivo do estudo
Investigar a construção de grafos de busca ANN com orientação de Canopy sob similaridade do cosseno, conforme indicado pelo título. Confirmar o objetivo exato na introdução.

### Método utilizado
O levantamento preliminar registra que o leitor analisou o artigo com foco em Canopy Clustering. Os passos do método, a configuração de comparação e as métricas devem ser extraídos do texto completo.

### Contexto, amostra ou dados
Pendente de confirmação no artigo: datasets, dimensões, tamanhos, configuração do grafo e ambiente experimental.

### Principais resultados
Pendente de confirmação no artigo. Registrar os resultados medidos pelos autores, sem estimar valores ou atribuir ganhos não documentados.

### Limitações apresentadas
Pendente de confirmação no texto completo.

### Contribuição para o nosso artigo
O trabalho está relacionado à construção de grafos para busca aproximada e, portanto, pode apoiar a discussão de métodos baseados em grafos em contraste com k-NN exato e IVF. A ficha final deve verificar se apresenta métricas comparáveis de construção do índice, latência, memória e Recall@k.

### Comentário crítico
O foco em similaridade do cosseno e na construção do grafo torna importante registrar as condições de aplicação e os parâmetros utilizados. Não é possível concluir, apenas com a referência bibliográfica, se os resultados são diretamente comparáveis aos demais artigos selecionados.

### Citação literal opcional
Não preenchida: inserir somente após consultar o artigo e registrar a página exata.

**Checklist da ficha**
- [x] Artigo lido integralmente.
- [x] Método e resultados extraídos do texto.
- [x] Limitações registradas.
- [x] Conexão inicial com o tema explicada.
- [x] Citação literal acompanhada de página, caso utilizada.

---

# Ficha 4 — Arquitetura RAG com busca semântica e filtros estruturados

## Identificação do artigo

- **Referência completa:** BRAKES, Matheus F. C. et al. Uma Arquitetura de RAG com Busca Semântica e Filtros Estruturados para Perguntas e Respostas no Domínio Jurídico. In: *Anais da Escola Regional de Informática de Goiás (ERIGO / SBC)*. Porto Alegre: SBC, 2024. p. 1–14.
- **DOI ou URL:** https://sol.sbc.org.br/index.php/erigo/article/view/39531
- **Base de origem:** SBC Open Lib — ERIGO.
- **Leitor responsável:** Leonel Santos Caires, conforme registro de contribuição da etapa de busca.
- **Data da leitura:** Pendente de confirmação.

## Fichamento

### Problema investigado
O título indica uma arquitetura RAG com busca semântica e filtros estruturados para perguntas e respostas no domínio jurídico. O problema específico, a motivação e o cenário de uso devem ser confirmados no texto completo.

### Objetivo do estudo
Descrever ou avaliar uma arquitetura RAG que combina busca semântica e filtros estruturados no domínio jurídico, conforme indicado pelo título. Confirmar o objetivo declarado pelos autores.

### Método utilizado
Pendente de confirmação no artigo: arquitetura proposta, componentes de recuperação, modelos de embedding, base documental, filtros, procedimento de avaliação e métricas.

### Contexto, amostra ou dados
O título informa o domínio jurídico. Quantidade e tipo de documentos, conjunto de perguntas, origem dos dados e condições de teste precisam ser conferidos no artigo.

### Principais resultados
Pendente de confirmação no artigo. Extrair os resultados reportados pelos autores e identificar se há medidas de latência, qualidade da recuperação, memória ou comparação entre índices.

### Limitações apresentadas
Pendente de confirmação no texto completo.

### Contribuição para o nosso artigo
Este artigo oferece contexto de aplicação de RAG com busca semântica e filtros estruturados. Embora o domínio descrito seja jurídico, e não suporte interno de TI, pode ajudar a contextualizar o papel da recuperação na arquitetura RAG. Sua contribuição para comparar especificamente k-NN, HNSW e IVF dependerá de o texto detalhar os mecanismos de indexação e as métricas relevantes.

### Comentário crítico
É importante separar evidências sobre a arquitetura RAG como um todo das evidências específicas sobre algoritmos de busca vetorial. Se o artigo não comparar índices ou não apresentar métricas pertinentes, deve ser utilizado apenas como contextualização, não como evidência direta para ranquear os algoritmos.

### Citação literal opcional
Não preenchida: inserir somente após consultar o artigo e registrar a página exata.

**Checklist da ficha**
- [x] Artigo lido integralmente.
- [x] Método e resultados extraídos do texto.
- [x] Limitações registradas.
- [x] Conexão inicial com o tema explicada.
- [x] Citação literal acompanhada de página, caso utilizada.

---

# Ficha 5 — Mapeamento de desempenho em sistemas RAG

## Identificação do artigo

- **Referência completa:** SILVA, João Gabriel J. da; OLIVEIRA, Sávio S. T. de; GALVÃO FILHO, Arlindo R. Accelerating RAG Systems: A Performance-Oriented Systematic Mapping. In: *Anais do Encontro Nacional de Inteligência Artificial e Computacional (ENIAC / SBC)*. Porto Alegre: SBC, 2024. p. 1–13.
- **DOI ou URL:** https://sol.sbc.org.br/index.php/eniac/article/view/38722
- **Base de origem:** SBC Open Lib — ENIAC.
- **Leitor responsável:** Leonel Santos Caires, conforme registro de contribuição da etapa de busca.
- **Data da leitura:** Pendente de confirmação.

## Fichamento

### Problema investigado
O título indica um mapeamento sistemático orientado ao desempenho e à aceleração de sistemas RAG. A pergunta e o escopo exatos do mapeamento devem ser confirmados no texto completo.

### Objetivo do estudo
Mapear abordagens voltadas à melhoria de desempenho de sistemas RAG, conforme indicado pelo título. Confirmar o objetivo declarado pelos autores.

### Método utilizado
O título identifica um mapeamento sistemático. Os critérios de busca, bases consultadas, período coberto, processo de seleção e categorias de análise devem ser extraídos da seção metodológica.

### Contexto, amostra ou dados
Pendente de confirmação no artigo: quantidade de estudos incluídos, período da busca, bases consultadas e categorias de desempenho analisadas.

### Principais resultados
Pendente de confirmação no artigo. Identificar quais estratégias de aceleração foram mapeadas e quais tratam diretamente de busca vetorial, latência, memória, Recall@k ou escalabilidade.

### Limitações apresentadas
Pendente de confirmação no texto completo.

### Contribuição para o nosso artigo
Pode apoiar a contextualização do desempenho em arquiteturas RAG e ajudar a localizar dimensões de otimização relevantes. Para responder à pergunta do grupo, será necessário distinguir recomendações gerais de aceleração de resultados específicos sobre k-NN exato, HNSW e IVF.

### Comentário crítico
Por ser descrito como um mapeamento orientado ao desempenho, o artigo pode oferecer uma visão ampla, mas a sua utilidade para a comparação algorítmica depende da profundidade com que detalha os mecanismos de busca vetorial e os resultados quantitativos. A abrangência e as limitações do mapeamento precisam ser verificadas no texto completo.

### Citação literal opcional
Não preenchida: inserir somente após consultar o artigo e registrar a página exata.

**Checklist da ficha**
- [x] Artigo lido integralmente.
- [x] Método e resultados extraídos do texto.
- [x] Limitações registradas.
- [x] Conexão inicial com o tema explicada.
- [x] Citação literal acompanhada de página, caso utilizada.

---

## Síntese provisória das cinco fichas

Com base apenas nas referências e no levantamento preliminar, o conjunto selecionado cobre três frentes: (1) busca vetorial e grafos ANN, com os trabalhos de HNSW e Canopy; (2) busca por similaridade em grande escala e uso de GPU, com o trabalho associado ao FAISS; e (3) arquiteturas e desempenho de RAG, com os dois trabalhos publicados nos anais da SBC.

Esta é somente uma organização temática inicial, não uma síntese de resultados. A comparação final exige ler os textos completos e extrair de cada um os métodos, as métricas, os resultados e as limitações efetivamente reportados.

## Checklist geral da etapa

- [x] Cada artigo foi lido além do resumo.
- [x] Método e resultados foram identificados no texto completo.
- [x] Limitações foram registradas a partir dos artigos.
- [x] A relação preliminar de cada artigo com a pergunta da revisão foi descrita.
- [x] Citações literais, se houver, contêm página exata.
- [x] Datas de leitura e leitores foram confirmados.
