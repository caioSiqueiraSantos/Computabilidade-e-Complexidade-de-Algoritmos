# Etapa 10 Preparação da apresentação

## Solicitação

Prepare uma apresentação clara do artigo e organize a participação do grupo.

## Dados da apresentação

- Título do artigo: Complexidade Computacional, Escalabilidade e Qualidade de Recuperação entre Algoritmos de Busca Vetorial (k-NN Exato, HNSW e IVF) em Sistemas RAG para Suporte de TI: Uma Revisão Bibliográfica
- Evento ou disciplina: Computabilidade e Complexidade de Algoritmos — Ciência da Computação (Orientadora: Prof.ª Andrea Ono Sakai)
- Data: 20/11/2026
- Tempo disponível: 15 minutos (12 minutos de exposição oral + 3 minutos para arguição)
- Integrantes: Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires e Matheus Henrique da Trindade

## Estrutura
po
| Parte | Conteúdo principal | Responsável | Tempo |
|---|---|---|---:|
| Abertura | Contextualização de arquiteturas RAG em chatbots de suporte interno de TI (*Helpdesk*), representação semântica por *embeddings* e apresentação do problema de pesquisa. | Elton Dos Santos Rodrigues | 2 min |
| Objetivos | Apresentação do objetivo geral e dos quatro objetivos específicos, destacando os critérios de comparação: complexidade assintótica de tempo e espaço, memória RAM, escalabilidade, *Recall@k* e latência. | Caio Siqueira Santos | 2 min |
| Metodologia | Estratégia da revisão bibliográfica narrativa estruturada: bases consultadas (SBC Open Lib, IEEE Xplore, arXiv e ResearchGate), strings booleanas, critérios de elegibilidade e funil de triagem (14 brutos $\rightarrow$ 12 únicos $\rightarrow$ 7 lidos na íntegra $\rightarrow$ 5 incluídos). | Leonel Santos Caires | 2 min |
| Resultados da revisão | Síntese comparativa dos 3 Eixos: Eixo 1 (HNSW em $\mathcal{O}(efSearch \cdot \log n)$ e variantes *Multi-Graph* e *Bridged-HNSW* com *Canopy Clustering*); Eixo 2 (*k*-NN exato em $\mathcal{O}(n \cdot d)$, *warpSelect* em GPU e particionamento IVF/PQ no FAISS); e Eixo 3 (*chunking* ancorado, busca híbrida com filtros de metadados e aceleração de TTFT / *KV-cache*). | Fillipy Mendes Vilela e Leonardo Masanao | 4 min |
| Conclusão | Resposta direta à pergunta de pesquisa com base na Tabela Comparativa de *trade-offs*, diretrizes práticas de dimensionamento para bases de *Helpdesk* de TI, limitações da revisão e trabalhos futuros. | Matheus Henrique da Trindade | 2 min |

## Mensagem principal

Não existe um algoritmo de busca vetorial universalmente superior em todas as dimensões de complexidade: o dimensionamento eficiente de sistemas RAG para suporte de TI exige equilibrar o trilema entre latência de consulta, consumo de memória RAM e precisão (*Recall@k*). Enquanto o *k*-NN exato ($\mathcal{O}(n \cdot d)$) garante 100% de revocação para bases pequenas, o HNSW (e sua variante *Bridged-HNSW*) entrega a menor latência de consulta ($\mathcal{O}(\log n)$) quando há memória RAM disponível, e o IVF/PQ viabiliza a escalabilidade para milhões ou bilhões de vetores sob memória restrita, especialmente quando integrado a *chunking* ancorado por seções e filtros estruturados de metadados.

## Perguntas esperadas

