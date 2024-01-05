# Cap 8: Algoritmos Gulosos

- Algoritmos gulosos (também chamados de algoritmos gananciosos)
- São fáceis!
- Às vezes, é suficiente ter um algoritmo eficaz para resolver um problema de forma bastante satisfatória. Os algoritmos gulosos são uma escolha nesses casos, pois são fáceis de implementar e geralmente oferecem soluções muito próximas da ideal.
- A cada etapa, escolhe-se a solução ideal, e no fim você tem uma solução global ideal.
- Algoritmos gulosos nem sempre funcionam, mas eles são tão simples de escrever!
- Às vezes, o melhor é inimigo do bom.

## Ploblema cobertura de conjuntos

Suponha que você esteja começando um programa de rádio e queira atingir ouvintes em todos os cinquenta estados americanos. É necessário decidir em quais estações transmitir para atingir todos os ouvintes. Porém transmitir em diferentes estações tem um custo, e você está tentando minimizar o número de estações nas quais você transmite para minimizar o custo.

- Temos uma lista de estações
- Cada estação abrange uma região e existe uma sobreposição

Como descobrir o menor conjunto de estações nas quais você pode transmitir e abranger os cinquenta estados?

1. Liste cada subconjunto possível de estações. Isso é chamado de conjunto de partes (também conhecido como conjunto de potência). Neste caso, existem 2^n possíveis conjuntos.
2. Entre eles, escolha o conjunto com o menor número de estações que abranja todos os cinquenta estados.

O problema neste caso é que o tempo para calcular cada possível subconjunto de estações é muito longo, uma vez que o tempo de execução é O(2^n), pois existem 2^n subconjuntos.