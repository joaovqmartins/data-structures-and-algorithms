# Estruturas de Dados e Algoritmos Avançados

Exercícios, implementações e materiais da disciplina **Estruturas de Dados e Algoritmos Avançados**, do **Instituto Infnet**.

[← Voltar para o início do repositório](..)

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| [`TP1_Teste_de_Performance.ipynb`](TP1_Teste_de_Performance.ipynb) | Teste de Performance 1: heap binária máxima implementada do zero, com análise teórica e empírica. |
| [`TP2_Teste_de_Performance.ipynb`](TP2_Teste_de_Performance.ipynb) | Teste de Performance 2: Trie (autocomplete e autocorrect) e grafos (lista e matriz de adjacência), integrados e exportados em Mermaid. |

## Conteúdo de cada notebook

### TP1: Heap binária
1. **Motivação:** uso de heaps em um problema real de priorização dinâmica (fila de pronto-socorro).
2. **Estrutura:** classe `BinaryHeap` (heap máxima) usando apenas uma lista, com funções de índice de pai e filhos e invariantes documentadas.
3. **Inserção:** `insert` com *sift-up* e registro de cada troca.
4. **Remoção da raiz:** `extract_max` com *sift-down*, passo a passo até a heap ficar vazia.
5. **Busca:** `contains` linear e por que a heap não serve para buscas frequentes.
6. **Remoção arbitrária:** `delete` com reorganização por *sift-up* ou *sift-down*.
7. **Validação:** `is_valid_heap` para verificar se um array é uma heap válida.
8. **Construção em `O(n)`:** `build_heap` pelo algoritmo de Floyd, sem inserções individuais.
9. **Comparação:** `build_heap` vs inserção incremental, com contagem de operações.
10. **Heap sort parcial:** os k maiores elementos sem ordenar o array todo.
11. **Análise empírica:** contagem de operações em tamanhos crescentes, comparada com a teoria.
12. **Documentação:** arquitetura, decisões algorítmicas e roteiro para a apresentação em vídeo.

### TP2: Trie e grafos
1. **Trie:** classes `TrieNode` e `Trie`, com inserção e marcação de fim de palavra (`is_end`).
2. **Busca exata:** `search`, diferenciando prefixo existente de palavra completa.
3. **Busca por prefixo:** `starts_with` como base do autocomplete.
4. **Traversal:** `collect_words` / `_collect_words`, sem perdas nem duplicações.
5. **Autocomplete:** `autocomplete(prefix, k)` em ordem lexicográfica, com parada antecipada.
6. **Autocorrect:** maior prefixo compartilhado, com critério de desempate explícito.
7. **Lista de adjacência:** classe `GraphAdjList` com `add_vertex` e `add_edge`.
8. **Matriz de adjacência:** classe `GraphAdjMatrix` e comparação de memória e consulta com a lista.
9. **Definições operacionais:** vértice, aresta, lista e matriz, apontados no próprio código.
10. **Exportação Mermaid:** `to_mermaid` sem duplicação de arestas.
11. **Integração:** Trie como índice de vértices (`find_vertices_by_prefix`).
12. **Decisões de Projeto e Complexidade:** tabelas em Big O, escolha de representação e decisões justificadas.

## Observações

- A biblioteca `pandas` é usada para exibir as tabelas de resultados do exercício 11 do TP1.
