# Cap 6: Pesquisa em Largura

- A pesquisa em largura lhe diz se há um caminho de X para Y
- Se esse caminho existir, a pesquisa em largura lhe dará o caminho mínimo.
- Se você tem um problema do tipo "encontre o menor X", tente modelar o seu problema utilizando grafos e use a pesquisa em largura para resolvê-lo.

## O que é um grafo ?

Grafos são formados por vértices(também chamados de nós) e arestas, e um vértice pode ser diretamente conectado a muitos outros vértices, por isso os chamamos de vizinhos.

![image](https://github.com/MarioLuiz/entendendo-algoritmos/assets/11471499/53f07897-f92c-4a33-adc5-17cf4fec3893)


- Grafos não direcionados não contêm setas, e a relação acontece nos dois sentidos (Alex - Rama significa "Alex ficou com Rama e Rama Ficou com Alex").

## Pesquisa em largura

Este algoritmo ajuda a responder a dois tipos de pergunta:

- Existe algum caminho do vértice A até o vértice B?
- Qual o caminho mínimo do vértice A até o vértice B?

## Filas

- Uma fila em estrutura de dados funciona exatamente como uma fila da vida real.
- Não é possível acessar elementos aleatórios em uma fila.
- É possivel duas operações na fila: enqueue (enfileirar) e dequeue (desenfileirar).

![image](https://github.com/MarioLuiz/entendendo-algoritmos/assets/11471499/853cfc04-fee5-4d2f-9bd2-f38bea19d057)


- A fila é uma estrutura de dadso FIFO (Fist in, First Out) ‘Primeiro a entrar, Primeiro a sair’
- A pilha é uma estrutura de dados LIFO (Last In, First Out) ‘Ultimo a entrar, Primeiro a sair’

## Implementando o grafo

- Como expressar uma relação do tipo“você -> bob”? Felizmente, você conhece uma estrutura de dados que lhe permite expressar relações: uma tabela hash!
- Uma tabela hash lhe permite mapear uma chave a um valor. Nesse caso você deseja mapear um vértice a todos os seus vizinhos.

## Tempo de execução

A pesquisa em largura tem tempo de execução O(número de pessoas + número de arestas), que é frequentemente escrito como O(V+A) (V para número de vértices, A para número de arestas).