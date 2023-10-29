# Cap 5: Tabelas Hash

Provavelmente você nunca terá que implementar uma tabela hash na vida, porque as linguagens de programação já fornecem implementação dessa funcionalidade.

## Função hash

- É uma função na qual você insere uma string e ela retorna um número.
- HashTables não permitem valores duplicados, ou seja, ao inserir uma chave que já existe na tabela ela subescreve o valor.

As tabelas hash são úteis para:

- Modelar relações entre dois itens
- Filtrar por duplicatas
- Caching/memorização de dados, em vez de solicitar estes dados do
servidor.

## Colisões

- Duas chaves são indicadas para o mesmo espaço, e isto é um problema.  Colisões são um problema, e você precisa solucioná-lo. Para isso há várias alternativas, e a mais simples é esta: se diversas chaves mapeiam para o mesmo espaço, inicie uma lista encadeada neste espaço.
- A função hash é muito importante. Ela mapeia todas as chaves para um único espaço. Idealmente, a sua função hash mapearia chaves de maneira simétrica por toda a hash.
- Caso as listas encadeadas se tornem muito longas, elas diminuirão demais o tempo de execução da tabela hash. Porém elas não se tornarão muito longas se você utilizar uma boa função hash!

## Desempenho

No caso médio, as tabelas hash têm tempo de execução O(1) para tudo. Assim, O(1) é chamado de tempo constante.

|  | Tabelas Hash
(Caso médio) | Tabelas Hash
(Pior caso) | Arrays | Listas encadeadas |
| --- | --- | --- | --- | --- |
| Procura | O(1) | O(n) | O(1) | O(n) |
| Inserção | O(1) | O(n) | O(n) | O(1) |
| Remoção | O(1) | O(n) | O(n) | O(1) |

No pior caso, as tabelas hash são lentas em ambos os casos. Assim, é importante que você não opere no pior caso; para isso é preciso evitar colisões. Para evitar colisões são necessários:

- Um baixo fator de carga
- Uma boa função hash

## Fator de Carga

- Para calcular o fator de carga de uma tabela hash basta dividir o número de itens na tabela hash pelo número total de espaços.
- O fator de carga mede quantos espaços continuam vazios na sua tabela hash.
- Se o fator de carga começar a crescer, será necessário adicionar mais espaços em sua tabela hash. Isso se chama redimensionamento.
- Uma boa regra geral é: redimensione quando o fator de carga for maior do que 0,7.
- O redimensionamento é caro e não deve ser feito com frequência. No entanto, em média, as tabelas hash têm tempo de execução O(1), mesmo com o redimensionamento.