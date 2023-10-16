# Cap 1: Introdução a Algoritmos

## Pesquisa Binária

- Pesquisa binária utiliza ‘array’ e só funciona em arrays ordenados.
- Tempo de exeção Logarítimo O(Log n).
- Conforme o Array cresce, a pesquisa binária se torna muito mais rápida.

## Notação Big O

- A notação Big O é uma notação especial que diz o quão rápido é um algoritmo.
- A notação Big O não fornece o tempo em segundos, mas sim em operações.
- A notação Big O estabelece o tempo de execução para a pior hipótese.

## Exemplos comuns de tempo execução Big O

- O(log n), também conhecido como tempo logarítmico. Exemplo: pesquisa binária.
- O(n), conhecido como tempo linear. Exemplo: pesquisa simples.
- O(n * log n). Exemplo: um algoritmo rápido de ordenação, como a ordenação quicksort.
- O(n^2). Exemplo: um algoritmo lento de ordenação, como a ordenação por seleção.
- O(n!) exemplo: algoritimo do caixeiro viajante.

## O caixeiro-viajante

Ele é um problema famoso da ciência da computação, pois seu crescimento é apavorante e algumas pessoas muito inteligentes acreditam que ele possa ser melhorado. Esse algoritmo é chamado de “o problema do caixeiro-viajante”. O caixeiro Opus, quer passar por todas as 5 cidades percorrendo uma distância mínima. Para isso, temos que analisar cada ordem possível de cidades para visitar, somar todas as distâncias.

| Cidades | Operações |
| --- | --- |
| 6 | 720 |
| 7 | 5040 |
| 8 | 40320 |
| ... | ... |
| 15 | 1307674368000 |

O numero de operaçoes aumenta drasticamente… De maneira geral, para n itens, é necessário n! (fatorial de n) operações para chegar a um resultado.
