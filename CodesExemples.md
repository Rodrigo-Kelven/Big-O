## Código de exemplo.

- ### O(1) - Complexidade Constante: Acesso direto a um elemento de um array. 
Exemplo em C:

        int array = {1, 2, 3, 4, 5};
        int x = array[2]; // O(1)


- ### O(log n) - Complexidade Logarítmica: Busca binária em uma lista ordenada.
Exemplo em C:

        int buscaBinaria(int array[], int tamanho, int valor) {
            int esquerda = 0, direita = tamanho - 1;
            while (esquerda <= direita) {
                int meio = esquerda + (direita - esquerda) / 2;
                if (array[meio] == valor) return meio;
                if (array[meio] < valor) esquerda = meio + 1;
                else direita = meio - 1;
            }
            return -1;
        }

- ### O(n) - Complexidade Linear: Busca linear em uma lista.
Exemplo em C:

        int buscaLinear(int array[], int tamanho, int valor) {
            for (int i = 0; i < tamanho; i++) {
                if (array[i] == valor) return i;
            }
            return -1;
        }

- ### O(n log n) - Complexidade Linearítmica: Merge Sort, um algoritmo de ordenação eficiente.
Exemplo em C:

        void merge(int array[], int inicio, int meio, int fim) {
            int i, j, k;
            int n1 = meio - inicio + 1;
            int n2 = fim - meio;
            int L[n1], R[n2];
            for (i = 0; i < n1; i++) L[i] = array[inicio + i];
            for (j = 0; j < n2; j++) R[j] = array[meio + 1 + j];
            i = 0; j = 0; k = inicio;
            while (i < n1 && j < n2) {
                if (L[i] <= R[j]) array[k] = L[i++];
                else array[k] = R[j++];
                k++;
            }
            while (i < n1) array[k++] = L[i++];
            while (j < n2) array[k++] = R[j++];
        }

        void mergeSort(int array[], int inicio, int fim) {
            if (inicio < fim) {
                int meio = inicio + (fim - inicio) / 2;
                mergeSort(array, inicio, meio);
                mergeSort(array, meio + 1, fim);
                merge(array, inicio, meio, fim);
            }
        }

- ###  O(n²) - Complexidade Quadrática: Bubble Sort, um algoritmo de ordenação simples.
Exemplo em C:

        void bubbleSort(int array[], int tamanho) {
            for (int i = 0; i < tamanho - 1; i++) {
                for (int j = 0; j < tamanho - i - 1; j++) {
                    if (array[j] > array[j + 1]) {
                        int temp = array[j];
                        array[j] = array[j + 1];
                        array[j + 1] = temp;
                    }
                }
            }
        }

- ### O(2^n) - Complexidade Exponencial: Cálculo recursivo dos números de Fibonacci.
Exemplo em C:

        int fibonacci(int n) {
            if (n <= 1) return n;
            return fibonacci(n - 1) + fibonacci(n - 2);
        }
