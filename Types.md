# Tipos de Big O

A notação Big O é uma ferramenta fundamental para analisar a eficiência de algoritmos, descrevendo como o tempo de execução ou o uso de memória cresce à medida que o tamanho da entrada aumenta. Ela é amplamente utilizada para comparar algoritmos e escolher a solução mais eficiente para um problema específico.

## Principais tipos de complexidade Big O:

- O(1) - Complexidade Constante: O tempo de execução é sempre o mesmo, independentemente do tamanho da entrada. Exemplo: acessar um elemento de um array.

- O(log n) - Complexidade Logarítmica: O tempo de execução cresce de forma logarítmica com o aumento da entrada. Exemplo: busca binária em arrays ordenados.

- O(n) - Complexidade Linear: O tempo de execução cresce proporcionalmente ao tamanho da entrada. Exemplo: busca linear em uma lista ou array não ordenado.

- O(n log n) - Complexidade Linearítmica: Combina características lineares e logarítmicas. Exemplo: algoritmos de ordenação como Merge Sort e Heap Sort.

- O(n²) - Complexidade Quadrática: O tempo de execução cresce quadraticamente com o tamanho da entrada. Exemplo: algoritmos de ordenação como Bubble Sort e Insertion Sort.

- O(n^c) - Complexidade Polinomial: O tempo de execução é proporcional a uma potência cc do tamanho da entrada. Exemplo: algoritmos que envolvem decomposição de matrizes.

- O(2^n) - Complexidade Exponencial: O tempo de execução dobra com cada aumento no tamanho da entrada. Exemplo: algoritmos recursivos como o cálculo de Fibonacci.

### A notação Big O é essencial para entender o desempenho de algoritmos, especialmente em cenários com grandes volumes de dados, e ajuda a escolher a abordagem mais eficiente para resolver um problema.

## Algoritmos correspondentes aos exemplos:

- O(1): Acesso direto a um elemento de um array.
- O(Log  n): Busca binária em uma lista ordenada.
- O(n): Busca linear em uma lista.
- O(n log n): Merge Sort, um algoritmo de ordenação eficiente.
- O(n²): Bubble Sort, um algoritmo de ordenação simples.
- O(n^c): Multiplicação de matrizes, que tem complexidade O(n3)O(n3).
- O(2^n): Cálculo recursivo dos números de Fibonacci

## Imagem de exemplo para melhor compreensão.
![Image](img/bigO.jpg)
