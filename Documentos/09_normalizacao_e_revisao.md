# Etapa 9 Normalização e revisão final

## Solicitação

Revise o conteúdo, as citações, as referências e a formatação antes da entrega.

## Identificação

- Título do artigo: Complexidade Computacional, Escalabilidade e Qualidade de Recuperação entre Algoritmos de Busca Vetorial (k-NN Exato, HNSW e IVF) em Sistemas RAG para Suporte de TI: Uma Revisão Bibliográfica
- Versão revisada: 1.0
- Data: 16/10/2026
- Responsável pela conferência final: Matheus Henrique da Trindade e Fillipy Mendes Vilela (com validação de Caio Siqueira Santos, Elton Dos Santos Rodrigues, Leonardo Masanao e Leonel Santos Caires)

## Revisão científica

- [x] Tema, problema e objetivos estão alinhados.
- [x] As conclusões respondem ao problema.
- [x] Não existem afirmações sem fonte quando a fonte é necessária.
- [x] As limitações do trabalho foram reconhecidas.
- [x] Não foram incluídos resultados inexistentes.

## Citações e referências

- [x] Toda obra citada aparece nas referências.
- [x] Toda referência listada foi citada no texto.
- [x] Citações diretas contêm página.
- [x] Autores, títulos, anos, DOI e links foram conferidos.
- [x] O padrão exigido foi aplicado de forma consistente.

## Escrita

- [x] O texto possui sequência lógica.
- [x] Os parágrafos apresentam uma ideia principal.
- [x] Foram corrigidos ortografia e concordância.
- [x] Repetições e frases vagas foram eliminadas.
- [x] O texto diferencia descrição de análise crítica.

## Formatação

- [x] O template institucional foi respeitado.
- [x] Títulos e subtítulos estão padronizados.
- [x] Tabelas e figuras possuem identificação e fonte.
- [x] Margens, fonte, espaçamento e paginação foram conferidos.

## Registro das correções

| Seção | Problema encontrado | Correção realizada | Responsável |
|---|---|---|---|
| **Palavras-chave e Introdução** | A versão inicial apresentava cinco palavras-chave e o objetivo geral não encerrava o último parágrafo da Introdução. | Redução para exatamente três palavras-chave conforme o template (`Busca vetorial; Retrieval-Augmented Generation (RAG); Complexidade de algoritmos`) e posicionamento do objetivo geral no fechamento da Introdução. | Caio Siqueira Santos |
| **Metodologia** | Necessidade de distinguir o desenho metodológico do grupo (revisão narrativa) do método de um dos artigos revisados (mapeamento sistemático de Silva, Oliveira e Galvão Filho, 2024). | Explicitação de que o artigo consiste em uma **revisão bibliográfica narrativa estruturada**, preservando os números reais da triagem da Etapa 5 (14 brutos $\rightarrow$ 12 únicos $\rightarrow$ 7 lidos na íntegra $\rightarrow$ 5 incluídos). | Leonel Santos Caires |
| **Revisão da Literatura — Eixo 1** | A descrição inicial da heurística de *Canopy Clustering* (Pinheiro e Lima, 2025) não diferenciava as três arquiteturas avaliadas no artigo completo e mantinha pendências herdadas da Etapa 6. | Consolidação dos dados do texto integral de Pinheiro e Lima (2025), detalhando as ordens de complexidade e os *trade-offs* entre *Baseline HNSW*, *Canopy-Based Multi-Graph HNSW* e *Bridged-HNSW*. | Leonardo Masanao |
| **Revisão da Literatura — Eixos 1 e 2** | Falta de padronização na notação matemática de complexidade assintótica entre grafos (HNSW) e partições de Voronoi (IVF). | Uniformização das expressões em notação $\mathcal{O}(\cdot)$, explicitando os parâmetros $n$, $d$, $M$, $efConstruction$, $efSearch$, $\alpha$, $\gamma$, $k_{centroids}$ e $n_{probe}$. | Fillipy Mendes Vilela |
| **Revisão da Literatura — Eixo 3** | Mistura entre as métricas de otimização de *chunking* e as métricas da busca híbrida com filtros do estudo de Brakes et al. (2024). | Separação exata dos ganhos do saneamento e *chunking* ancorado ($-66,78\%$ de tokens/chunk; $+181,1\%$ em *Recall@10*; $+163,3\%$ em *MRR@10*) dos ganhos da ablação com filtros estruturados ($+15,6\%$ em *Recall@10*; $+27,5\%$ em *MRR@10*; $-24,1\%$ na latência fim-a-fim). | Elton Dos Santos Rodrigues |
| **Síntese Crítica, Resumo e Referências** | Falta de fonte na Tabela 1 e ordenação numérica das referências herdada da Etapa 5. | Inclusão de título numerado e fonte na Tabela 1, revisão do Resumo em parágrafo único e ordenação alfabética estrita das cinco referências segundo a norma ABNT NBR 6023, mantendo a consistência de anos e URLs com as Etapas 5 e 6. | Matheus Henrique da Trindade |

## Contribuições

| Integrante | Atividade realizada |
|---|---|
| Caio Siqueira Santos | Revisou o alinhamento entre tema, problema, palavras-chave e objetivo geral na Introdução e nas Considerações Finais. |
| Elton Dos Santos Rodrigues | Conferiu a distinção das métricas experimentais no Eixo 3 e a consistência lógica entre os achados e a conclusão. |
| Fillipy Mendes Vilela | Conferiu e uniformizou todas as notações de complexidade assintótica de tempo e espaço ao longo do artigo e da Tabela 1. |
| Leonardo Masanao | Verificou a fidelidade técnica da síntese das variantes *Baseline*, *Multi-Graph* e *Bridged-HNSW* e as limitações de escopo. |
| Leonel Santos Caires | Revisou a seção de Metodologia para garantir conformidade com a triagem da Etapa 5 e a distinção entre revisão narrativa e sistemática. |
| Matheus Henrique da Trindade | Realizou a conferência cruzada entre citações no texto e referências em norma ABNT, além de consolidar o registro das correções. |
