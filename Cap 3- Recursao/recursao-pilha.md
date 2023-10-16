# Cap 3: Recursão

## Recursão

- Não há nenhum benefício quanto ao desempenho ao utilizar a recursão. Na verdade, os loops algumas vezes são melhores para o desempenho de um programa.
- É mais fácil escrevê-la erroneamente e acabar em um loop infinito.
- Toda função recursiva tem duas partes: o caso-base e o caso recursivo.
- Caso recursivo é quando a função chama a si mesma.
- Caso-base é quando a função não chama a si mesma novamente, de forma que o programa não se torna um loop infinito.

## Pilha

- Pilha contém apenas duas ações: push (inserir) e pop (remover e ler).
- Quando você insere um item, ele é colocado no topo da pilha.
- Quando você lê um item, le apenas o topo da pilha e ele é retirado da pilha.

## Pilha de chamada (call stack).

- Quando você chama uma função a partir de outra, a chamada de função fica pausada em um estado parcialmente completo.
- Essa pilha é usada para guardar as variáveis de múltiplas funções.
- Todas as chamadas de função vão para a pilha de chamada.
- A pilha de chamada pode ficar muito grande e ocupar muita memória.

Usar a pilha é bom, porém, existe um custo: salvar toda essa informação pode ocupar muita memória. Cada uma destas funções de chamada ocupa um pouco de memória, e quando a sua pilha está muito cheia é sinal de que seu computador está salvando informação para muitas chamadas de funções. Para esta situação, você tem duas opções:

- Reescrever seu código utilizando loops.
- Utilizar o que chamamos de tail recursion (recursão de cauda). Isto é um tópico avançado em recursão. Esta técnica também não é suportada por todas as linguagens de programação.