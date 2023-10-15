# Cap 2: Ordenação por Seleção

## Arrays

- Todos os dados de um array são armazenados contiguamente (uma do lado da outra) na memoria.
- Arrays são ótimos se você deseja ler elementos aleatórios.

## Listas Encadeadas

- Cada item da lista armazena o endereço do próximo item da lista. Um monte de endereços aleatórios de memória estão ligados.
- Listas encadeadas são ótimas se você quiser ler todos os itens, um de cada vez.
- Listas encadeadas são melhores caso você queira inserir um elemento no meio de uma lista.
- Listas encadeadas são melhores caso você queira deletar um elemento.

|  | Arrays | Listas |
| --- | --- | --- |
| Leitura | O(1) | O(n) |
| Inserção | O(n) | O(1) |
| Eliminação | O(n) | O(1) |

O(n) = Tempo de execução Linear

O(1) = Tempo de execução constante

## Ordenação por Seleção (Crescente)

1. Criar uma lista Vazia (Para armazenar itens ordenados).
2. Filtrar menor valor na lista desordenada e retornar o indice do elemento.
3. Pegar indice do menor valor no passo 2 e adicionar na nova lista do passo 1.
4. Excluir o indice na lista desordenada no passo 2.
5. Repetir passo 2, 3 e 4 até que a lista desordenada esteja vazia.
6. Retornar a lista ordenada do passo 1.

Tempo de execução O(n × n) ou O(n^2).