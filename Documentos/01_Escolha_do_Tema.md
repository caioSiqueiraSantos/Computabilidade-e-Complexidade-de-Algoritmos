# Etapa 1 Tema e delimitação

## Solicitação

Defina um tema específico, relevante e viável para o artigo de revisão bibliográfica.

## Identificação

- Grupo: 3
- Integrantes: Caio Siqueira Santos, Elton Dos Santos Rodrigues, Fillipy Mendes Vilela, Leonardo Masanao, Leonel Santos Caires, Matheus Henrique da Trindade
- Data: 08/10/2026

## Preenchimento

### Área geral

Complexidade e escalabilidade de algoritmos de busca vetorial e indexação aplicados a Inteligência Artificial e RAG (Retrieval-Augmented Generation).

### Tema delimitado

Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI

### Do tema amplo ao específico

- Tema amplo: IA Generativa, RAG e Suporte de TI
- Objeto estudado: Algoritmos de busca vetorial exata e aproximada (k-NN exato por força bruta, HNSW baseado em grafos de proximidade multicamadas e IVF baseado em particionamento em clusters de Voronoi).
- Contexto ou aplicação: Sistemas RAG (Retrieval-Augmented Generation) aplicados a chatbots de suporte interno de TI (Helpdesk corporativo).
- Aspecto que será analisado: Complexidade assintótica temporal (indexação e consulta), complexidade de espaço (consumo de memória RAM), escalabilidade e métricas de desempenho/qualidade (Recall@k e latência).
- O que ficará fora do estudo: Avaliação de serviços ou softwares comerciais fechados, ajuste fino (fine-tuning) ou treinamento de modelos de linguagem (LLMs), engenharia de prompt e métodos de recuperação puramente lexicais/tradicionais (como BM25 puro).

### Justificativa

Em arquiteturas de busca semântica e RAG, a eficiência da recuperação da informação depende fundamentalmente da estrutura de dados e dos algoritmos de indexação vetorial. Compreender as trocas computacionais (trade-offs) entre precisão absoluta, uso de memória RAM e tempo de resposta (latência) nos algoritmos de busca vetorial é essencial para a Ciência da Computação. O estudo beneficia a academia ao comparar métodos exatos e aproximados em cenários práticos de Helpdesk, bem como o mercado corporativo, permitindo dimensionar sistemas de suporte eficientes e escaláveis.

### Viabilidade

- Há artigos científicos disponíveis? Há artigos científicos disponíveis? Sim (artigos seminais como Malkov & Yashunin e Johnson et al./FAISS, além de publicações em anais da SBC).
- O tema pode ser estudado no prazo? Sim (abordagem analítica e comparativa com base em literatura consolidada e benchmarks públicos).
- O grupo possui acesso às fontes necessárias? Sim (bases SBC Open Lib, arXiv, IEEE Xplore e bibliotecas de código aberto como FAISS).

## Produto da etapa

Tema delimitado e justificativa.

## Checklist

- [X] O tema é específico.
- [X] O tema é relevante.
- [X] O tema é viável.
- [X] O recorte está claro.
- [X] O tema foi validado pelo professor.

## Contribuições

| Integrante | Atividade realizada |
| Caio Siqueira Santos | Pesquisou a fundamentação teórica sobre k-NN exato (força bruta) e redigiu a justificativa de relevância. |
| Elton Dos Santos Rodrigues | Estruturou o afunilamento do tema e elaborou a formulação da problemática central. |
| Fillipy Mendes Vilela | Mapeou a viabilidade técnica e levantou dados de complexidade do algoritmo HNSW (grafos). |
| Leonardo Masanao | Realizou levantamento preliminar sobre o algoritmo IVF (clusters/arquivos invertidos) e escopo de exclusão. |
| Leonel Santos Caires | Ajustou o escopo da área geral de interesse e adequou o tema ao feedback da orientação. |
| Matheus Henrique da Trindade | Organizou a consolidação dos dados no template, revisou o checklist e estruturou o registro de contribuições. |
