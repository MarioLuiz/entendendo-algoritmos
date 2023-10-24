# Cap 4: Quicksort

## Dividir para conquistar

- O algoritmos Quicksort utiliza a técnica dividir para conquistar.
- Os algoritmos DC são recursivos.

Passos para aplicação da técnica DC(dividir para conquisatar)

1 - Descubra o caso-base, que deve ser o caso mais simples possível.

2 - Descubra como reduzir o seu problema para que ele se torne o caso-base.

- O algoritmo DC não é um simples algoritmo que você aplica em um problema, mas sim uma maneira de pensar sobre o problema.

## QuickSort

1. Escolher um elemento do array para ser o pivô.
2. Criar 2 SubArrays (esquerdo e direito).
3. Pegar todos numeros menores que o pivô e colocar no sub ArrayMenor(esquerdo).
4. Pegar todos numeros menores que o pivô e colocar no sub ArrayMaior(direito).
5. Pegar o Array esquero e direito e repetir passo 1, 2 ,3 e 4 até que a lista esteja ordenada.
6. Retornar a lista ordenada.

Tempo de execução O(n * Log n).

O desempenho do quicksort depende bastante da escolha do pivô. O melhor caso é o caso médio.