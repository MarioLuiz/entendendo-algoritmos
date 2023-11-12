# Cap 7: Algoritmo de Dijkstra

O algoritmo de Dijkstra tem quatro passos:

1. Encontre o vértice mais “barato”. Esse é o vértice em que você consegue chegar no menor tempo possível. 
2. Verique se há um caminho mais barato para os vizinhos desse vértice.
Caso exista, atualize os custos deles.
3. Repita até que você tenha feito isso para cada vértice do grafo.
4. Calcule o caminho final.

Um grafo com pesos é chamado de grafo ponderado (também chamado de grafo valorado). Um grafo sem pesos é chamado de grafo não ponderado (também chamado de grafo não valorado).

Image Grafo Ponderado e não ponderado

- Você não pode usar o algoritmo de Dijkstra se você tiver arestas com pesos negativos.
- Se quiser encontrar o caminho mínimo em um grafo contendo arestas com pesos negativos, existe um algoritmo especíco para isso! Ele é chamado de algoritmo de Bellman-Ford.