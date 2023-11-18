# Cap 7: Algoritmo de Dijkstra

O algoritmo de Dijkstra tem quatro passos:

1. Encontre o vértice mais “barato”. Esse é o vértice em que você consegue chegar no menor tempo possível. 
2. Verique se há um caminho mais barato para os vizinhos desse vértice.
Caso exista, atualize os custos deles.
3. Repita até que você tenha feito isso para cada vértice do grafo.
4. Calcule o caminho final.

Um grafo com pesos é chamado de grafo ponderado (também chamado de grafo valorado). Um grafo sem pesos é chamado de grafo não ponderado (também chamado de grafo não valorado).

![image](https://github.com/MarioLuiz/entendendo-algoritmos/assets/11471499/ed9caf2f-705d-4fe7-9a8e-e092f0ab30fd)

- Você não pode usar o algoritmo de Dijkstra se você tiver arestas com pesos negativos.
- Se quiser encontrar o caminho mínimo em um grafo contendo arestas com pesos negativos, existe um algoritmo especíco para isso! Ele é chamado de algoritmo de Bellman-Ford.

## Implementação

- Para implementar esse algoritmo você precisará de três tabelas Hash: Grafo, Custos e Pais.
- As tabelas Hash Custo e Pais serão atualizadas conforme o algoritmo for executado.
