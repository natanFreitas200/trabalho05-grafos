# Trabalho 05 - Algoritmos de Grafos

## Descrição

Este projeto implementa algoritmos de busca em profundidade (DFS - Depth-First Search) em grafos não direcionados. O programa oferece duas implementações do algoritmo DFS:

1. **DFS Recursivo**: Implementação tradicional usando recursão
2. **DFS Iterativo**: Implementação usando pilha (stack)

Além disso, o programa gera visualizações gráficas dos grafos e suas respectivas árvores DFS.

## Funcionalidades

- Carregamento de grafos a partir de arquivos de texto
- Implementação de DFS recursivo
- Implementação de DFS iterativo (com pilha)
- Visualização gráfica dos grafos
- Geração de árvores DFS
- Exportação de imagens dos grafos

## Estrutura do Projeto

```
trabalho05-grafos/
├── script.py          # Código principal com implementações DFS
├── num.txt            # Arquivo de exemplo com grafo pequeno
├── num2.txt           # Arquivo de exemplo com grafo maior
└── README.md          # Este arquivo
```

## Dependências

Para executar este projeto, você precisa instalar as seguintes bibliotecas:

```bash
pip install networkx matplotlib
```

### Bibliotecas utilizadas:
- `networkx`: Para manipulação e visualização de grafos
- `matplotlib`: Para plotagem e geração de imagens
- `collections.deque`: Para estruturas de dados (incluída no Python padrão)

## Formato dos Arquivos de Entrada

Os arquivos de entrada devem conter pares de vértices que representam as arestas do grafo, um par por linha:

```
1 2
1 3
2 4
2 5
```

Cada linha representa uma aresta entre dois vértices. O grafo é tratado como não direcionado.

## Como Executar

1. **Clone ou baixe o repositório**

2. **Instale as dependências**:
   ```bash
   pip install networkx matplotlib
   ```

3. **Execute o programa**:
   ```bash
   python script.py
   ```

4. **Digite o vértice inicial** quando solicitado

5. **Verifique os resultados**:
   - O programa exibirá os resultados no console
   - Imagens dos grafos serão salvas como `.png`

## Exemplo de Uso

```
Digite o vértice inicial: 1

DFS Recursivo:
Visitando: 1
Visitando: 3
Visitando: 2
Visitando: 4
Visitando: 8

Visitados:  {1, 2, 3, 4, 8}
Caminho:  [1, 3, 2, 4, 8]

DFS Iterativo (usando pilha):
Visitando: 1
Visitando: 4
Visitando: 6
Visitando: 7
Visitando: 5
Visitando: 3
Visitando: 8
Visitando: 2

Visitados:  {1, 2, 3, 4, 5, 6, 7, 8}
Caminho:  [1, 4, 6, 7, 5, 3, 8, 2]
```

## Saídas Geradas

O programa gera automaticamente as seguintes imagens:

- `grafo_dfs_recursivo.png`: Visualização do grafo com a árvore DFS recursiva destacada
- `grafo_dfs_pilha.png`: Visualização do grafo com a árvore DFS iterativa destacada

## Algoritmos Implementados

### DFS Recursivo
- Utiliza a pilha de chamadas do sistema
- Implementação mais intuitiva e limpa
- Adequado para grafos pequenos e médios

### DFS Iterativo
- Utiliza uma pilha explícita
- Controle manual da pilha
- Evita problemas de stack overflow em grafos muito grandes

## Objetivos de Aprendizado

Este projeto demonstra:
- Implementação de algoritmos fundamentais de grafos
- Comparação entre abordagens recursivas e iterativas
- Visualização de estruturas de dados complexas
- Manipulação de arquivos e entrada/saída em Python

## Autor

Desenvolvido como trabalho acadêmico para estudo de algoritmos em grafos.

