# Etapa 2 Problema de pesquisa

## Solicitação

Transforme o tema em uma pergunta clara, específica e respondível por meio da literatura científica.

## Tema aprovado

Complexidade e escalabilidade de algoritmos de busca vetorial em chatbots RAG para suporte de TI

## Pergunta de pesquisa

Como a literatura compara a complexidade computacional, uso de memória, escalabilidade e qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte de TI?

## Verificação

- O que se deseja descobrir ou compreender? 
Compreender os trade-offs algorítmicos entre tempo de processamento (latência e complexidade assintótica), consumo de memória RAM, capacidade de escala e eficácia na recuperação da informação (Recall@k) ao confrontar métodos exatos e aproximados.
- Qual é o objeto da pergunta? 
Três algoritmos fundamentais de busca vetorial: k-NN exato por força bruta (Flat), HNSW (Hierarchical Navigable Small World baseado em grafos de proximidade) e IVF (Inverted File Index baseado em particionamento em clusters de Voronoi).
- Qual é o contexto ou recorte? 
Sistemas de recuperação de informação semântica em arquiteturas RAG (Retrieval-Augmented Generation) aplicadas a chatbots de atendimento e suporte interno de TI (Helpdesk).
- A pergunta pode ser respondida por artigos científicos? 
Sim. Justificativa: Existe ampla produção científica teórica e experimental sobre algoritmos de busca por vizinhos mais próximos (Nearest Neighbors), relatórios técnicos de bibliotecas de referência (como FAISS) e artigos de eventos da SBC (como SBSI e ENIAC) que documentam formalmente as ordens de complexidade de tempo/espaço e os resultados empíricos de benchmarks.
- Por que essa pergunta é relevante? 
Porque bases de conhecimento corporativas crescem continuamente e a busca exata (k-NN) torna-se computacionalmente proibitiva em larga escala. Responder a essa pergunta permite mapear formalmente os limites de desempenho dos métodos aproximados (HNSW e IVF), orientando o dimensionamento eficiente de infraestrutura de TI corporativa.

## Produto da etapa

Pergunta de pesquisa aprovada.

## Checklist

- [X] Está escrita em forma de pergunta.
- [X] É clara e objetiva.
- [X] Está alinhada ao tema.
- [X] Pode ser respondida por revisão bibliográfica.
- [X] Não exige experimento que não será realizado.

## Contribuições

| Integrante | Atividade realizada |
| Elton Dos Santos Rodrigues | Formulou a redação inicial da pergunta de pesquisa focando nas variáveis de desempenho e complexidade. |
| Leonel Santos Caires | Refinou a pergunta delimitando o escopo estritamente ao que a literatura científica compara. |
| Caio Siqueira Santos | Redigiu a verificação da viabilidade de resposta por meio de artigos teóricos e experimentais. |
| Fillipy Mendes Vilela | Mapeou e detalhou o objeto da pergunta (estruturas de k-NN, grafos HNSW e arquivos invertidos IVF). |
| Leonardo Masanao | Redigiu o contexto de aplicação e a relevância prática para o dimensionamento em suporte interno de TI. |
| Matheus Henrique da Trindade | Realizou a revisão de clareza, checagem dos critérios do checklist e consolidação do documento. |
