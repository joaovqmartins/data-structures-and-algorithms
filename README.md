# Estruturas de Dados e Algoritmos

Repositório com exercícios, implementações e materiais da disciplina **Velocidade e Qualidade com Estruturas de Dados e Algoritmos**. Trata-se de um projeto acadêmico desenvolvido no **Instituto Infnet**.

O repositório também inclui o TP1 da disciplina **Estruturas de Dados e Algoritmos Avançados**.

Todo o código é escrito em **Python 3** e organizado em notebooks Jupyter (`.ipynb`), desenvolvidos no **Google Colab**. Boa parte das soluções é **instrumentada**: em vez de apenas rodar, os algoritmos contam comparações, cópias e acessos, para que a análise de complexidade (Big O) seja baseada em evidências medidas.

## Estrutura do repositório

| Arquivo | Conteúdo |
|---|---|
| `TP1_Teste_de_Performance_Estruturas_de_Dados.ipynb` | Teste de Performance 1: list comprehension e raciocínio algorítmico (ordenação de um baralho com restrições). |
| `TP2_Teste_de_Performance_Estruturas_de_Dados.ipynb` | Teste de Performance 2: hash tables, ordenações quadráticas, pilhas e filas. |
| `TP3_Teste_de_Performance_Estruturas_de_Dados.ipynb` | Teste de Performance 3: recursão, programação dinâmica, QuickSort e QuickSelect. |
| `AT_Assessment_Estruturas_de_Dados.ipynb` | Assessment final: busca, ordenação, BST, hashtable, pilha/fila, árvore de expressão e simulador de eventos. |
| `TP1_Teste_de_Performance_Estruturas_de_Dados_Avancados.ipynb` | Teste de Performance 1 de Estruturas de Dados e Algoritmos Avançados: heap binária máxima implementada do zero, com análise teórica e empírica. |

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

### TP1 de Estruturas de Dados e Algoritmos Avançados: Heap binária
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

## Principais conceitos abordados

- Análise de complexidade com Big O (`O(1)`, `O(log n)`, `O(n)`, `O(n log n)`, `O(n²)`, `O(2ⁿ)`)
- Arrays, listas encadeadas, pilhas, filas e filas circulares
- Hash tables, colisões, encadeamento e fator de carga
- Árvores binárias de busca (inserção, busca, deleção e travessias)
- Recursão, backtracking e memoização
- Heaps binárias e filas de prioridade
- Algoritmos de ordenação e seleção (Bubble, Selection, Insertion, QuickSort e QuickSelect)

## Como executar

**Opção 1: Google Colab (recomendada).** Os notebooks foram desenvolvidos no [Google Colab](https://colab.research.google.com/), então é o ambiente em que funcionam sem configuração. Basta abrir o Colab, escolher a aba **GitHub** em *Abrir notebook* e colar a URL do repositório.

**Opção 2: localmente.**

```bash
# clonar o repositório
git clone https://github.com/joaovqmartins/data-structures-and-algorithms.git
cd data-structures-and-algorithms

# instalar as dependências
pip install jupyter pandas

# abrir os notebooks
jupyter notebook
```

Os notebooks usam principalmente a biblioteca padrão do Python (`random`, `math`, `os`, `sys`, `collections`). A biblioteca `pandas` é usada para exibir as tabelas de resultados no `AT_Assessment_Estruturas_de_Dados.ipynb` e no `TP1_Teste_de_Performance_Estruturas_de_Dados_Avancados.ipynb`.

## Observações

- Por terem sido executados no Google Colab, algumas saídas refletem o ambiente dele. Por exemplo, a listagem de diretórios do exercício 4 do TP3 mostra as pastas padrão do Colab (`.config` e `sample_data`).
- Os notebooks incluem enunciados, código, saídas de execução e análises escritas em Markdown.
- Algumas saídas dependem de números aleatórios, então os valores exatos podem variar entre execuções.
- O notebook `TP2` pode ser executado em Python 3.7 ou superior, pois depende da ordem de inserção dos dicionários.

## Autor

Desenvolvido por [@joaovqmartins](https://github.com/joaovqmartins) como projeto acadêmico do Instituto Infnet.
