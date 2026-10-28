# Velocidade e Qualidade com Estruturas de Dados e Algoritmos

Exercícios, implementações e materiais da disciplina **Velocidade e Qualidade com Estruturas de Dados e Algoritmos**, do **Instituto Infnet**.

[← Voltar para o início do repositório](..)

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| [`TP1_Teste_de_Performance.ipynb`](TP1_Teste_de_Performance.ipynb) | Teste de Performance 1: list comprehension e raciocínio algorítmico (ordenação de um baralho com restrições). |
| [`TP2_Teste_de_Performance.ipynb`](TP2_Teste_de_Performance.ipynb) | Teste de Performance 2: hash tables, ordenações quadráticas, pilhas e filas. |
| [`TP3_Teste_de_Performance.ipynb`](TP3_Teste_de_Performance.ipynb) | Teste de Performance 3: recursão, programação dinâmica, QuickSort e QuickSelect. |
| [`AT_Assessment.ipynb`](AT_Assessment.ipynb) | Assessment final: busca, ordenação, BST, hashtable, pilha/fila, árvore de expressão e simulador de eventos. |

## Conteúdo de cada notebook

### TP1: Fundamentos
- List comprehension para filtrar caracteres de uma string.
- Elaboração de um algoritmo de ordenação de cartas sob restrições de manipulação.

### TP2: Estruturas de dados e ordenação básica
- **Hash tables:** comparação entre solução quadrática (laços aninhados) e solução `O(N)` para encontrar o maior número único, com contagem de comparações e acessos.
- Interseção de arrays em tempo linear, primeiro valor duplicado, letra ausente do alfabeto e primeiro caractere não repetido.
- **Selection Sort** e **Insertion Sort** instrumentados, com análise de melhor e pior caso.
- **Pilha** (`Stack`) com tratamento de overflow e underflow, e **fila** (`Queue`) circular com ponteiros de início e fim.
- Reversão de string usando pilha.
- Análise de qualidade de funções hash e distribuição de chaves.

### TP3: Recursão e algoritmos avançados
- Multiplicação recursiva por soma, com rastreamento das chamadas e retornos.
- Fatoração recursiva de inteiros e potenciação recursiva com expoentes negativos.
- Navegação recursiva em estrutura de diretórios.
- Geração recursiva de combinações (times) e problema da mochila com backtracking.
- Análise de complexidade exponencial e otimização com **programação dinâmica (memoização)**.
- **QuickSort** instrumentado (comparações e cópias) em entradas ordenadas, invertidas e aleatórias.
- **QuickSelect** e comparação de custo com o QuickSort.

### AT: Assessment
1. **Busca:** busca linear e binária instrumentadas, verificação de pré-condição com "falha rápida" e busca em lista encadeada.
2. **Ordenações quadráticas:** Bubble, Selection e Insertion Sort em quatro padrões de entrada, e validação por **BST** com travessia in-order.
3. **Otimização orientada a Big O:** deduplicação `O(n²)` vs `O(n)`, `k_smallest` por ordenação vs QuickSelect, `k_smallest_bst`, e busca e deleção na BST.
4. **Hashtable com encadeamento:** `HashTableChained` feita do zero, com rehash automático por fator de carga e cenário adversarial de colisões.
5. **Pilha e fila com invariantes:** capacidade fixa, exceções específicas, árvore binária de expressão a partir de notação pós-fixa e avaliação recursiva vs iterativa.
6. **Simulador de checkout:** quatro filas, tratamento de overflow e underflow, logs e índice dos clientes atendidos em uma BST.

## Observações

- Por terem sido executados no Google Colab, algumas saídas refletem o ambiente dele. Por exemplo, a listagem de diretórios do exercício 4 do TP3 mostra as pastas padrão do Colab (`.config` e `sample_data`).
- O notebook `TP2` pode ser executado em Python 3.7 ou superior, pois depende da ordem de inserção dos dicionários.
- A biblioteca `pandas` é usada para exibir as tabelas de resultados no `AT_Assessment.ipynb`.
