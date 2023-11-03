# Cap 6: Pesquisa em Largura

- A pesquisa em largura lhe diz se há um caminho de X para Y
- Se esse caminho existir, a pesquisa em largura lhe dará o caminho mínimo.
- Se você tem um problema do tipo "encontre o menor X", tente modelar o seu problema utilizando grafos e use a pesquisa em largura para resolvê-lo.

## O que é um grafo ?

Grafos são formados por vértices(também chamados de nós) e arestas, e um vértice pode ser diretamente conectado a muitos outros vértices, por isso os chamamos de vizinhos.

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/051c2763-dcc9-4601-8bf0-c623948760b8/93cb9adc-4048-4e01-9744-106108db52d5/Untitled.png)

- Grafos não direcionados não contêm setas, e a relação acontece nos dois sentidos (Alex - Rama significa "Alex ficou com Rama e Rama Ficou com Alex").

## Pesquisa em largura

Este algoritmo ajuda a responder a dois tipos de pergunta:

- Existe algum caminho do vértice A até o vértice B?
- Qual o caminho mínimo do vértice A até o vértice B?

## Filas

- Uma fila em estrutura de dados funciona exatamente como uma fila da vida real.
- Não é possível acessar elementos aleatórios em uma fila.
- É possivel duas operações na fila: enqueue (enfileirar) e dequeue (desenfileirar).

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/051c2763-dcc9-4601-8bf0-c623948760b8/f26d5260-7225-49b1-93eb-cf93553e67dd/Untitled.png)

- A fila é uma estrutura de dadso FIFO (Fist in, First Out) ‘Primeiro a entrar, Primeiro a sair’
- A pilha é uma estrutura de dados LIFO (Last In, First Out) ‘Ultimo a entrar, Primeiro a sair’

## Implementando o grafo

- Como expressar uma relação do tipo“você -> bob”? Felizmente, você conhece uma estrutura de dados que lhe permite expressar relações: uma tabela hash!
- Uma tabela hash lhe permite mapear uma chave a um valor. Nesse caso você deseja mapear um vértice a todos os seus vizinhos.