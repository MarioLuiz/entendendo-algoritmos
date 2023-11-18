# Cap 7: Algoritmo de Dijkstra

O algoritmo de Dijkstra tem quatro passos:

1. Encontre o vértice mais “barato”. Esse é o vértice em que você consegue chegar no menor tempo possível. 
2. Verique se há um caminho mais barato para os vizinhos desse vértice.
Caso exista, atualize os custos deles.
3. Repita até que você tenha feito isso para cada vértice do grafo.
4. Calcule o caminho final.

Um grafo com pesos é chamado de grafo ponderado (também chamado de grafo valorado). Um grafo sem pesos é chamado de grafo não ponderado (também chamado de grafo não valorado).

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/051c2763-dcc9-4601-8bf0-c623948760b8/2859e540-ca78-45b9-9d27-dbf39bc1eb64/Untitled.png)

- Você não pode usar o algoritmo de Dijkstra se você tiver arestas com pesos negativos.
- Se quiser encontrar o caminho mínimo em um grafo contendo arestas com pesos negativos, existe um algoritmo especíco para isso! Ele é chamado de algoritmo de Bellman-Ford.

## Implementação

- Para implementar esse algoritmo você precisará de três tabelas Hash: Grafo, Custos e Pais.
- As tabelas Hash Custo e Pais serão atualizadas conforme o algoritmo for executado.