# Análise Comparativa de Algoritmos de Busca Vetorial em Sistemas RAG

## Sobre o Projeto

Este repositório contém os artefatos e documentos do projeto de pesquisa da disciplina de **Computabilidade e Complexidade de Algoritmos**. 

O estudo foca na análise teórica e comparativa da complexidade e escalabilidade de algoritmos de busca vetorial utilizados em sistemas de Inteligência Artificial, especificamente em arquiteturas **RAG (Retrieval-Augmented Generation)** voltadas para cenários práticos como o suporte de TI.

### Objetivo Principal
Realizar uma avaliação algorítmica formal comparando métodos exatos e aproximados (ANN - *Approximate Nearest Neighbors*) sob o prisma de métricas de complexidade assintótica, uso de recursos computacionais e qualidade de recuperação.

## Algoritmos Analisados

O escopo da pesquisa foca em três abordagens distintas de busca em espaços vetoriais para a análise de *trade-offs*:

1. **k-NN Exato (Flat / Força Bruta):** 
   * Base de referência (100% de acurácia/*recall*).
   * Alta complexidade temporal de busca $\mathcal{O}(n \cdot d)$.
2. **HNSW (*Hierarchical Navigable Small World*):** 
   * Abordagem baseada em grafos multicamadas.
   * Otimização de latência de busca $\mathcal{O}(\log n)$, porém com maior consumo de complexidade espacial (memória RAM).
3. **IVF (*Inverted File Index*):** 
   * Abordagem baseada em particionamento do espaço vetorial (células de Voronoi/clusters via *k-means*).
   * Prioriza menor pegada de memória em troca de maior latência de indexação e leve perda na revocação.

## Métricas e Critérios de Comparação

A análise fundamenta-se nos seguintes pilares da Ciência da Computação:
* **Complexidade Assintótica de Tempo:** Tempo de construção da estrutura de índice vs. tempo de consulta (latência).
* **Complexidade Assintótica de Espaço:** Pegada de memória RAM necessária para armazenar e percorrer as estruturas de dados.
* **Qualidade da Recuperação:** Métrica de *Recall@k*, avaliando a degradação aceitável de acurácia dos métodos aproximados em relação à força bruta.

## Contexto Acadêmico

* **Curso:** Ciência da Computação
* **Disciplina:** Computabilidade e Complexidade de Algoritmos
* **Orientadora:** Prof.ª Andrea Ono Sakai
* **Semestre/Ano:** 2º Semestre / 2026

## Integrantes do Grupo

| Nome | Atuação Principal na Etapa de Definição |
|---|---|
| **Caio** | Fundamentação teórica de busca k-NN e relevância |
| **Elton** | Funil metodológico e definição do problema |
| **Fillipy** | Viabilidade e complexidade de grafos (HNSW) |
| **Leonardo** | Levantamento de literatura e análise de IVF |
| **Leonel** | Delimitação da área e escopo em Ciência da Computação |
| **Matheus** | Consolidação estrutural, documentação e revisão |

---
*Este é um projeto acadêmico desenvolvido exclusivamente para fins de pesquisa e avaliação universitária.*
