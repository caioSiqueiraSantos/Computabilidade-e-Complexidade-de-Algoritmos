# Etapa 3 Objetivo geral e objetivos específicos

## Solicitação

Defina o objetivo geral e os objetivos específicos do artigo.

## Problema de pesquisa

Como a literatura compara a complexidade computacional, uso de memória, escalabilidade e qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte de TI?

## Objetivo geral

Analisar comparativamente a complexidade computacional (tempo e espaço), o consumo de memória, a escalabilidade e a qualidade de recuperação (Recall@k e latência) dos algoritmos de busca vetorial k-NN exato, HNSW e IVF na recuperação de informação de sistemas RAG para suporte interno de TI, com o propósito de evidenciar os principais trade-offs algorítmicos necessários ao dimensionamento eficiente de bases de conhecimento corporativas.

## Objetivos específicos

1. Conceituar a arquitetura RAG (Retrieval-Augmented Generation) e o papel dos embeddings e da recuperação semântica em bases de suporte de TI.
2. Conceituar os princípios de indexação e busca vetorial, diferenciando os métodos exatos (k-NN Flat) dos métodos aproximados por grafos (HNSW) e por agrupamento/particionamento (IVF).
3. Determinar e comparar formalmente a complexidade assintótica de tempo (construção e consulta) e de espaço (memória RAM) dos algoritmos k-NN exato, HNSW e IVF.
4. Analisar a relação entre latência de consulta e a perda de precisão (métrica de Recall@k) introduzida pelos algoritmos aproximados frente à busca exata.

## Quadro de alinhamento

| Elemento | Texto |
| Problema | Como a literatura compara a complexidade computacional, o uso de memória, a escalabilidade e a qualidade (Recall@k e latência) entre os algoritmos de busca vetorial (k-NN exato, HNSW e IVF) em chatbots RAG para suporte interno de TI? |
| Objetivo geral | Analisar comparativamente a complexidade computacional (tempo e espaço), o consumo de memória, a escalabilidade e a qualidade de recuperação (Recall@k e latência) dos algoritmos de busca vetorial k-NN exato, HNSW e IVF na recuperação de informação de sistemas RAG para suporte interno de TI, com o propósito de evidenciar os principais trade-offs algorítmicos necessários ao dimensionamento eficiente de bases de conhecimento corporativas. |
| Resultado esperado | Avaliar os trade-offs operacionais e a escalabilidade dos três algoritmos para orientar o dimensionamento eficiente de bases vetoriais em ambientes corporativos de Helpdesk. |

## Produto da etapa

Um objetivo geral e de três a quatro objetivos específicos.

## Checklist

- [X] Os objetivos começam com verbos no infinitivo.
- [X] O objetivo geral responde ao problema.
- [X] Os objetivos específicos detalham o objetivo geral.
- [X] Os objetivos são compatíveis com uma revisão bibliográfica.
