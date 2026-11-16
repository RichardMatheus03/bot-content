# Grafos — Lista e Matriz de Adjacência

Notebook da disciplina **EDB II (UFRN)**, **Grupo D**, para o Google Colab.

- Richard Matheus Bezerra Ataliba
- Mateus Ferreira Torres Galvão
- Jefferson Deylane Costa dos Santos

O arquivo `colab_base_jefferson.ipynb` é o notebook base do Jefferson. O arquivo `grafos_lista_matriz.ipynb` foi desenvolvido a partir dele (o cabeçalho `#jefferson - mateus -  Richard` permanece) e usa o grafo dos slides da aula.

## Grafo da aula

Vértices: A, B, C, D.

Arestas não direcionadas e sem peso: **(A, B), (A, C), (B, C), (B, D), (C, D)**.

Não existe a aresta (A, D). A matriz é simétrica.

```text
A ----- B
| \     |
|  \    |
C ----- D
```

## O que o notebook cobre

- Classes `GrafoLista` e `GrafoMatriz`, só com a biblioteca padrão do Python.
- Grafo direcionado ou não, com peso ou sem peso.
- Incluir e remover vértice, incluir e remover aresta, consultar aresta, vizinhos, grau, grau de entrada e grau de saída, imprimir.
- Tabela de complexidade de tempo e de espaço, lista contra matriz.
- O grafo da aula nas duas representações.
- Um exemplo direcionado com pesos.
- Conversão lista ↔ matriz.
- Medição de tempo e de memória num ciclo esparso e num grafo completo.
- Testes com `assert`.
- Exemplos curtos de rede social (amizade e seguir) e de mapas (distância e rua de mão única).

O notebook já foi executado de ponta a ponta: as saídas estão gravadas nas células. Abrir no Colab e executar de novo repete os testes.

## Como executar

### Google Colab

1. Abra [Google Colab](https://colab.research.google.com/).
2. Envie `grafos_lista_matriz.ipynb` (*File → Upload notebook*).
3. Use *Ambiente de execução → Executar tudo*.

Não há pacote para instalar.

### Neste repositório

Na pasta `grafos-edb2`, com Python 3:

```bash
pip install jupyter nbclient ipykernel
jupyter nbconvert --execute --inplace grafos_lista_matriz.ipynb
```

Se algum `assert` falhar, o comando termina com erro e a célula aponta a linha.