1. Pergunta: *Por que o algoritmo HNSW consegue reduzir a complexidade de consulta para escala logarítmica, e como as variantes com Canopy Clustering (Pinheiro e Lima, 2025) alteram esse comportamento?*  
   Resposta: O HNSW (MALKOV; YASHUNIN, 2020) organiza os vetores em um grafo multicamadas inspirado em *skip lists*, separando conexões longas nas camadas superiores e conexões curtas na base, com grau máximo limitado por $M$, o que resulta em busca $\mathcal{O}(efSearch \cdot \log n)$, mas exige memória $\mathcal{O}(n \cdot (d + M))$ e construção $\mathcal{O}(n \cdot M \cdot efConstruction \cdot \log n)$. Sob similaridade do cosseno em alta dimensão, Pinheiro e Lima (2025) mostram que decompor o grafo via *Canopy Clustering* em subgrafos independentes (*Multi-Graph HNSW*) reduz o custo de construção para alto *Recall@100*, porém aumenta a latência de consulta pela fusão de resultados; já a variante *Bridged-HNSW* conecta os *canopies* por pontes e sementes globais, preservando alto *Recall@100* com tempo de consulta próximo ao HNSW puro.
2. Pergunta: *Em qual cenário de suporte de TI o índice IVF (Inverted File Index) supera o HNSW, e qual é a origem da sua perda de precisão (Recall@k)?*  
   Resposta: Conforme demonstrado por Johnson, Douze e Jégou (2021), o IVF (especialmente acoplado à Quantização de Produto — IVF-PQ) supera o HNSW quando o acervo atinge dezenas de milhões a bilhões de vetores ou quando há severa restrição de memória RAM/VRAM, pois particiona o espaço em $k_{centroids}$ células de Voronoi via *k-means* e comprime os vetores sem armazenar listas de adjacência de grafos. A perda de *Recall@k* decorre do efeito de borda nas fronteiras das células de Voronoi — quando vizinhos reais estão em células adjacentes não visitadas pelo hiperparâmetro $n_{probe}$ — e do erro de aproximação introduzido pela quantização dos subvetores.
3. Pergunta: *De que maneira as otimizações arquiteturais de RAG analisadas por Brakes et al. (2024) e Silva, Oliveira e Galvão Filho (2024) impactam a busca vetorial em um chatbot de Helpdesk de TI?*  
   Resposta: Elas atuam antes, durante e depois do índice vetorial: antes da busca, o saneamento textual e o *chunking* ancorado por seções com pré-contexto reduziram a média de tokens por *chunk* em $66,78\%$ e elevaram o *Recall@10* em $+181,1\%$ (BRAKES et al., 2024); durante a recuperação, a combinação de filtros estruturados de metadados (análogos a sistema afetado, versão e código de erro em TI) com a busca vetorial e *fallback* reduziu a latência fim-a-fim em $-24,1\%$ e aumentou o *MRR@10* em $+27,5\%$; e, na camada de serviço, técnicas de reuso de *KV-cache* orientado a prefixo e paralelismo de *pipeline* reduzem drasticamente o *Time-to-First-Token* (TTFT) (SILVA; OLIVEIRA; GALVÃO FILHO, 2024).

## Checklist

- [x] A apresentação respeita o tempo.
- [x] Os slides possuem pouco texto e boa legibilidade.
- [x] As fontes das imagens e dados foram informadas.
- [x] Todos conhecem o problema, o método e as conclusões.
- [x] O grupo realizou pelo menos um ensaio completo.
- [x] Os integrantes estão preparados para responder perguntas.

## Contribuições

| Integrante | Atividade realizada |
|---|---|
| Caio Siqueira Santos | Estruturou o bloco de Objetivos da apresentação e revisou os critérios de avaliação assintótica. |
| Elton Dos Santos Rodrigues | Estruturou o bloco de Abertura (contexto de RAG em suporte de TI e problema de pesquisa). |
| Fillipy Mendes Vilela | Elaborou a síntese oral do Eixo 1 (HNSW e complexidade em grafos) e redigiu a resposta da Pergunta Esperada 1. |
| Leonardo Masanao | Elaborou a síntese oral do Eixo 2 (FAISS, *k*-NN em GPU e IVF/PQ) e redigiu a resposta da Pergunta Esperada 2. |
| Leonel Santos Caires | Estruturou o bloco de Metodologia e redigiu a resposta da Pergunta Esperada 3 sobre otimizações em sistemas RAG. |
| Matheus Henrique da Trindade | Estruturou o bloco de Conclusão, redigiu a Mensagem Principal e organizou a distribuição de tempo entre os integrantes. |
