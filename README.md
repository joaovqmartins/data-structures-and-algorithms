# Estruturas de Dados e Algoritmos

Repositório com exercícios, implementações e materiais de duas disciplinas de estruturas de dados e algoritmos. Trata-se de um projeto acadêmico desenvolvido no **Instituto Infnet**.

Todo o código é escrito em **Python 3** e organizado em notebooks Jupyter (`.ipynb`), desenvolvidos no **Google Colab**. Boa parte das soluções é **instrumentada**: em vez de apenas rodar, os algoritmos contam comparações, cópias e acessos, para que a análise de complexidade (Big O) seja baseada em evidências medidas.

## Disciplinas

| # | Disciplina | Pasta | Atividades |
|---|---|---|---|
| 1 | Velocidade e Qualidade com Estruturas de Dados e Algoritmos | [`01-velocidade-e-qualidade`](01-velocidade-e-qualidade) | TP1, TP2, TP3 e Assessment |
| 2 | Estruturas de Dados e Algoritmos Avançados | [`02-algoritmos-avancados`](02-algoritmos-avancados) | TP1 |

Cada pasta tem o seu próprio `README.md`, com a descrição de cada notebook.

## Estrutura do repositório

```
data-structures-and-algorithms/
├── README.md
├── 01-velocidade-e-qualidade/
│   ├── README.md
│   ├── TP1_Teste_de_Performance.ipynb
│   ├── TP2_Teste_de_Performance.ipynb
│   ├── TP3_Teste_de_Performance.ipynb
│   └── AT_Assessment.ipynb
└── 02-algoritmos-avancados/
    ├── README.md
    └── TP1_Teste_de_Performance.ipynb
```

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

Os notebooks usam principalmente a biblioteca padrão do Python (`random`, `math`, `os`, `sys`, `collections`). A biblioteca `pandas` é usada para exibir as tabelas de resultados no Assessment da disciplina 1 e no TP1 da disciplina 2.

## Observações

- Os notebooks incluem enunciados, código, saídas de execução e análises escritas em Markdown.
- Algumas saídas dependem de números aleatórios, então os valores exatos podem variar entre execuções.

## Autor

Desenvolvido por [@joaovqmartins](https://github.com/joaovqmartins) como projeto acadêmico do Instituto Infnet.
