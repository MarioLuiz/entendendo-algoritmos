# Cap 7: Algoritmo de Dijkstra

O algoritmo de Dijkstra tem quatro passos:

1. Encontre o vértice mais “barato”. Esse é o vértice em que você consegue chegar no menor tempo possível. 
2. Verique se há um caminho mais barato para os vizinhos desse vértice.
Caso exista, atualize os custos deles.
3. Repita até que você tenha feito isso para cada vértice do grafo.
4. Calcule o caminho final.

Um grafo com pesos é chamado de grafo ponderado (também chamado de grafo valorado). Um grafo sem pesos é chamado de grafo não ponderado (também chamado de grafo não valorado).

![image](https://github.com/MarioLuiz/entendendo-algoritmos/assets/11471499/ed9caf2f-705d-4fe7-9a8e-e092f0ab30fd)

- A pesquisa em largura é usada para calcular o caminho mínimo para um
grafo não ponderado.
- O algoritmo de Dijkstra é usado para calcular o caminho mínimo para
um grafo ponderado.
- Você não pode usar o algoritmo de Dijkstra se você tiver arestas com pesos negativos.
- O algoritmo de Dijkstra funciona quando todos os pesos são positivos.
- Se quiser encontrar o caminho mínimo em um grafo contendo arestas com pesos negativos, existe um algoritmo especíco para isso! Ele é chamado de algoritmo de Bellman-Ford.

## Implementação

- Para implementar esse algoritmo você precisará de tres tabelas Hash: Grafo, Custos e Pais e precisará de um array para guardar todos os vétices processados.
- As tabelas Hash Custo e Pais e também o array Processados serão atualizadas conforme o algoritmo for executado.
- Algoritmo da implementação do Dijkstra:
![image](https://github.com/MarioLuiz/entendendo-algoritmos/assets/11471499/c431b6bb-8b3d-43c2-b9a0-3a34ad88aad6)

